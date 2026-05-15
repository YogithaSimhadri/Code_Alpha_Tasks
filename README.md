# Task 2: Exploratory Data Analysis (EDA) - Flipkart Laptops

## 1. Core Questions Asked Before Analysis
* What is the overall price distribution of laptops listed on Flipkart?
* Which specific laptop models represent the extreme maximum and minimum price boundaries?
* Is there a correlation between higher prices and better user ratings?
* Are the price columns properly formatted as numerical fields for calculations?

## 2. Dataset Structure Summary
* **Total Records (Rows):** 624
* **Total Features (Columns):** 2

### Variable Definitions & Types:
* `Laptop_Name` -> Type: Categorical (Text String)
* `Selling_Price` -> Type: Numerical (Continuous Integer)
* `MRP` -> Type: Numerical (Continuous Integer)
* `Rating` -> Type: Numerical (Float / Decimal)

## 3. Structural Data Cleaning Observations
* **Issue:** Price columns originally contained the Indian Rupee symbol ('₹') and currency formatting commas (e.g., ₹62,990). This caused Excel/Google Sheets to read them as text strings instead of numbers.
* **Resolution:** Performed a global Find & Replace to strip the '₹' and ',' characters. This successfully converted the variables into clean numerical data types, enabling mathematical operations like `AVERAGE`, `MIN`, and `MAX`.
