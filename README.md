# HR Analytics Dashboard | Power BI

## Project Overview

This project is an interactive HR Analytics Dashboard built using Power BI. The dashboard provides insights into employee performance, salary distribution, department-wise analysis, and workforce metrics. It helps management understand employee trends and make data-driven decisions.

---

## Objectives

* Analyze employee salary and performance data.
* Identify top-performing employees.
* Compare department-wise salary and rating metrics.
* Track workforce distribution across departments.
* Generate actionable business insights and recommendations.

---

## Tools & Technologies

* Power BI Desktop
* DAX (Data Analysis Expressions)
* Microsoft Excel
* Data Visualization

---

## Dataset Information

The dataset contains employee-related information including:

* Employee ID
* Employee Name
* Department
* Salary
* Performance Rating

---

## Key Performance Indicators (KPIs)

The dashboard includes the following KPIs:

* Total Employees
* Average Salary
* Average Rating
* Highest Salary
* Excellent Employees Count

---

## Dashboard Features

## HR Analytics Dashboard

![Dashboard](HR%20Analytics%20Dashboard/dashboard_screenshot.png)

### Employee Analysis

* Total employee count
* Department-wise employee distribution

### Salary Analysis

* Average salary by department
* Highest salary identification

### Performance Analysis

* Average rating by department
* Employee performance classification
* Top performer identification

### Advanced Visualizations

* Performance distribution chart
* Employee salary vs performance rating scatter plot
* Interactive department slicer

---

## DAX Measures Used

### Total Employees

```DAX
Total Employees =
COUNT(HR_Analytics[EmployeeID])
```

### Average Salary

```DAX
Average Salary =
AVERAGE(HR_Analytics[Salary])
```

### Average Rating

```DAX
Average Rating =
AVERAGE(HR_Analytics[Rating])
```

### Highest Salary

```DAX
Highest Salary =
MAX(HR_Analytics[Salary])
```

### Excellent Employees

```DAX
Excellent Employees =
CALCULATE(
    COUNTROWS(HR_Analytics),
    HR_Analytics[Rating] >= 4.5
)
```

---

## Calculated Columns

### Bonus

```DAX
Bonus =
HR_Analytics[Salary] * 0.10
```

### Performance Category

```DAX
Performance =
IF(
    HR_Analytics[Rating] >= 4.5,
    "Excellent",
    "Good"
)
```

---

## Key Insights

* IT department has the highest average salary.
* HR and IT departments have the highest employee count.
* Employee F is identified as the top performer.
* Only 2 employees are classified as Excellent performers.

---

## Business Recommendations

* Review HR compensation structure to improve retention.
* Recognize and reward high-performing employees.
* Analyze successful practices in the IT department and apply them across other departments.
* Develop performance improvement plans for lower-performing employees.

---

## Project Outcome

The dashboard successfully transforms raw employee data into meaningful insights using Power BI and DAX. It demonstrates data visualization, KPI development, business analysis, and dashboard design skills relevant to Data Analyst roles.

---

## Author

**Animesh Tiwari**

Aspiring Data Analyst | SQL | Python | Power BI | Excel
