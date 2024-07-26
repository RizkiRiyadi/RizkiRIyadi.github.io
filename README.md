# Rizki's Portfolio
## About
Hi, I'm Rizki! I am an fresh graduate from Binus and majoring Industrial Engineering. I am intersted in data analytic in supply chain especially Production Planning & Inventory Control (PPIC). I have developed pretty strong understanding in forecasting because of my thesis. 

## Table of Contents
- [About](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/README.md#about)
- [Portofolio Projects](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/README.md#protofolio-projects)
  - Python 
    - [Forecasting Natural Gas Demand Using The Auto Arima And Facebook Prophet Method To Accelerate The Process Of Confirming Gas Availability In Value Stream Mapping (VSM) PT. Perusahaan Gas Negara Tbk](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/README.md#Forecasting-Natural-Gas-Demand-Using-The-Auto-SARIMA-and-Facebook-Prophet-Method-To-Accelerate-The-Process-Of-Confirming-Gas-Availability-With-Value-Stream-Mapping-(VSM)-at-PT.-Perusahaan-Gas-Negara-Tbk)
    - [Supply Chain](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/README.md#supply-chain)
  - SQL
    - [Beauty Center Database](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/README.md#beauty-center-database)
- [CV](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/README.md#cv)
- [Contacts](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/README.md#contacts)

## Protofolio Project

### Forecasting Natural Gas Demand Using The Auto SARIMA And Facebook Prophet Method To Accelerate The Process Of Confirming Gas Availability With Value Stream Mapping (VSM) at PT. Perusahaan Gas Negara Tbk
**Code:** [here](https://github.com/RizkiRiyadi/ForecastGasDemandKarawang/blob/main/Sarima_Prophet.ipynb)

**Paper:** [here](https://drive.google.com/file/d/1q_EdiAQxdWOSzgbl0E5lwcdnXckU9rCZ/view?usp=sharing)

**Description:** This is my thesis project focuses on forecasting gas demand for industrial sector customers in Karawang Regency using the Facebook Prophet and auto ARIMA forecasting methods to speed up the process of confirming customer gas availability using Value Stream Mapping (VSM). Currently, PGN faces challenges in planning accurate and timely  gas  distribution,  this  is  caused by inaccurate customer gas usage and PGN still uses qualitative forecasting. This is made worse by the lack of employee awareness in prioritizing gas distribution planning and this process takes a long time, so that confirmation of gas availability is often late.

**Goals:**
- Know the best forecasting method to predict gas demand for industrial sector customers in Karawang Regency at PT. Perusahaan Gas Negara Tbk.
- Know the characteristics of gas usage by industrial sector customers in Karawang Regency at PT Perusahaan Gas Negara Tbk.


**Findings:**

![OverviewData](https://github.com/RizkiRiyadi/ForecastGasDemandKarawang/blob/main/ForecastPhotos/OverviewData.png)
![Decomposition](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/ForecastPhotos/time%20series%20decomposition.png)


In the picture above we can see there are weekly seasonality in gas usage data. So we using Seasonal Autoregressive Integrated Moving Average (SARIMA) instead of Autoregressive Integrated Moving Average (ARIMA)

![Train_Test_Forecast_SARIMA](https://github.com/RizkiRiyadi/ForecastGasDemandKarawang/blob/main/ForecastPhotos/Train_Test_Forecast_SARIMA.png)

For our best model in auto SARIMA we cannot forecast sudden drop in our gas demand, so we are using facebook prophet that well known best foreceasting method to maintan sudden spike in demand


![Actual_Forecast_Prophet_Extended Holiday](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/ForecastPhotos/Actual%20and%20Forecast%20Data%20Prophet%20With%20Extended%20Holiday.png)

With facebook prophet we can forecast the sudden demand drop when idul fitri.

![ForecastAccuracy](https://github.com/RizkiRiyadi/ForecastGasDemandKarawang/blob/main/ForecastPhotos/ForecastAccuracy.png)

I tried many well know forecasting method and i get facebook prophet as the best method for my data.

![CVSM](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/ForecastPhotos/CVSM.png)

Forecasting is one of many step to confirming gas availbility to customer. I am using Value Stream Mapping and time study to improve this process, removing waste, and shorten bureaucracy.

![FVSM](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/ForecastPhotos/FVSM.png)

With my propsed Future State Value Stream Mapping we can get rid of time) waste as many as 371.23 minutes.

<br/>

### Supply Chain
**Repo:** [here](https://github.com/RizkiRiyadi/Supply_Chain_Case/blob/main/Supply-Chain-EDA.ipynb)

**Description:** Supply chain analytics is a valuable part of data-driven decision-making in various industries such as manufacturing, retail, healthcare, and logistics. It is the process of collecting, analyzing and interpreting data related to the movement of products and services from suppliers to customers.

Here is a dataset that i use from Fashion and Beauty startup. The dataset is based on the supply chain of Makeup products. Below are all the features in the dataset:

- Product Type
- SKU
- Price
- Availability
- Number of products sold
- Revenue generated
- Customer demographics
- Stock levels
- Lead times
- Order quantities
- Shipping times
- Shipping carriers
- Shipping costs
- Supplier name
- Location
- Lead time
- Production volumes
- Manufacturing lead time
- Manufacturing costs
- Inspection results
- Defect rates
- Transportation modes
- Routes
- Costs

**Goal:**
- Analyze data using data visualization to find area of improvement

**Findings:**

![Correlatiom](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/SupplyChainPhotos/CorrelationAnalysisTop5.png)

- Price with manufacturing lead time indicate weak negative linear relationship with -0,3 value.
- Order quantities with costs indicate weak linear positive linear realationship with 0,17 value.
- Other than that realationship with other columns have low significance.

![SalesRevenue](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/SupplyChainPhotos/Sales%26RevenueAnalysis.png)

- The higher the price of skincare product the more revenue generated.
- The lower the price of cosmetics and haircare products the less revenue generated.
  
![SalesProductType](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/SupplyChainPhotos/SalesByProductType.png)
![RevenueByProduct](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/SupplyChainPhotos/RevenueByProduct.png)

- Skincare product type is the best selling  and the most revenue generated
  
![DefectCarriers](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/SupplyChainPhotos/DefectRatesShipping.png)
![DefectTranspot](https://github.com/RizkiRiyadi/RizkiRiyadi.github.io/blob/main/SupplyChainPhotos/DefectRateTransportModes.png)

- Defect rates for different shipping carriers relatively same, so defect rates doesn't effect by type of shipping carriers.
- Defect rates by transportation modes lead by road modes. This means item with road modes more likely to broke.
  
<br/>

### Beauty Center Database
- **Repo:**
  - Data Definition Language (DDL): [here](https://github.com/RizkiRiyadi/BeautyCenterDatabase/blob/main/Query%20B%20DDL.sql)
  - Data Manipulation Language (DML):
    - Database: [here](https://github.com/RizkiRiyadi/BeautyCenterDatabase/blob/main/Query%20C%20DML.sql)
    - Transactions Simulation: [here](https://github.com/RizkiRiyadi/BeautyCenterDatabase/blob/main/Query%20D%20DML%20simulate.sql)
  - Query Case: [here](https://github.com/RizkiRiyadi/BeautyCenterDatabase/blob/main/10%20case%20Query%20E.sql)
 
    
**Description:**

**Goal:**

**Findings:**

*hsdsd
![ERD](https://github.com/RizkiRiyadi/BeautyCenterDatabase/blob/main/Beauty%20Center%20ERD.png)


## CV
Link: [here](https://drive.google.com/file/d/1xZBB3X-Lh30Yw9mKAcJqkjlQJHtzz5mU/view?usp=sharing)

## Contacts
- LinkedIn: [Mohammad Rizki Riyadi](https://www.linkedin.com/in/mohammad-rizki-riyadi/)
- Email: rizkiriyadi76@gmail.com


