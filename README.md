# Project overview: Unsupervised learning - customer clustering
Project: Customer clustering. The project is part of Udacity 'Introducton to Machine Learning with Tensorflow' excersises. 

In this project, unsupervised learning techniques are applied to identify segments of the population that form the core customer base for a mail-order sales company in Germany. In first step Germany demographics data is used to identify relevant segments in general population. The segmentation model is then applied on the mail-order company customer data to segment the customer based on the general population segments. These segments can then be used to direct marketing campaigns towards audiences that will have the highest expected rate of returns.

The key analysis steps performed are:
1. Loading the data and interpreting the content
2. Demographics data cleansing
	- Preprocessing the data (handling missing data and cleansing features/data rows with high share of NaNs) 
	- Selecting and re-econding/engineering features to numeric data (non-numeric, categorical or mixed type features)
	- Summarizing the preprocessing, feature selection and re-econding/engineering phases into single data cleansing function
3. Applying feature tranformations for cleaned demographics data
	- Feature scaling
	- PCA based dimensionality reduction
	- Intrepreting the PCA components
4. Clustering the transformed demographics data
    - Apply KMeans clustering to the data and identifying optimal number of clusters using avg. distance error curve
	- Apply optimal cluster nr. to cluster the data
5. Applying demographic cluster model to company customer and interpreting the results
	- Cleansing the customer data 
	- Clustering the company customer data using the demographics clustering model
	- Comparing the clustering results on customer data vs demographcis to identify over/underrepresented clusters

### Data

The demographic data used in the project is provided by Bertelsmann Arvato Analytics. Data is not included in the GitHub repository due to copyright. 

Data and the data descsriptions are included in the four files:
- `Udacity_AZDIAS_Subset.csv` Demographics data for the general population of Germany; 891211 persons (rows) x 85 features (columns). (not included in github due to copyright)
- `Udacity_CUSTOMERS_Subset.csv` Demographics data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns). (not included in github due to copyright)
- `Data_Dictionary.md` Detailed information file about the features in the provided datasets.
- `AZDIAS_Feature_Summary.csv` Summary of feature attributes for demographics data; 85 features (rows) x 4 columns


### Code and files

- `Identify_Customer_Segments.ipynb` Jypter notebook file with the main code and analysis. 
- `helper_functions.py` Python scripts to help on printing intermediate results and visualisations.
- `Data_Dictionary.md` Detailed information file about the features in the provided datasets.
- `AZDIAS_Feature_Summary.csv` Summary of feature attributes for demographics data; 85 features (rows) x 4 columns

### Install

This project requires **Python 3.x** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [seaborn](https://seaborn.pydata.org/)

You will also need to have Juypyter software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html)

### Run

In a terminal or command window run the following commands:

```bash
jupyter notebook Identify_Customer_Segments.ipynb
```  
