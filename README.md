# job_market_etl

### **Scraping Job Listings and Analysing Job Market Trends**

### **Overview:**

Create an ETL pipeline that scrapes job listings from websites like **Indeed**, **LinkedIn**, or **Glassdoor**. Collect data on job titles, companies, locations, salary ranges, and required skills. Analyse trends in the job market (e.g., most in-demand skills, average salaries for different positions) and store the data in a structured format.

### **Steps:**

1. **Data Collection and Exploration:**
    - Use the **Indeed API** if available if not use a web scraper such as **BeautifulSoup** or **Scrapy**.
    - Explore the data and decide what is relevant to the project
    - Store relavent data in a dataframe

2. **Data Transformation:**
    - Clean and transform the data using **pandas**:
        - Parse salary ranges (e.g., convert "50K-70K" to numeric ranges).
        - Extract keywords or required skills from the job descriptions and categorize them (e.g., using regex to identify programming languages like Python, JavaScript, etc.).
3. **Loading Data:**
    - Load the cleaned and transformed data into a **PostgreSQL** database.
    - Use **SQLAlchemy** or **pandas** to insert data into tables.
4. **Analysis:**
    - Perform basic trend analysis on job titles, salaries, and required skills over time.
    - For example, find out which skills are most in-demand or the average salary for specific job titles.
5. **Automation:**
    - Set up an **Airflow** pipeline to run the scraping job on a regular basis (e.g., every week) to keep the job market data updated.
6. **Visualization:**
    - Use **Matplotlib**, **Seaborn**, or **Plotly** to create visualizations of job market trends, such as the most in-demand skills or salary distributions for different job titles.

### **Skills Demonstrated:**

- Connecting to an API 
- Web scraping (Scrapy, BeautifulSoup)
- Data transformation (pandas)
- Databases (PostgreSQL)
- ETL automation (Airflow)
- Basic data analysis and trend identification
- Data visualization (Matplotlib, Seaborn, Plotly)