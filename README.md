## Project Objective
Analyze **Shield Insurance** company's data and create a dashboard comprising General view, Sales Mode, and Age Group views covering the following requirements

**General View:**

1. Focus on understanding the number of customers and the total revenue generated
2. Track the MoM revenue growth rate and customer growth rate to monitor progress
3. Analyze revenue by city and age group
4. Analyze customers by city and age group

**Sales Mode:**

1. Calculate total customers' split percentages by sales mode
2. Calculate total revenue split percentages by sales mode
3. Analyze the trend of sales mode over the month

**Age Group:**

Analyze age group data to understand the impact on our business.

1. Analyze age group data to understand expected settlement, sales mode, and policy preference

### Data overview
1. dim_customer.csv: Contains all customer information
2. dim_date.csv: Holds dates at daily, monthly levels, and week numbers of the year
3. dim_policies.csv: Encompasses all policy data
4. fact_premiums.csv: Includes information about policy orders
5. fact_settlements.csv: Contains details about policy settlements




### Approach
Imported datasets to Power BI and built a dashboard. Constructed a Star-schema data model.

I've created 3 pages: General View, Sales Mode, and Age Group and they have:

**General View:**
1. Four key metrics: Total customers, Total Revenue, Average daily revenue growth, and Average daily customer growth for the selected month. When selecting November, KPI shows blank for targets because we don't have data before November, and the message displayed is "Last month values are not available for the selected filter
2. Customer growth and revenue growth trend by months with a toggle to switch between the two
3. Revenue is split by city and age group
4. Customer segmentation by city and age group

**Sales Mode View:**
1. Customers % by sales mode
2. Revenue % by sales mode
3. Revenue % & customers % for sales mode by months with a toggle to switch between the two

**Age Group View:**
1. Customers by age group
2. Customers by age group vs sale Mode
3. Expected settlement by age group
4. Customers by age group Vs policy


+ To interact with [Live dashboard](https://app.powerbi.com/view?r=eyJrIjoiNWRhMWYyNmItOGIwMy00ZTEyLTlkOGMtNzJlMDBkMWRkYjcwIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9).
+ [Presentation Link](https://www.linkedin.com/feed/update/urn:li:activity:7155392298116096001/).

### Insights
March reports the highest customer growth and revenue growth.

Considering all the months:
1. **Delhi NCR** reports the highest number of customers with 11,007 and generated revenue of 401.57M, followed by **Mumbai** with 6,432 customers and 239.51M revenue
2. Age group **31-40** reports the highest number of customers with 11,415 and generated revenue of 354.44M, followed by **41-50** with 4,737 customers and 196.59M revenue
3. Out of all the modes (Offline Agent, Offline Direct, Online App, Online Website), customers prefer to purchase policies from **Offline Agents**, resulting in the highest revenue generated through Offline Agents for the Company
4. Since **Feb 23**, customers approaching **Online Apps** are in second place, followed by **Online websites.** So, Shield Insurance should focus on promoting their online apps and websites, considering the current trend towards online services
5. Here is the table that shows policy preference by **age group**
   
    | Age Group   | Policy      | 
    | ----------- | ----------- |
    | 18-24       | POL4321HEL  |
    | 25-30       | POL4321HEL  |
    | 31-40       | POL3309HEL  |
    | 41-50       | POL6303HEL  |
    | 51-65       | POL9221HEL  |
    | 65+         | POL2005HEL  |
