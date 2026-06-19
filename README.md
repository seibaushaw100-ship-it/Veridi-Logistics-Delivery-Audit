\# Veridi Logistics Delivery Performance Audit

## A. Executive Summary

This project analyzed delivery performance using the Olist Brazilian E-Commerce dataset to investigate whether delayed deliveries were contributing to negative customer reviews. The analysis revealed that Veridi Logistics achieved an on-time delivery rate of 92.3%, while 7.7% of orders were delivered late. Certain product categories and customer states experienced significantly higher late-delivery rates than others. Furthermore, customer satisfaction was strongly affected by delivery performance, with late and undelivered orders receiving substantially lower review scores. These findings suggest that targeted improvements in specific regions and product categories can improve operational efficiency and customer experience.

## B. Project Links

### Notebook Link

https://colab.research.google.com/drive/1cPKoGzyP1jj7Xv-fgzj6BEn2DB6XOBYc?usp=sharing

### Dashboard Link

The Power BI dashboard was developed using Power BI Desktop. Due to Power BI online publishing requirements, the dashboard is provided through the included .pbix file and dashboard screenshot contained in this repository.

### Presentation Link

https://drive.google.com/file/d/1FKHvQAQ0rt6\_NZ6KZ57gZ3-OkG5eYUJG/view?usp=sharing

### Dashboard Screenshot



\#C. Technical Explanation

### Data Cleaning

The project utilized the Olist Brazilian E-Commerce Dataset obtained from Kaggle. Multiple relational tables were integrated, including:
•	olist\_orders\_dataset.csv
•	olist\_order\_reviews\_dataset.csv
•	olist\_customers\_dataset.csv
•	olist\_products\_dataset.csv
•	product\_category\_name\_translation.csv
The datasets were merged using common keys such as order\_id and customer\_id. Duplicate records were checked, missing values were handled appropriately, and date columns were converted to datetime format to support delivery performance calculations. Product categories were translated from Portuguese to English using the provided translation dataset.

### Feature Engineering

Several business-focused features were created, including:
•	Days\_Difference
•	Delivery\_Status
•	Late\_Flag
•	Late Delivery Rate
•	On-Time Delivery Rate
Orders were classified into On Time, Late, Super Late, and Not Delivered categories to support performance analysis.

### Candidate’s Choice Challenge

An additional analysis titled "Orders by Delivery Status" was added to the dashboard. This feature helps management quickly understand the volume of orders that are delivered on time, delivered late, super late, or not delivered. It provides a clearer picture of operational performance and allows decision-makers to monitor service quality beyond the standard KPI metrics.

## Key Findings

•	Total Orders Processed: 99,441
•	On-Time Delivery Rate: 92.3%
•	Late Delivery Rate: 7.7%
•	Average Review Score: 4.02

## Dashboard Overview

The Power BI dashboard includes:
	Total Orders KPI
	On-Time Delivery Rate KPI
	Late Delivery Rate KPI
	Average Review Score KPI
	Top 5 Product Categories by Late Delivery Rate
	Top States by Late Delivery Rate
	Review Score by Delivery Status
	Orders by Delivery Status
	State Filter Slicer

## Geographic Analysis

Several customer states experienced disproportionately high late-delivery rates, indicating regional logistics challenges that require further investigation.
Product Category Analysis
Home Comfort, Furniture \& Mattress, and Audio product categories recorded some of the highest late-delivery rates, suggesting the need for improved inventory handling and transportation planning.

## Customer Satisfaction Analysis

Average review scores varied significantly across delivery statuses:
•	On Time: 4.21
•	Late: 3.41
•	Super Late: 1.78
•	Not Delivered: 1.74
These results demonstrate a strong relationship between delivery performance and customer satisfaction.

## Tools Used

•	Python (Pandas, NumPy, Matplotlib, Seaborn)
•	Google Colab
•	Power BI (DAX)
•	GitHub

## Repository Contents

• Veridi\_Logistics\_Notebook.ipynb
• Veridi\_Logistics\_Notebook.html (or PDF)
• Veridi\_Logistics\_Dashboard.pbix
• Dashboard\_Screenshot.png
• Veridi\_Logistics\_Presentation.pdf
• README.md

## Recommendations

1. Improve logistics planning for product categories with high late-delivery rates.
2. Investigate delivery bottlenecks in underperforming states.
3. Enhance delivery monitoring and tracking systems.
4. Reduce delivery delays to improve customer satisfaction.
5. Continue monitoring logistics performance using the Power BI dashboard.

\## Conclusion
The analysis demonstrates that delivery performance is a significant driver of customer satisfaction. While Veridi Logistics maintains a strong overall on-time delivery rate, targeted interventions in specific product categories and regions can further reduce delays and improve the customer experience. The developed dashboard provides a practical decision-support tool for monitoring logistics performance and supporting continuous improvement initiatives.

