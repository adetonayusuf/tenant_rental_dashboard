# tenant_rental_dashboard
Power BI Dashboard Analysis of Tenant Rent Performance/Activities

Business Overview/Problem
HomeVibe Properties has identified several pressing challenges related to tenant retention, presented in bullet points for clarity:

- High Tenant Churn Rates: The company faces elevated tenant turnover rates, resulting in increased operational costs and lost revenue. 
- Limited Tenant Insights: HomeVibe Properties lacks actionable insights into tenant satisfaction and their concerns, making it challenging to proactively address issues. 
- Inefficient Lease Renewals: The lease renewal process is plagued by inefficiencies, contributing to tenant dissatisfaction and administrative overhead. 
- Lack of Trend Identification: Identifying trends and patterns affecting tenant retention is difficult, hindering the development of effective retention strategies.

Rationale for the Project
The importance of tenant retention in the real estate and property management industry cannot be overstated. Here are the top five reasons highlighting the significance of this project:

- Enhanced Revenue: Improved tenant retention directly correlates with increased revenue and profitability as existing tenants renew their leases. 
- Positive Reputation: Elevated tenant satisfaction generates positive word-of-mouth, attracting new tenants and enhancing the company's brand image. 
- Operational Efficiency: Streamlining lease renewal processes reduces administrative overhead, allowing for better resource allocation. 
- Competitive Edge: Data-driven decision-making provides a competitive advantage in the highly competitive real estate market. 
- Sustainability: A focus on tenant retention aligns with sustainable business practices by reducing the environmental impact of turnover.

Aim of the Project

The primary objectives of this project are as follows:

- Interactive Tenant Retention Dashboard: Design and implement an interactive tenant retention dashboard using Power BI. 
- Data Analysis: Analyze historical tenant data to identify factors affecting tenant churn and provide actionable insights. 
- Lease Renewal Optimization: Streamline lease renewal processes to increase tenant retention rates.

Data Description

This case study contains 4 datasets and  they are as follows;

Tenant Information Dataset:

 - Tenant ID (N/A): A unique identifier for each tenant. 
 - Tenant Name (Text): The name of the tenant. 
 - Contact Details (Text - Phone number or email): Contact information for the tenant. 
 - Lease Start Date (Date): The date when the tenant's lease agreement started. 
 - Lease End Date (Date): The date when the tenant's lease agreement is scheduled to end. 

Lease Details Dataset:

 - Lease ID (N/A): A unique identifier for each lease. 
 - Lease Start Date (Date): The date when the lease agreement started. 
 - Lease End Date (Date): The date when the lease agreement is scheduled to end. 
 - Lease Term (Months) (Months): The duration of the lease in months. 
   Rent Amount (Currency - e.g., USD): The amount of rent for the lease. 
 - Payment History (Currency - e.g., USD): The total amount paid for the lease. 

Tenant Feedback Dataset:

 - Feedback ID (N/A): A unique identifier for each feedback entry. 
 - Tenant ID (Link to Tenant Information Dataset): Identifies the tenant associated with the feedback. 
 - Survey Response (Text): Text responses to survey questions, indicating tenant satisfaction. 
 - Comments (Text): Open-ended comments provided by tenants, offering additional feedback or details. 

Property Information Dataset:

 - Property ID (N/A): A unique identifier for each property. 
 - Property Name (Text): The name or title of the property. 
 - Location (Text - Address or coordinates): The location of the property. 
 - Property Type (Text): The type of property (e.g., Apartment, Single-family home). 
 - Amenities (Text): A list of amenities offered at the property. 
 - Historical Occupancy Rate (%) (Percentage): The historical occupancy rate of the property, expressed as a percentage.


Tech Stack

 Tool - Power BI
  It will be used for ;

 - Data Integration 
 - Data Transformation 
 - Data Analysis and Modeling 
 - Real-time Data Visualization 
 - Dashboard Design 
 - Reporting 
 - Cloud Integration

Project Scope

 - Exploratory Data Analysis: Explore the data to understand its characteristics and discover patterns. 
 - Data Transformation: Prepare the data for analysis by transforming, encoding, or normalizing it. 
 - Data Analysis: Analyze data to understand pattern in order to generate insights that will be visualized. 
 - Data Visualization: Create visual representations to communicate insights effectively. 
 - Interpretation and Insight Generation: Extract meaningful insights and interpret the results.

   Actions
- Imported the above tables into Power query no cleaning needed on any of the table.
- Merged tenant information & feedback to tenant feedback table to form tenant information & feedback table
- Merged lease details and tenant information & feedback to form lease details table.
- Load the tables into power Bi
  

  ![Tenant Power Query](https://github.com/adetonayusuf/tenant_rental_dashboard/blob/main/Tenant%20-%20Power%20query.png)
  
  
  - After importing the data into Power BI, I then created date tables
  - Modelled the tables using star schema
    

  ![Tenant Data Modelling](https://github.com/adetonayusuf/tenant_rental_dashboard/blob/main/Tenant%20Data%20Modelling.png)
  

  - Created some measures that will help with detailed analysis like churn rate, Total Payment Histoty, Churned Leases, Rent Collection Performance Etc
  - We created the dashboard below base on the analysis above
    
 
  ![Tenant Retention Dashboard](https://github.com/adetonayusuf/tenant_rental_dashboard/blob/main/Tenant%20Retention%20Dashboard.png)
  


    Insights
    
   - Seasonal and Trend-Based Churn Patterns: The line chart of churn rate by month reveal seasonal patterns or specific times of the year when churn rates
     spike, indicating periods where targeted retention efforts could be most benefcial

   - Lease Term Preferences and Their Impact on Retention: The frequency distribution of lease terms highlights tenant preferences, showing whether shorter or
     longer leases correlate with higher retention rates, suggesting adjustments to lease offerings.

   - Direct Correlation Between Tenant Satisfaction and Retention: Analysis from the bar chart showing satisfaction scores and the combo chart correlating
     churn status with satisfaction scores by property type provide concrete evidence that higher satisfaction levels are crucial for reducing churn rates

   - Financial Efficiency and Its Role in Overall Property Performance: Rent collection performance insights can highlight operational efficiencies or issues
     affecting the company's financial health and its ability to invest in property improvements and tenant services.

   - Effectiveness of Renewal Strategies Over Time: The comparison of renewed versus expired leases over time can indicate the success of recent retention
     strategies or highlight the need for new approaches.

    Recommendations
  
   - Implement Targeted Retention Programs: Based on identified churn patterns, develop targeted retention programs during high-risk perlods, such as
     personalized communication, special offers, or community events to engage tenants.
     
   - Adjust Lease Terms to Meet Tenant Preferences: If certain lease lengths correlate with higher retention, consider offering more fiexible or preferred lese
     terms to new and renewing tenants to encourage longer stays.
     
   - Enhance Tenant Satistaction: Prioritize improvements in areas directly impacting tenant satisfaction, as identified through survey responses. This could
     include property amenities, maintenance responsiveness, and community-building efforts.
     
   - Optimize Financial Operations. Address any identified inefficiencies in rent collection to improve financial stability. Consider implementing technology
     solutions for easier payment processes or offering incentives for on-time payments.
