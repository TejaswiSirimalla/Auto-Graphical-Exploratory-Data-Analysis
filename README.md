<h3 align='center'>Auto Graphical Exploratory Data Analysis</h3>

**Auto Graphical Exploratory Data Analysis** is an automated system designed to generate comprehensive graphical analysis of datasets, facilitating users in understanding the underlying structures and patterns in data, focused towards machine learning tasks such as classification, regression, and clustering.

**Libraries Used**: `pandas`, `numpy`, `matplotlib`, `plotly`, `bokeh`, `scikit-learn`, `math`, `statsmodels`, `os`, `warnings`

**Input**
> 1. Data present in either of the two file formats: csv, xlsx should be fed as input. <br>
> 2. If the input dataset is an excel file having more than one sheet, user is prompted with all the available sheets to enter the sheet containing the dataset for analysis.

**Reference Dataset used** : `Raisin` dataset from University of California, Irvine's ML repository [Link](https://archive.ics.uci.edu/dataset/850/raisin)

Given a dataset, a user tries to find patterns and build a model of interest over the data. Most of these models either fall under supervised or unsupervised ML. In this project, a user can perform graphical analysis over the given dataset with the intention of building a classifier or a regressor or for finding clusters in the data. This allows a user to perform a dedicated graphical analysis with the ML task of interest. The aim is to let the user gain visual understanding of the overall dataset from the view of the user's ML task of interest. To achieve this, we have relied on Shannon's entropy and Information gain to select not more than 4 most relevant features guided by the user's ML task.

In the reference dataset, as per (https://archive.ics.uci.edu/dataset/850/raisin), following are the list of columns
> 1. Area: represents number of pixels present within the boundaries of a raisin.
> 2. Perimeter: calculates the distance between pixels and between the boundaries of raisin.
> 3. MajorAxisLength: represents length of the main axis on the raisin.
> 4. MinorAxisLength: represents length of the small axis on the raisin
> 5. Eccentricity: It represents eccentricity of the ellipse of raisins.
> 6. ConvexArea: represents number of pixels of the smallest convex shell of the region formed by the raisin.
> 7. Extent: represents ratio of region formed by raisin to the total pixels in the bounding box.
> 8. Class: Kecimen and Besni raisin.

When the user intends to build a classifier over `Class` dependent column, the project suggests that the following are the 4 most relevant features: 
> 1.MajorAxisLength
> 2.Perimeter
> 3.Extent
> 4.Eccentricity

<h4>Screenshots</h4>

1. Following are the plots for the feature: MajorAxisLength
   ![image](https://github.com/user-attachments/assets/e055be9f-fa23-4843-9519-79bb54df1e7d)

2. Following are the plots for the feature: Perimeter
   ![image](https://github.com/user-attachments/assets/a47de951-5284-4711-a864-17147e2cdda3)

3. Following are the plots for the feature: Extent
   ![image](https://github.com/user-attachments/assets/095207cc-62fa-425a-bd60-b0568775624a)

5. Following are the plots for the feature: Eccentricity

<!--
<h3> Methodology </h3>

**Step-1: Data input**
> 1. Data present in either of the two file formats: csv, xlsx should be fed as input. <br>
> 2. If the input dataset is an excel file having more than one sheet, user is prompted with all the available sheets to enter the sheet containing the dataset for analysis.

**step-2: Data Preprocessing**
-->
