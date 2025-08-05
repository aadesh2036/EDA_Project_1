# EDA_Project_1
A data analysis project on the Netflix dataset, demonstrating data cleaning, preprocessing, and visualization techniques with Pandas and Seaborn to uncover content trends.
# Exploratory Data Analysis of Netflix Content

## 🚀 Objective
This project is an Exploratory Data Analysis (EDA) of the Netflix Movies and TV Shows dataset. The primary objective was to practice and demonstrate the full data analysis workflow: from loading and cleaning a raw dataset to answering specific questions with data manipulation and creating insightful visualizations. The project utilizes key Python libraries including Pandas for data wrangling, and Matplotlib/Seaborn for plotting.

## 📊 Dataset
The dataset used for this analysis is the "Netflix Movies and TV Shows" collection, publicly available on Kaggle. It contains information about titles available on Netflix up to 2021.
* **Source:** [Kaggle - Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)

## 🛠️ Analysis Workflow
The analysis followed a structured, multi-step process:
1.  **Data Loading and Inspection:** The raw `.csv` file was loaded into a Pandas DataFrame. Initial inspection was performed using `.head()`, `.info()`, and `.describe()` to understand the data's structure, identify data types, and locate missing values.
2.  **Data Cleaning and Preprocessing:** Missing values were handled strategically. Rows with a small number of nulls in important columns were dropped, while columns with many nulls (like `director`, `cast`) were filled with a placeholder ("Unknown") to preserve data integrity.
3.  **Question-Driven Analysis & Visualization:** Specific questions were formulated to guide the analysis. Pandas was used to filter, group, and aggregate the data to answer these questions, and the findings were visualized using Seaborn and Matplotlib.

## 📈 Key Findings & Visualizations

### 1. What is the breakdown of content on Netflix?
The analysis shows that Netflix has a significantly larger library of Movies compared to TV Shows, with movies making up nearly 70% of the content in this dataset.

`![Content Breakdown Chart](<img width="767" height="599" alt="Screenshot 2025-08-06 001245" src="https://github.com/user-attachments/assets/504beb7b-65cb-477f-93da-b3075e7cd561" />)
`

### 2. Who are the top 5 most common actors on Netflix?
By processing the multi-valued `cast` column, the analysis identified the actors with the most appearances. This required splitting the string of cast members, handling nulls, and aggregating the counts for each individual actor.

`![Top 5 Actors Chart](<img width="995" height="581" alt="Screenshot 2025-08-06 001238" src="https://github.com/user-attachments/assets/b1656ee9-1d01-4cec-80b7-00313dd6b163" />
)`

### 3. Which countries produce the most content?
The analysis of the `country` column, which often contains multiple countries for a single title, revealed the top 10 content-producing nations. The United States is the largest producer by a wide margin, followed by India.

`![Top 10 Countries Chart](<img width="1137" height="737" alt="Screenshot 2025-08-06 001226" src="https://github.com/user-attachments/assets/59c5b658-cb37-48d9-9a6e-58f67d7cbdfe" />)
`

## 💻 Technology Stack
* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn

## 🚀 How to Run
1.  Clone this repository.
2.  Ensure you have all the libraries from the Technology Stack installed (`pip install pandas numpy matplotlib seaborn jupyter`).
3.  Place the `netflix_titles.csv` file in the root directory.
4.  Launch Jupyter Notebook and open the `netflix_analysis.ipynb` file.
