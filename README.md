![image](https://github.com/user-attachments/assets/5628137b-feb3-4e0f-b7c3-c9340ae469eb)<h3 align='center'>Auto Graphical Exploratory Data Analysis</h3>

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
   ![image](https://github.com/user-attachments/assets/b300efff-f9e0-4255-8df0-45853cdc9642)

> User can find rules to classify data based on distribution plots. <br>
> For example the distribution plot between both of the distributions and at MajorAxisLength=400 and so MajorAxisLength>400 as Besni and MajorAxisLength<=400 as Kecimen.
> The box plots of various features compares the distribution of the features against classes. The user can clearly view that there are several outliers in the given data. Outliers for MajorAxisLength and Perimeter are towards extreme high values while outliers for Extent and Eccentricity are towards extreme low values.
> Both of these observations can be clearly viewed from violin plots by observing the shape of distribution over the box plot.

6. Following is a piar plot between MajorAxisLength and Extent
   ![image](https://github.com/user-attachments/assets/349ee8a4-e5ca-4b36-b515-4ad7f8944e43)

8. Following is a pair plot between Extent and Perimter
   ![image](https://github.com/user-attachments/assets/ab3a61cf-eb7b-46cd-bbb3-b0b4fa4beb69)

10. Following is a pair plot between MajorAxisLength and Perimter
    ![image](https://github.com/user-attachments/assets/62b13d1d-e517-4165-b6e2-7401fc608a70)

12. Following is a pair plot between Perimeter and Eccentricity
    ![image](https://github.com/user-attachments/assets/beeaa0cc-f3c4-4849-b45e-54c079e6feb9)

14. Following is a pair plot between MajorAxisLength and Eccentricity
    ![image](https://github.com/user-attachments/assets/a281767b-a2e3-4388-ac3e-58eb102a1d25)

16. Following is a pair plot between Extent and Eccentricity
    ![image](https://github.com/user-attachments/assets/5a96b03e-756e-4e00-ad68-ff1b98ef2d9b)

> The scatter plots between pair of features of the four features are present here.
> This could help a user infer the distribution of data items in these two feature space.
> Since the classification boundary is subjective to user for imagination, the user may intend to draw a decision boundary at a place which need not be true. Hence we have introduced the concept of `classifiable pair plots`. These plots clearly mention where the classification boundary can be drawn. This is essential as the plotting of one class of data over other may hinder users from having a holistic view of the spread of the dataitems in the feature space. The classifiable pair plots considers a classification boundary considering all the data items. This approach ensures a clearer understanding of data distribution and minimizes the risk of subjective misinterpretation, providing a more accurate basis for defining and evaluating classification models.


<!--
<h3> Methodology </h3>

**Step-1: Data input**
> 1. Data present in either of the two file formats: csv, xlsx should be fed as input. <br>
> 2. If the input dataset is an excel file having more than one sheet, user is prompted with all the available sheets to enter the sheet containing the dataset for analysis.

**step-2: Data Preprocessing**
-->
