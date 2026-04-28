Customer Shopping Behavior: End-to-End Data Pipeline & Analysis

📌 Project Overview
This project demonstrates a complete data engineering and analytics workflow. I transformed raw consumer data using Python, migrated it to a cloud-based PostgreSQL database (Neon), and performed deep SQL analysis to drive business insights. The final stage involved building an interactive dashboard in Power BI to visualize customer segments and purchasing patterns.

🛠️ Tech Stack
Language: Python 3.12 (Pandas, SQLAlchemy)

Database: PostgreSQL (Cloud-hosted via Neon.tech)

Analysis: SQL (Complex queries, CTEs, Window Functions)

Visualization: Power BI Desktop

Environment: Docker / Google Colab

🚀 Data Pipeline Workflow
1. Data Preprocessing (Python)
Cleaned and transformed the customer_shopping_behavior.csv dataset.

Handled missing values and optimized data types for SQL compatibility.

Established a secure connection to a cloud PostgreSQL instance using SQLAlchemy and Psycopg2.

2. Cloud Database Management (Neon)
Migrated the local dataframe to a Neon Cloud Database, bypassing local network restrictions and ensuring high availability.

Configured SSL-encrypted connections for secure data transit.

3. SQL Analysis
Executed business-critical queries directly in the cloud environment to answer key questions:

Revenue Analysis: Comparing total spend across genders and categories.

Customer Segmentation: Categorizing users as 'New', 'Returning', or 'Loyal' based on purchase history.

Performance Metrics: Identifying top-performing products and average review ratings.

Shipping Impact: Analyzing how different shipping methods (Express vs. Standard) correlate with purchase amounts.

4. Business Intelligence (Power BI)
Connected Power BI to the Neon Cloud PostgreSQL server.

Developed an interactive dashboard featuring:

Sales trends and category breakdowns.

Demographic insights.

Product performance rankings.

📈 Key Insights
Segment Performance: Identified which customer segment (Loyal vs. New) contributes most to the bottom line.

Product Trends: Determined the top 3 items in each category with the highest review ratings.

Shipping Influence: Found a correlation between shipping choice and total order value.

📂 Project Structure
Data_Analytics_Project.ipynb: Python notebook for data cleaning and DB upload.

Business_Questions.sql: A collection of SQL queries used for the analysis.

customer_shopping_behavior.csv: The raw dataset used for this project.

Customer_Behavior_Dashboard.pbix: The final Power BI dashboard file.

🛠️ How to Run
Database: Set up a free PostgreSQL instance on Neon.tech.

Environment: Update the connection string in the Python notebook with your Neon credentials.

Execute: Run the cells in .ipynb to clean and push the data.

Visualize: Open the .pbix file in Power BI and update the data source to your cloud server.
