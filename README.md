# Melbourne Housing Market Analysis

<img src="https://github.com/davarques/Melbourne-Housing-Market/assets/160759223/504e90ce-bddc-4c12-b425-89d13158a37a" width="600">

## Project Overview 📋

In this project, we'll conduct exploratory data analysis (EDA) of Melbourne's housing market dataset from 2016 to 2018 to practice our Python skills. We'll provide the dataset and its information, along with some randomly interesting findings discovered during exploration. For more detailed insights, we recommend reviewing the script attached in teh project, which contains additional details.

### Datasets 💾 
[Melbourne housing market data (2016-2018)](https://raw.githubusercontent.com/dipalira/Melbourne-Housing-Data-Kaggle/master/Data/Melbourne_housing_FULL.csv)

####  Column's Description: 
Here's a breakdown of the columns in the Melbourne Housing DataFrame:

* <span style="font-size: smaller;">**Suburb**: Name of the suburb where the property is located.</span>
* <span style="font-size: smaller;">**Address**: Address of the property.</span>
* <span style="font-size: smaller;">**Rooms**: Number of rooms in the property.</span>
* <span style="font-size: smaller;">**Type**: Type of property (e.g., house, unit, townhouse).</span>
* <span style="font-size: smaller;">**Price**: Price of the property.</span>
* <span style="font-size: smaller;">**Method**: Method of sale (e.g., auction, private sale).</span>
* <span style="font-size: smaller;">**SellerG**: Real estate agent or agency handling the sale.</span>
* <span style="font-size: smaller;">**Date**: Date of sale.</span>
* <span style="font-size: smaller;">**Distance**: Distance from the property to the central business district (CBD) or another point of interest.</span>
* <span style="font-size: smaller;">**Postcode**: Postal code of the area where the property is located.</span>
* <span style="font-size: smaller;">**Bedroom2**: Number of bedrooms (alternate method of recording).</span>
* <span style="font-size: smaller;">**Bathroom**: Number of bathrooms.</span>
* <span style="font-size: smaller;">**Car**: Number of car spaces.</span>
* <span style="font-size: smaller;">**Landsize**: Size of the land associated with the property.</span>
* <span style="font-size: smaller;">**BuildingArea**: Area of the building on the property.</span>
* <span style="font-size: smaller;">**YearBuilt**: Year the property was built.</span>
* <span style="font-size: smaller;">**CouncilArea**: Local council governing the area where the property is located.</span>
* <span style="font-size: smaller;">**Latitude**: Latitude coordinate of the property location.</span>
* <span style="font-size: smaller;">**Longitude**: Longitude coordinate of the property location.</span>
* <span style="font-size: smaller;">**Regionname**: Name of the region where the property is located.</span>
* <span style="font-size: smaller;">**Propertycount**: Number of properties in the area.</span>

## Some Inisghts & Findings 🔍

**Region Analysis:** To spot the cheapest and most expensive regions within Melbourne.

![Screenshot 2024-05-08 at 17 00 37](https://github.com/davarques/Melbourne-Housing-Market/assets/160759223/d003697d-69fe-42b9-bf9d-9a00b34fc32e)

---

Region's grouped in `Price_category` (ranges) visualization with **heatmap**:

* We can see how `Southern Metropolitan` has the highest housing prices. 

<img src="https://github.com/davarques/Melbourne-Housing-Market/assets/160759223/eec0fc2a-1e35-4d16-8d83-46b9990a2f78" width="750">

---

Analysing the the **frequenecy of property types** (houses, units or townhouse)

* The major porperty type sold in Melbour are `houses`

<img src="https://github.com/davarques/Melbourne-Housing-Market/assets/160759223/fe7fd9c5-4645-41e4-bb54-02b689a9b890" width="500">

---

**Box plot** between `Price` and `Time`:

* We can see a high number of `outliers` 

![image](https://github.com/davarques/Melbourne-Housing-Market/assets/160759223/85d15afd-8606-4f1f-b895-a97aec5a30b3)

---

**Scatter Plot:** We can see low negative correlation betwee `Distance` to the city center and `Price`. 

<img src="https://github.com/davarques/Melbourne-Housing-Market/assets/160759223/d58bcd1f-179d-42e1-8cf5-6dd71547be67" width="600">

---

**Scatter Plot:** No correlation betwee `Landsize` and `Price`. 

<img src="https://github.com/davarques/Melbourne-Housing-Market/assets/160759223/481b03e6-707b-4a77-b76c-dc1dcdbdefaf" width="600">

---

Relation between number of `Rooms` and `Price` 

* We can see weak or no realtion between `Rooms` and `Price`

![Screenshot 2024-05-08 at 16 56 49](https://github.com/davarques/Melbourne-Housing-Market/assets/160759223/bedc8cd4-bafc-4841-b68e-ae4e98528f17)

---

**QQ Plot**

<img src="https://github.com/davarques/Melbourne-Housing-Market/assets/160759223/59ff8f08-bad3-4036-9bc1-de9d376e2905" width="600">

Skewness and Kurtosis results:

![Screenshot 2024-05-08 at 17 18 47](https://github.com/davarques/Melbourne-Housing-Market/assets/160759223/20b02b85-57c8-43d7-adfa-ba15e689d49f)

* Skewness of 2.59 suggests a right-skewed distribution, indicating fewer extreme high values.
* Kurtosis of 13.10 indicates heavy-tailedness, implying more extreme values than a normal distribution. These findings highlight the presence of outliers in the dataset, which could impact analysis and modeling.
