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

## 7.	DATA ANALYSIS 
- Exploratory Data Analysis (EDA)
Before we start digging into all the details, it’s crucial to do exploratory data analysis (EDA) on the Bliss Shopping Mall dataset. EDA means we’ll take a good look at the data to understand its main characteristics. We’ll do this by summarizing how the data behaves and by making pictures that show us any important trends. This first look helps us see how the data is organized and what’s in it, So, we can find deeper insight later.
- Dashboard Summary
  
![Screenshot 2025-02-19 203524](https://github.com/user-attachments/assets/d28997d9-9688-4cde-81fe-ffcda59bf24f)

### Key Performance Indicators (KPIs)
KPIs were added to tell us how well Bliss Shopping Mall is doing. In our analysis of Bliss Shopping Mall performance based on key metrics:
### Total Customer: Bliss Shopping Mall serves a customer base of approximately 99,457 people.
### Revenue: The company has achieved a revenue of N 251,505,794,25.
### Total Orders: The total number of orders processed amounts to 28,000.
### Number of Malls: Orders were placed from 10 different malls.

###  Customer Analysis Report
From the dashboard above the gender distribution among Bliss Shopping Customers is as follows;
- Males: Represent 40% of the total customer base, with a count of 39,975.
- Females: Represent 60% of the total customer base, with a count of 59,482.
This information suggests that a majority of customers are female. This demographic insight could be valuable for tailoring marketing strategies, product development, and customer engagement efforts to better suit customer base.
 
From the dashboard above the revenue distribution between male and female customers is as follows;
- Males:
- Generated revenue: $101,298.65
- Females:
- Generated revenue: $150,207,136.02
From this chart, it’s clear that females generated significantly more revenue than males. This information can be crucial for understanding the customer base and can help in making data-driven decisions for future business strategies.
 
From the dashboard above the number of customers in four different age groups: Elders, Seniors, Young Adults, and Adults. Here’s a breakdown of the data:
- Elders: 53,275 customers (tall blue bar)
- Seniors: 15,488 customers (shorter green bar)
- Young Adults: 15,359 customers (shorter dark blue bar)
- Adults: 15,335 customers (shorter yellow bar)
Key Insights:
- The Elders age group has the highest number of customers, significantly more than the other groups.
- The number of customers in the Seniors, Young Adults, and Adults groups are relatively similar, with only slight variations between them.
This distribution suggests that the majority of customers are Elders. It might be beneficial to explore why this age group is the largest and consider tailoring your marketing strategies and services to better cater to their needs.

From the dashboard above the revenue contributions from different age groups. Here's the detailed breakdown:
- Elders: $135,373,070.43
- Senior: $39,623,760.76
- Adult: $38,390,691.71
- Young Adult: $38,118,271.35
Key Insights:
- The Elders age group has the highest revenue contribution, significantly more than the other age groups.
- The contributions from Seniors, Adults, and Young Adults are relatively similar, with only slight variations between them.
This distribution indicates that the Elders age group is not only the largest in terms of customer numbers but also the most significant in terms of revenue generation. This could be an opportunity to further tailor Bliss Shopping Mall's marketing and service offerings to meet the preferences and needs of this age group.

From the dashboard above the number of visitors at various malls. Here's the detailed breakdown:
- Mall of Istanbul: 19,943 visitors
- Kanyon: 19,823 visitors
- Metrocity: 15,011 visitors
- Metropol AVM: 10,161 visitors
- Istinye Park: 9,781 visitors
- Zorlu Center: 5,075 visitors
- Cevahir AVM: 4,991 visitors
- Forum Istanbul: 4,947 visitors
- Viaport Outlet: 4,914 visitors
- Emaar Square Mall: 4,811 visitors

Key Insights:
- Mall of Istanbul and Kanyon are the most visited malls, with visitor numbers close to each other.
- There is a noticeable drop in the number of visitors after the top three malls (Mall of Istanbul, Kanyon, and Metrocity).
- Emaar Square Mall has the least number of visitors among the listed malls.
This data can be valuable for understanding which malls are the most popular and potentially why they attract more visitors. It could also guide decisions related to retail space, advertising, and customer engagement efforts.

## 8.	KEY FINDINGS AND INSIGHTS
### Customer Demographics:  The majority of customers are female (60%). Elders form the largest age group, and they contribute the highest revenue.
### Revenue Insights: Elders generate more than half of the total revenue, making them a crucial demographic for the mall.
### Mall Visits: The Mall of Istanbul and Kanyon are the most popular shopping destinations, indicating high foot traffic and customer preference.
### Payment Preferences: A significant portion of transactions is conducted in cash, which might indicate a need for better card or digital payment options.


## 9.	RECOMMENDATIONS 
### Targeted Marketing Strategies
- Since elders form the largest age group and generate the highest revenue, Bliss Shopping Mall should design age-appropriate promotions, loyalty programs, and discounts to encourage repeat visits.
- As 60% of customers are female, marketing campaigns should be tailored towards products, services, and experiences that appeal to women.
### Optimizing Store Locations and Partnerships
- The Mall of Istanbul and Kanyon have the highest foot traffic, indicating that opening more stores or investing in premium retail spaces in these locations could maximize revenue.
- Partnering with high-performing retailers in these malls can further enhance sales opportunities.
### Enhancing Customer Experience
- Since many transactions are conducted in cash, introducing better card and digital payment options (e.g., mobile wallets, contactless payments) can improve convenience and increase purchase frequency.
- Educating customers about digital payment security and offering incentives for card usage can encourage adoption.

### Revenue Growth Opportunities
- Understanding that elders drive the highest revenue, the mall could introduce specialized services such as senior-friendly amenities, personalized shopping assistance, and exclusive senior discounts to retain and grow this customer segment.
- Expanding product offerings catering to elder needs, such as health and wellness stores, would enhance shopping appeal.
### Strategic Resource Allocation
- Marketing budgets should be directed more towards high-traffic locations and demographics contributing the most revenue, ensuring a higher return on investment (ROI).
- Improving foot traffic in underperforming malls through promotional events, seasonal campaigns, and exclusive deals can balance revenue streams.
