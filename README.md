# Customer-Analysis-for-Bliss-Shopping-Mall.
## 1.	Project Overview
Shopping malls serve as central hubs for retail and entertainment, attracting diverse customers with varying purchasing behaviors, preferences, and spending habits. In an increasingly data-driven business landscape, malls must leverage analytical tools to optimize customer experience, improve revenue streams, and enhance overall operational efficiency.
## 2. Project Description
Comprehensive customer analysis: revenue, demographics, payment preferences, and mall traffic insights via interactive Excel dashboard for data-driven decision-making. 
By analyzing this data, I will help Bliss Shopping Mall visualize key metrics and enable strategic decisions for its board meeting. 
Stakeholders: Board of Directors
Project Timeline: One Week
## 3. Date used
- <a href="https://github.com/thekelvini/Customer-Analysis-for-Bliss-Shopping-Mall./blob/main/Dataset_Shopping%20Mall.xlsx"> Dataset Shopping Mall</a>
- <a href="https://github.com/thekelvini/Customer-Analysis-for-Bliss-Shopping-Mall./blob/main/Dataset_Shopping%20Mall.xlsx"> Dashboard Shopping Mall</a>
## 4. BUSINESS PROBLEM 
Bliss Shopping Mall, a prominent retail center, is looking to harness data insights to refine its business strategy and maximize profitability. By analyzing key aspects such as revenue trends, customer demographics, payment preferences, and foot traffic patterns, the mall's management can make informed decisions that drive growth and improve customer satisfaction.
This project involves developing an interactive Excel dashboard to provide a comprehensive customer analysis. The dashboard will present visualized insights into:
- Revenue Performance – Identifying trends in sales and profitability across different timeframes.
- Demographics – Understanding customer profiles based on age, gender, and other key characteristics.
- Payment Preferences – Analyzing transaction data to determine preferred payment methods.
- Mall Traffic Insights – Assessing peak shopping hours, foot traffic trends, and customer movement patterns.
  
The insights generated from this analysis will be instrumental in guiding strategic decision-making during the Bliss Shopping Mall board meeting. By leveraging this data, the management team can enhance marketing strategies, improve tenant selection, optimize mall layout, and implement customer-centric initiatives to drive sustainable growth.

### Key Result
Below are the Key Result Areas (KRA) the Board will focus on. The dashboard clearly and effectively answers these areas:
**Session A:** 
These are to be displayed as a single virtual on your dashboard
1.	**Customer Base Volume:** Quantify the aggregate count of unique customers captured within the dataset.
2.	**Cumulative Revenue Generated:** Compute the comprehensive sum of revenue accrued from all transactions.
3.	**Total Units Purchased:** Determine the consolidated volume of products ordered across all customer orders.
**Session B:**
1.	**Revenue Contribution by Age Demographic:** Quantify the proportional revenue impact (%) of each defined age cohort relative to total revenue.
2.	**Gender-Based Revenue Distribution:** Analyze the percentage share of total revenue attributable to each gender (Female/Male).
3.	**Gender-Specific Customer Segmentation:** Calculate the total number of distinct customers categorized by gender.
4.	**Prevalent Payment Method Identification:** Determine the payment method with the highest frequency of usage.
5.	**High-Traffic Mall Assessment:** Identify the shopping mall with the greatest volume of customer visits.
6.	**Age Cohort Payment Preferences:** Evaluate the predominant payment method adopted by customers within each age category.

## 5.	DATA COLLECTION 
Data was extracted from the Bliss analysis database using SQL. It was then loaded into Excel, and data cleaning and transformation were done to prepare it for exploratory analysis. 
- Dataset Name: Bliss Shopping Mall Dataset
- Source: Bliss Shopping Mall Dataset internal database system.
- Data Extraction Methods: Data was extracted using SQL. I connected to the bliss database through Excel “Get Data”. 
- Size: The number of rows is 99457 using =COUNTA(A2:A99458), The number of columns is 13 using =COUNTA(A2:K2) and file size]
- Format: The file format, is CSV.
- Data Dictionary: The columns in the data set include Invoice number, Customer_ID, Gender, Age, Category, Quantity, Price, Payment Method, and shopping mall.

## 6.	DATA CLEANING AND PREPARATION
- Data Preprocessing Steps: Create a table for the dataset
- Remove duplicate: There was no duplicate in the datasets.
- Handling missing values: there are no missing values in the dataset
- I use =PRODUCT(G2*H2) to generate the revenue column
- I use =IF(OR(C3="F", C3="Female"), "Female", IF(OR(C3="M", C3="Male"), "Male", "Invalid")) to standardize the gender.
- Age category was used standardize =IF([@Age]<=25, "Young Adult", IF([@Age]<=33, "Adult", IF([@Age]<=41, "Senior", IF([@Age]>=42, "Elderly"))))
- Data transformation: Data was transformed to a pivot table for analysis 
- Tools Used: SQL was used for data extraction, while Excel was used for visualization.

![Screenshot 2025-02-20 121315](https://github.com/user-attachments/assets/fe300d7f-4579-43ec-87d6-16cd97d3afd7)
![Screenshot 2025-02-20 121944](https://github.com/user-attachments/assets/57fd6391-d292-4c43-9be0-51fe3b80f105)

