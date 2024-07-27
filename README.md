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
**Repo:**
  - Data Definition Language (DDL): [here](https://github.com/RizkiRiyadi/BeautyCenterDatabase/blob/main/Query%20B%20DDL.sql)
  - Data Manipulation Language (DML):
    - Database: [here](https://github.com/RizkiRiyadi/BeautyCenterDatabase/blob/main/Query%20C%20DML.sql)
    - Transactions Simulation: [here](https://github.com/RizkiRiyadi/BeautyCenterDatabase/blob/main/Query%20D%20DML%20simulate.sql)
  - Query Case: [here](https://github.com/RizkiRiyadi/BeautyCenterDatabase/blob/main/10%20case%20Query%20E.sql)
 
    
**Description:** Madyline is a beauty center managed by your best friend, Mady. Mady manage all of activities that belongs to Madyline like provide beauty treatment service to customer and purchasing the
beauty product with supplier. To improve Madyline’s management, Mady hired you as a database administrator are required to analyze and design a database for Bob’s shop using SQL Server Management Studio. 

**Goal:**
1. Create Entity Relationship Diagram to maintain service transactions and purchase transactions.
2. Create a database system using DDL syntax that relevant with service transactions and purchase transactions.
3. Create query using DML syntax to fill the tables in database systems with data based on the following conditions:
    - Master table must be filled with more than or equals 10 data.
    - Transaction table must be filled with more than or equals 15 data.
    - Transaction detail table must be filled with more than or equals 25 data. 
4. Create query using DML syntax to simulate the transactions process for service transactions and purchase transactions. Note: DML syntax to fill database and DML syntax to simulate the transactions process should be a different query.
5.  Provide some query that resulting important data

**Answer:**
1. ERD to maintain service transactions and purchase transactions.
   I am using 3NF relational database, with that i can minimize redudancy and make database work faster
  ![ERD](https://github.com/RizkiRiyadi/BeautyCenterDatabase/blob/main/Beauty%20Center%20ERD.png)

5.  Provide some query that resulting important data
- Display EmployeeName, SupplierID, and Purchase Transaction Quantity (obtained from the  sum  of  quantity),  and  PaymentType  for  every  purchase
  ```
  transaction  which  the the transaction happened on the 25   day and the id of the supplier is ‘SPR008’.
    select EmployeeName, SupplierID, [Purchase Transaction Quantity] = sum(PurchaseTransactionQuantity), PaymentTransactionType 
  from Employee e
  	join PurchaseTransctionDetail ptd on e.EmployeeID = ptd.EmployeeID
  	join PurchaseTransaction pt on ptd.PurchaseTransactionID = pt.PurchaseTransactionID
  where SupplierID = 'SPR008' and day(PurchaseTransactionDate) ='25'
  group by EmployeeName, SupplierID, PaymentTransactionType
  ```
  ![image](https://github.com/user-attachments/assets/cbc7a194-a2d8-4e81-b810-95882573aadc)

- Display  CustomerID,  CustomerName,  ServiceTransactionDate  and  Total  Treatment (obtained from the count of the treatment) for every customer whose gender is female and the Total Treatment is greater than 2.
  ```
  select c.CustomerID, CustomerName, ServiceTransactionDate, [Total Treatment] = count(TreatmentID) 
  from Customer c
  	join ServiceTransactionDetail std on c.CustomerID = std.CustomerID
  	join ServiceTransaction st on st.ServiceTransactionID = std.ServiceTransactionID
  where CustomerGender = 'Female' 
  group by c.CustomerID, CustomerName, ServiceTransactionDate
  having count(TreatmentID) > 2
  ```
  ![image](https://github.com/user-attachments/assets/90ba659b-9c4a-4c66-b5b0-5ffa314390d7)

- Display SupplierName, Purchase Transaction Date (obtained from purchase date in ‘yyyy.mm.dd’), Total Product Type (obtained from the count of product purchased), and Total Quantity (obtained from the sum of quantity) for every purchase transaction which the transaction happened on the 9 month and Total Quantity is greater than 200. 
  ```
  select SupplierName, [Purchase Transaction Date] = convert(varchar, PurchaseTransactionDate, 102), 
  	[Total Product Type] = count(ProductID), [Total Quantity] = sum(PurchaseTransactionQuantity)
  from PurchaseTransaction pt
  	join Supplier s on s.SupplierID = pt.SupplierID
  where month(PurchaseTransactionDate) = '9' 
  group by SupplierName, PurchaseTransactionDate
  having sum(PurchaseTransactionQuantity) > 200
  ```
  ![image](https://github.com/user-attachments/assets/73e33728-2db7-47e9-8ab3-37c2a6679f7f)

- Display  CustomerName  (obtained  from  customer’s  name  in  uppercase  format), CustomerGender, RoomThemeName,  and  Service  Transaction  Date obtained from service date in ‘yyyy.mm.dd’) for every service transaction that happened on the 25  day and the salary of employee is less than the average of all employee’s salary. (alias subquery)
  ```
   select EmployeeName, [Employee Gender] = left(EmployeeGender, 1), CustomerName, 
  	[Total Service Transaction] = count(st.ServiceTransactionID)
    from Employee e
    	join ServiceTransaction st on e.EmployeeID = st.EmployeeID
    	join ServiceTransactionDetail std on std.ServiceTransactionID = st.ServiceTransactionID
    	join Customer c on c.CustomerID = std.CustomerID
    where day(ServiceTransactionDate) % 2 = 0
    group by EmployeeName, EmployeeGender, CustomerName, st.ServiceTransactionID
    having avg(EmployeeSalary) < 5000000
  ```
  ![image](https://github.com/user-attachments/assets/a3275168-6b05-4133-aad8-fcf428b79842)

- Display  CustomerName  (obtained  from  customer’s  name  in  uppercase  format), CustomerGender, RoomThemeName,  and  Service  Transaction  Date (obtained from service date in ‘yyyy.mm.dd’) for every service transaction that happened on the 25  day and the salary of employee is less than the average of all employee’s salary. (alias subquery) 
 ```
  select [CustomerName] = upper(CustomerName), CustomerGender, RoomThemeName, 
	[Service Transaction Date] = convert(varchar, ServiceTransactionDate, 102)
  from Customer c 
  	join ServiceTransactionDetail std on std.CustomerID = c.CustomerID
  	join ServiceTransaction st on st.ServiceTransactionID = std.ServiceTransactionID
  	join RoomTheme rt on st.RoomThemeID = rt.RoomThemeID
  	join Employee e on e.EmployeeID = st.EmployeeID,
  	(select Average = avg(EmployeeSalary) from Employee) as x
  where day(ServiceTransactionDate) = '25' 
  	and EmployeeSalary < x.Average
  group by CustomerGender, RoomThemeName, ServiceTransactionDate, CustomerName
  ```
  ![image](https://github.com/user-attachments/assets/1e470dce-b033-41a3-a5cf-80ab265920ed)

- Display SupplierName, PurchaseDate (obtained from purchases date in ‘Mon dd, yyyy’ format), and ProductName (obtained from the product’s name in lowercase format) for every purchase transaction with product price is greater than the average price of all products and the supplier’s name ends with ‘Distribution’. (alias subquery) 
  ```
  select SupplierName, PurchaseDate = convert(varchar, PurchaseTransactionDate, 107), ProductName = lower(ProductName)
  from Supplier s, PurchaseTransaction pt, Product p, (select Average = avg(ProductPrice) from Product) as x
  where s.SupplierID = pt.SupplierID 
  	and p.ProductID = pt.ProductID 
  	and  ProductPrice > x.Average
  	and SupplierName like '% Distribution'
  group by SupplierName, PurchaseTransactionDate, ProductName

  ```
  ![image](https://github.com/user-attachments/assets/234ee5e7-3272-43c4-961b-efc06dbfe4bf)

- Display Total Purchase Transaction (obtained from count of purchase transactions and ended  with  ‘  Transaction(s)’),  SupplierName,  Employee  Name (obtained  from employee’s  name  from  the  first  character  until  a  character  before  space),  and PurchaseTransactionDate for every purchase transaction with the quantity is lower than the average quantity of all purchase transaction and the purchase transaction happened on Wednesday. (alias subquery)
  ```
  Select [Total Purchase Transaction] = cast(count(pt.PurchaseTransactionID) as varchar) + ' Transaction(s)', SupplierName, 
  	[Employee Name] = LEFT(EmployeeName,CHARINDEX(' ',EmployeeName + ' ')-1), PurchaseTransactionDate
  from PurchaseTransaction pt, Supplier s, Employee e, PurchaseTransctionDetail ptd,
  	(select Average = avg(PurchaseTransactionQuantity) from PurchaseTransaction) as z
  where s.SupplierID = pt.SupplierID
  	and pt.PurchaseTransactionID = ptd.PurchaseTransactionID
  	and e.EmployeeID = ptd.EmployeeID
  	and PurchaseTransactionQuantity < z.Average 
  	and datename(weekday, PurchaseTransactionDate) = 'Wednesday'
  group by SupplierName, EmployeeName, PurchaseTransactionDate
  ```
  ![image](https://github.com/user-attachments/assets/a54f5293-c78f-4db5-a1fe-a39f116a9009)

- Display SupplierName, Purchase Transaction Date (obtained from purchases date in ‘mm/dd/yyyy’ format), ProductName, Product Number (obtained from ProductID by replacing the first three characters with ‘PR’), and Total Purchase Transaction (obtained from the count of the transaction) for every purchase transaction where the quantity is lower than the sum of all quantity that have ProductID is ‘PDT005’. Sort the result by supplier name in descending order (alias subquery)
  ```
  select SupplierName, [Purchase Transaction Date] = convert(varchar, PurchaseTransactionDate, 101), ProductName,	
  	[Product Number] = replace(p.ProductID, 'PDT', 'PR') , 
  	[Total Purchase Transaction] = count(pt.PurchasetransactionID)
  from Supplier s, PurchaseTransaction pt, Product p,
  	(select alias = sum(PurchaseTransactionQuantity) from PurchaseTransaction) as x
  where pt.SupplierID = s.SupplierID 
  	and p.ProductID = pt.ProductID
  	and PurchaseTransactionQuantity < x.alias 
  	and p.ProductID = 'PDT005'
  group by SupplierName, PurchaseTransactionDate, ProductName, p.ProductID
  order by SupplierName desc
  ```
  ![image](https://github.com/user-attachments/assets/9912665d-758d-4415-ac8f-8bd9e8aa2b50)

  
- Create  a  view  named  ‘ViewPurchaseTransaction’  to  display  EmployeeName, SupplierName,  Total  Purchase  Transaction  (obtained  from  the  count  of purchase transaction), and Maximum Purchase (obtained from the maximum of quantity) for every employee whose name contains ‘d’ character and the Total Purchase Transaction is greater than 1.
  ```
  create view ViewPurchaseTransaction as 
  select EmployeeName, SupplierName, [Total Purchase Transaction] = count(t.TreatmentID), 
  	[Maximum Purchase] = max(PurchaseTransactionQuantity)
  from Employee e
  	join ServiceTransaction st on st.EmployeeID = e.EmployeeID
  	join Treatment t on t.TreatmentID = st.TreatmentID
  	join PurchaseTransctionDetail ptd on ptd.EmployeeID = e.EmployeeID
  	join PurchaseTransaction pt on pt.PurchaseTransactionID = ptd.PurchaseTransactionID
  	join Supplier s on s.SupplierID = pt.SupplierID
  where EmployeeName like 'd%' or EmployeeName like '%d%' or EmployeeName like '%d'
  group by EmployeeName, SupplierName
  having count(t.TreatmentID) > 1
  ```
  ![image](https://github.com/user-attachments/assets/1b0ac502-994f-4c01-9bc8-e5782896f617)

- Create a view named ‘ViewEmployeeSalaryinRoomDetail’ to display EmployeeName. EmployeeSalary, ServiceTransactionID, Total Treatment Transaction (obtained from the count of treatment) for every transaction that happened in room ‘ROT001’ and average of employee salary is less than 4000000.
  ```
  create view ViewEmployeeSalaryinRoomDetail as 
  select EmployeeName, EmployeeSalary, ServiceTransactionID, [Total Treatment Transaction] = count(t.TreatmentID) 
  from Employee e
  	join ServiceTransaction st on e.EmployeeID = st.EmployeeID
  	join Treatment t on t.TreatmentID = st.TreatmentID
  where RoomThemeID = 'ROT001'
  group by EmployeeName, EmployeeSalary, ServiceTransactionID, t.TreatmentID
  having avg(EmployeeSalary) < 4000000
  ```
  ![image](https://github.com/user-attachments/assets/0a4adc9a-3d31-4645-a373-a29a76dc2313)
  
## CV
Link: [here](https://drive.google.com/file/d/1xZBB3X-Lh30Yw9mKAcJqkjlQJHtzz5mU/view?usp=sharing)

## Contacts
- LinkedIn: [Mohammad Rizki Riyadi](https://www.linkedin.com/in/mohammad-rizki-riyadi/)
- Email: rizkiriyadi76@gmail.com


