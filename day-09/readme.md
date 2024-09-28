# Today's Learnings
***How Data Gathering is performed and how to understand the data?***
*Also provided the jupyter notebook for hands-on implementation*

## Data Gathering
There are many types/formats in which data is stored and shared. But at large scale very few methods are used which are
  - **CSV files**
      - Can be found on kaggle, github, etc.
      - Accessed through pandas, pd.read_csv()
  - **JSON / SQL format data**
      - From urls, databses
      - For SQL, sql_connector is used
      - pd.read_json()
  - **API fetched data**
      - from urls, etc.
      - real-time data fetching.
      - various techniques are used according to requirements.
  - **Web Scrapping**
      - from website's code using developers tools.
      - mainly used for search-based data fetching.
   
  ## Understanding the Data
  To understand the data, we should know the answer for the following questions related to given data.
  - *How much big it is ?*
      - size of the data
  - *How does it look like ?*
      - feature counts
      - datatypes of features
  - *Does it contains missing values ?*
  - *Duplicate values check ?*
  - *Mathematical relation ?*
      - find correlation between columns
   
  After performing this steps we perform **Exploratory Data Analysis** on provided dataset.
  ### Exploratory Data Analysis
  #### Univariate Analysis
  - Individually analysing each column.
  - Use seaborn, matplotlib, etc. libraries to draw visualisations for the analysis.
    - PieCharts, Bar graph for categorical data.
    - Histogram, Distplot, BoxPlot for numerical data.

  #### Multivariate Analysis
  - Variable combinations
      - **Numerical - Numerical:** Scatterplot
      - **Numerical - Categorical:** Distplot
      - **Categorical - Categorical:** ClusterMap


  After performing all these steps at last you can generate a report using pandas profiling, which generates an detailed report of performed EDA on dataset.
  - *PS:I've provided a report for my dataset*
