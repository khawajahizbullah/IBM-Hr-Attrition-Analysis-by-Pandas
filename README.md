# 📊 HR Analytics Project (IBM Attrition Data + Department Budget)

## 📌 Project Overview
This project explores the **IBM HR Employee Attrition dataset** and a **synthetic Department Budget dataset** to perform HR analytics using the Pandas library in Python.  
The main goal is to **analyze employee attrition, salary spend, and compare actual vs allocated department budgets**.

---

## 🎯 Project Goals
- Explore and clean HR employee data.
- Handle missing values appropriately.
- Perform data transformations such as filtering and salary updates.
- Analyze attrition patterns across departments.
- Compare **department salary spend vs budget allocation**.

---

## 🛠️ Pandas Features Demonstrated
This project highlights essential Pandas functions and workflows:

- **Exploration**
  - `.head()`, `.tail()`, `.describe()`, `.info()`, `.isnull().sum()`

- **Handling Missing Data**
  - `.fillna()` for categorical values
  - `.interpolate()` for numeric values
  - `.dropna()` where needed

- **Updating & Filtering**
  - Filtering all `Attrition == 'Yes'` entries
  - Applying a **performance-based salary increment of 5%**

- **Sorting**
  - Sort by `YearsAtCompany` ascending
  - Then by `MonthlyIncome` descending

- **Aggregation & Grouping**
  - Group by `Department` and calculate:
    1. Average **MonthlyIncome**
    2. Median **Age**
    3. Sum of **Attrition == 'Yes'** (employees who left)

- **Merging & Joining**
  - Created a synthetic **DepartmentBudget.csv**
  - Merged with HR salary spend to compare **budget vs actual spend**
  - Added a column `Budget_Status` → `"Under Budget"` or `"Over Budget"`

---

## 📈 Key Insights
- The **Sales department** had the **highest attrition rate**, suggesting possible employee dissatisfaction or work pressure.  
- **Research & Development (R&D)** went **over budget**, with salary expenses exceeding the allocated budget.  
- The **HR department** remained within budget but had lower average income compared to other departments.  
- Employees with **fewer years at the company sometimes earned higher salaries**, possibly due to performance-based increments.  
- A **5% salary increase for high performers** raised overall salary distribution but did not significantly change attrition trends.  
- Median age analysis showed that departments with younger employees had **slightly higher attrition** compared to older workforce groups.  



