
<img src="http://imgur.com/1ZcRyrc.png" style="float: left; margin: 20px; height: 55px">
# Kaggle Challenges - House Prices (Regression)

![housesbanner](https://storage.googleapis.com/kaggle-competitions/kaggle/5407/media/housesbanner.png)

This is project for Data Science Immersive course from General Assembly.

## Table of contents
* [Problem Statement](#Problem-Statement)
* [Datasets Description](#Datasets-Description)
* [Data Dictionary](#Data-Dictionary)
* [Conclusions](#Conclusions)
* [Reference](#Reference)
* [Group Members](#Group-Members)


## Problem Statement <a name="Problem-Statement"></a>

This a python script project is about house pricing competition on Kaggle, which aims to apply EDA and machine learning models in order to predict the house pricing for Ames Housing dataset.

As a home buyer to describe their dream house, and they probably won't begin with the height of the basement ceiling or the proximity to an east-west railroad. However, we can confidently say that more attributes influences price negotiations than the number of bedrooms or a white-picket fence. With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, we built a machine learning model that predicts the final price of each home.



## Datasets Description <a name="Datasets-Description"></a>

This is the link to the dataset used for this project:

* [Ames Housing Dataset](https://www.kaggle.com/prevek18/ames-housing-datas)



##  Data Dictionary <a name="Data-Dictionary"></a>

The dataset's features listed bellow:

|Feature|Type|Dataset|Description|
|---|---|---|---|
|Id|int|df|Id of the house|
|MSSubClass|int|df|Identifies the type of dwelling involved in the sale|
|MSZoning|object|df|Identifies the general zoning classification of the sale|
|LotFrontage|float|df|Linear feet of street connected to property|
|LotArea|int|df|Lot size in square feet|
|Street|object|df|Type of road access to property|
|Alley|object|df|Type of alley access to property|
|LotShape|object|df|General shape of property|
|LandContour|object|df|Flatness of the property|
|Utilities|object|df|Type of utilities available|
|LotConfig|object|df|Lot configuration|
|LandSlope|object|df|Slope of property|
|Neighborhood|object|df|Physical locations within Ames city limits|
|Condition1|object|df|Proximity to various conditions|
|Condition2|object|df|Proximity to various conditions (if more than one is present)|
|BldgType|object|df|Type of dwelling|
|HouseStyle|object|df|Style of dwelling|
|OverallQual|int|df|Rates the overall material and finish of the house|
|OverallCond|int|df|Rates the overall condition of the house|
|YearBuilt|int|df|Original construction date|
|YearRemodAdd|int|df|Remodel date (same as construction date if no remodeling or additions)|
|RoofStyle|object|df|Type of roof|
|RoofMatl|object|df|Roof material|
|Exterior1st|object|df|Exterior covering on house|
|Exterior2nd|object|df|Exterior covering on house (if more than one material)|
|MasVnrType|object|df|Masonry veneer type|
|MasVnrArea|float|df|Masonry veneer area in square feet|
|ExterQual|object|df|Evaluates the quality of the material on the exterior|
|ExterCond|object|df|Evaluates the present condition of the material on the exterior|
|Foundation|object|df|Type of foundation|
|BsmtQual|object|df|Evaluates the height of the basement|
|BsmtCond|object|df|Evaluates the general condition of the basement|
|BsmtExposure|object|df|Refers to walkout or garden level walls|
|BsmtFinType1|object|df|Rating of basement finished area|
|BsmtFinSF1|int|df|Type 1 finished square feet|
|BsmtFinType2|object|df|Rating of basement finished area (if multiple types)|
|BsmtFinSF2|int|df|Type 2 finished square feet|
|BsmtUnfSF|int|df|Unfinished square feet of basement area|
|TotalBsmtSF|int|df|Total square feet of basement area|
|Heating|object|df|Type of heating|
|HeatingQC|object|df|Heating quality and condition|
|CentralAir|object|df|Central air conditioning|
|Electrical|object|df|Electrical system|
|1stFlrSF|int|df|First Floor square feet|
|2ndFlrSF|int|df|Second floor square feet|
|LowQualFinSF|int|df|Low quality finished square feet (all floors)|
|GrLivArea|int|df|Above grade (ground) living area square feet|
|BsmtFullBath|int|df|Basement full bathrooms|
|BsmtHalfBath|int|df|Basement half bathrooms|
|FullBath|int|df|Full bathrooms above grade|
|HalfBath|int|df|Half baths above grade|
|BedroomAbvGr|int|df|Bedrooms above grade (does NOT include basement bedrooms)|
|KitchenAbvGr|int|df|Kitchens above grade|
|KitchenQual|object|df|Kitchen quality|
|TotRmsAbvGrd|int|df|Total rooms above grade (does not include bathrooms)|
|Functional|object|df|Home functionality (Assume typical unless deductions are warranted)|
|Fireplaces|int|df|Number of fireplaces|
|FireplaceQu|object|df|Fireplace quality|
|GarageType|object|df|Garage location|
|GarageYrBlt|float|df|Year garage was built|
|GarageFinish|object|df|Interior finish of the garage|
|GarageCars|int|df|Size of garage in car capacity|
|GarageArea|int|df|Size of garage in square feet|
|GarageQual|object|df|Garage quality|
|GarageCond|object|df|Garage condition|
|PavedDrive|object|df|Paved driveway|
|WoodDeckSF|int|df|Wood deck area in square feet|
|OpenPorchSF|int|df|Open porch area in square feet|
|EnclosedPorch|int|df|Enclosed porch area in square feet|
|3SsnPorch|int|df|Three season porch area in square feet|
|ScreenPorch|int|df|Screen porch area in square feet|
|PoolArea|int|df|Pool area in square feet|
|PoolQC|object|df|Pool quality|
|Fence|object|df|Fence quality|
|MiscFeature|object|df|Miscellaneous feature not covered in other categories|
|MiscVal|int|df|$Value of miscellaneous feature|
|MoSold|int|df|Month Sold (MM)|
|YrSold|int|df|Year Sold (YYYY)|
|SaleType|object|df|Type of sale|
|SaleCondition|object|df|Condition of sale|

## Conclusions <a name="Conclusions"></a>

As a second project in our Data Science Immersive Course with General Assembly and MiSK Academy, we were asked to finish this "House Prices" Competition in Kaggle, We used multiple data cleaning methods, employed (EDA) methods including a good number of visualizations, to get to know the data well, and we preprocessed our dataset with some transformation methods. Finally, we applied multiple machine learning methods in order to predict the Sale Price of the houses in the test data set. The regrission models used were Linear, Ridge, Lasso, Elastic Net, KNN, Decision Tree, Random Forest and a few more models. We achieved an amazing score in Kaggle competition that we are very proud of, we were ranked as the 607th out of 4,675 teams.

Root-Mean-Squared-Error (RMSE) = 0.11890


* ![our Score on Kaggle](score/Group5_score.png)

* ![our rank on Kaggle](score/Group5_ranking_score.png)

## Reference <a name="Reference"></a>

The link bellow is for our Kaggle Challenges House Prices
* [Kaggle Challenges House Prices](https://www.kaggle.com/raghadalharbi/kernel7735b2acfc)


## Group Members <a name="Group-Members"></a>

* [Raghad Alharbi](https://www.kaggle.com/raghadalharbi)
* [Fatimah Aljohani](https://www.kaggle.com/fatmahaljohani)
* [Hessah Hamed Alkhattabi](https://www.kaggle.com/hessahalkhattabi)

