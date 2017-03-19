# Medicare_and_medicaid_prescription_data

The notebooks in this repository perform exploratory analysis on the data avialable from Medicaid and Medicare website. The data provides valuable information about doctors/practitioners such as their specialty, years of practicing, region, gender etc. It also provides information about the drugs they have prescribed and their counts. Understanding the trends can be very helpful for doctors/practitioners to get information about drugs presrcibed by fellow practioners in their specialty. The data can also be used for drug manufacturers/providers to understand the prescription requirements of each specialty, and may assist them in designing personalized catalog of each individual doctor catering to their needs.

There are 3 notebooks in this repository.

*(NOTE : Some of the notebooks are not rendered properly on GitHub. Please click on the link to the nbviewer to access these notebooks).*

1. Prescription Data - Exploratory Analysis

The notebook provides valuable information and statistics about the doctors. It provides information about distriubtion of doctors based on the region that they are from, gender etc. , and percent of doctor belonging to each specialty.

LINK : http://nbviewer.jupyter.org/github/toofanix/Medicare_and_medicaid_prescription_data/blob/master/Prescription%20Data%20-%20Exploratory%20Analysis.ipynb

2. Prescription Data - Machine Learning - Supervised Learning

The notebook uses Logistic Regression using the drugs prescribed by a doctor/practitioner as input features and tries to predict gender, specialty and region. Using logistic regression it is possible to predict the specialty of the preactitioner with ~81% accuracy. It is interesting to note that some specialties (Adult Health and Medical) are hard to predict and are mostly mis-classified as Family. I use LIME to understand the regression model for the specialty 'Psychiatry' and 'Adult Health' to understand how and which features are used for prediction.

3. Prescription Data - Low Dimensional Representation and Unsupervised Machine Learning

The notebook using PCA, Isomap and TSNE to generate a low-dimensional representation of the prescription data. Using TSNE it can be observed that specialties 'Cardiovascular Disease', 'Endocrinology, Diabetes & Metabolism', 'Geriatric Medicine', 'Nephrology', 'Neurology', 'Psychiatry' and 'Rheumatology' form separate clusters whereas 'Adult Health', 'Family' and 'Medical' overlap and form one cluster. The 3D visualization gives us a better sense of why regression analysis in the preivous notebook was unable to predict the specialties 'Adult Health', 'Family' and 'Medical' robustly.

The notebook also has some preliminary clustering analysis using KMeans, DBSCAN, Affinity Propogation and HDBSCAN*. 

