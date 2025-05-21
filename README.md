# e2ERail_Data_Analysis_Task

Dataset - inventory and sales data

Task: data analysis, visualization, and reporting

Given Data features:
Product_ID	
Product_Name	
Catagory	
Supplier_ID	
Supplier_Name	
Stock_Quantity	
Reorder_Level	
Reorder_Quantity	
Unit_Price	
Date_Received	
Last_Order_Date	
Expiration_Date	
Warehouse_Location	
Sales_Volume	
Inventory_Turnover_Rate	
Status
TOTAL FEATURE : 15 columns 

Data cleaning and preparation
1)checking duplicates, null, blank, type of each column
2)classify numeric and non-numeric features
3)Understand which feature is needed for analysis, remove unnecessary columns, extract new columns.



CATEGORY FEATURE : 
1)Product_Name
2)Catagory
3)Supplier_Name
4)status
5)new column : Inventory_Performance_Category
6)new column : Inventory_Risk_Assessment 
7)new column : Shelf Life Status 
8)Warehouse_Location -- not needed (unique values)


NUMERICAL FEATURE:
1)Stock_Quantity
2)Reorder_Level	
3)Reorder_Quantity	
4)Unit_Price 
5)Sales_Volume
6)new column : Shelf life (expiration date - date received) there are many values coming under negative ,some expiration date is before date received for each product
8)Inventory_Turnover_Rate -- not needed	(used as extracting feature)
9)Product_ID -- not needed (unique values)
10)Supplier_ID -- not needed unique value (when we used as extracting feature) Supplier_ID : 38-037-1699 
can take Region code (38) as region category

--> we can get 38 but without confirmation of what 38 means, we can't use this. There 100 unique value but when we filter from supplier name,it is 350 unique value, logically we can't use this feature


DATE FEATURE:
1)Date_Received	
2)Last_Order_Date	
3)Expiration_Date	


Turnover Rate Inventory_Performance_Category Inventory_Risk_Assessment 
1–29	      Slow-moving stock	               risk of expiry
30–80	      Healthy movement	               ideal range
80–100	      Fast-moving stock	               watch for stockouts

New data ,
Numerical features -
stock quantity,re-order level,re-order quantity,unit price,sales volume 
Categorical features -
Product name,product category,supplier name,inventory performance category,investment risk assessment category,status,shelf life status,Predicted_Status,Status 
Date features- 
Date received,expiration date, last order date 

Did Analysis in these areas:

Overstocking,bought too much

Low demand,customers don’t want it

Old/outdated items based on expiration date

It ties up our money,cash stuck in stock

We may need storage space or pay warehousing costs.

Risk of damage, expiry

If we’re not careful, customers may go to competitors.


