🚗 Cars Data Analysis using Pandas
📌 Project Overview

This project focuses on analyzing a dataset of cars and their specifications using Python and Pandas. The dataset is provided in CSV format and includes details such as make, origin, price, weight, and fuel efficiency.
The main objective is to perform data cleaning, exploration, and transformation to extract meaningful insights.

📂 Dataset
The dataset contains information about different cars.
Features include:
Make
Origin
MSRP (price)
Invoice
Weight
MPG (City/Highway)

⚙️ Technologies Used
Python 🐍
Pandas 📊
Jupyter Notebook 📓

🔍 Tasks Performed
1. Data Loading
Imported dataset using Pandas
pd.read_csv()

2. Data Exploration
Viewed dataset using:
.head()
.shape()

3. Data Cleaning
Checked for missing values:
car.isnull().sum()
Filled missing values with column mean
Converted price columns (MSRP, Invoice) from string to numeric

4. Data Analysis
✅ Value Counts
Counted number of cars by manufacturer:
car['Make'].value_counts()

✅ Filtering Data
Selected cars from Asia and Europe:
car[car['Origin'].isin(['Asia','Europe'])]

✅ Removing Unwanted Records
Removed cars with weight above 4000:
car[~(car['Weight'] > 4000)]

✅ Applying Functions
Increased city mileage (MPG_City) by 3:
car['MPG_City'] = car['MPG_City'].apply(lambda x: x + 3)

📊 Key Insights
Identified distribution of car manufacturers
Cleaned inconsistent price data
Filtered dataset based on region and weight
Modified mileage values for analysis

📁 Project Structure
├── Cars.ipynb
├── README.md
└── dataset.csv

✨ Future Improvements
Add visualizations using Matplotlib/Seaborn
Perform advanced statistical analysis

📝 Conclusion
This project demonstrates effective data cleaning and analysis techniques using Pandas on a real-world dataset.
It highlights how structured data processing can uncover meaningful insights for better decision-making.
