# Uber Trips Analysis - 2016 Dataset

## Project Overview
- Analyzed Uber trips from 2016 to uncover usage patterns, trip durations, and popular routes.  
- Objective: identify trends in trip purposes, distances, and round-trip behavior to optimize operations and understand customer behavior.  

## Dataset
- **My Uber Drives - 2016.csv**  
- Contains details of Uber trips including:
  - START_DATE, END_DATE  
  - START and STOP locations  
  - MILES (trip distance)  
  - CATEGORY (ride type)  
  - PURPOSE of trip  

## Data Preprocessing & Feature Engineering
- Standardized column names and removed special characters  
- Filled missing `PURPOSE` values using forward-fill  
- Converted `START_DATE` and `END_DATE` to datetime objects  
- Calculated trip duration in minutes (`MINUTES`)  
- Created a `ROUND_TRIP` feature to flag trips starting and ending at the same location  
- Extracted month from `START_DATE` for seasonal analysis  

## Exploratory Data Analysis
- Identified **top and least popular start and stop points**  
- Analyzed distribution of trip distances (`MILES`) and durations (`MINUTES`)  
- Visualized most common trip purposes and their relation to categories  
- Examined trips over months to identify **seasonal patterns**  
- Explored correlation between numerical features  

## Key Insights
- Most trips are single-direction; round trips are rare  
- Trip purpose significantly affects distance and duration  
- Certain start and stop locations are consistently more popular  
- Seasonal and monthly trends impact Uber usage patterns  

## How to Run the Repository
1. Clone the repository  

        git clone https://github.com/your-username/Uber-Trips-Analysis.git
        cd Uber-Trips-Analysis

2. Install required dependencies
   
        pip install pandas numpy matplotlib seaborn
3. Ensure `My Uber Drives - 2016.csv` is present in the project directory  
4. Launch Jupyter Notebook

        jupyter notebook
5. Run the notebook sequentially to reproduce EDA and feature analysis  

## Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  

## Conclusion
- The analysis provides insights into Uber trip patterns, popular routes, and trip purposes.  
- Data-driven insights can help optimize ride operations and improve customer experience.
