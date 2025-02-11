# SUPERSTORE-REPORT
SUPERSTORE POWERBI REPORT
### *Final Project Report: Power BI Sales Analysis*  

#### *1. Importing the Excel File*  
The Superstore dataset was imported from an Excel file stored on the local system. The dataset contained three tables:  
- *Orders*: Main transaction data  
- *Returns*: Details of returned orders  
- *Users*: Manager details per region  

---

#### *2. Data Cleaning and Transformation*  
Data transformation was performed in Power Query Editor to ensure accuracy and usability. The following steps were taken:  
- Removed *Column 26* and *Column 27* as they were completely empty and unnecessary.  
- Changed data types for better analysis:  
  - Order Date and Ship Date were converted to *Date format*.  
  - Profit, Sales, and Discount were converted to *Number format*.  
- The *Product Base Margin* column had *1% missing values*, which were replaced with the column average.  

---

#### *3. Creating Relationships Between Tables*  
To link the tables effectively, the following relationships were established:  
- *Orders Table → Returns Table: Since Order ID had duplicate values in the Orders table, a **Bridge Table (ID Bridge)* was created to resolve the many-to-many relationship.  
- *Orders Table → Users Table: A relationship was created using the **Region column*.  

---

#### *4. Visualizations Created*  
Multiple charts and visuals were designed to present the insights effectively:  

##### *Pie Charts*  
1. *Total Sales by State/Province*  
2. *Total Sales by Region*  
3. *Total Sales by City*  
4. *Average Profit by Region*  
5. *Total Shipping Cost by Ship Mode*  
6. *Average Unit Price by Product Category*  

##### *Line Chart*  
- Monthly Profit Trend (*Order Date vs. Sum of Profit*)  

##### *Card Visuals*  
- Displaying *Total Sales, Total Profit, and Total Quantity Ordered*  

##### *Tree Map*  
- *Product Category-wise Sales, grouped by **Technology, Furniture, and Office Supplies*  

##### *Stacked Bar Chart*  
- *Sales Count by Order Priority*  

##### *Waterfall Chart*  
- *Profit Analysis Over Time, grouped by **Product Category*  

##### *Ribbon Chart*  
- *Sales Trend Over Time, based on **Order Date vs. Sum of Sales*  

---

#### *5. Challenges Faced and Solutions*  
- *Duplicate Order ID Issue: The Orders table contained duplicate Order IDs, which prevented the creation of a one-to-many relationship with the Returns table. To fix this, an **ID Bridge Table* was created to manage the relationship correctly.  
- *Map View Disabled*: Initially, the map visualization was not available. This was resolved by enabling map visuals in Power BI settings and correctly categorizing location fields.  

---

#### *6. Dashboard Customization for Better Readability*  
- Applied *consistent colors and themes* to improve readability.  
- Renamed charts to clearly describe the information presented, such as *"Month-wise Profit Trend"* for the line chart.  
- Ensured *data labels were visible* in charts for easy interpretation.  

---

#### *7. Insights and Business Use Cases*  
This report helps in analyzing sales performance, profit trends, and shipping costs. Key benefits include:  
- *Identifying top-performing states and cities* in terms of sales.  
- *Understanding regional profitability* to improve business strategies.  
- *Tracking monthly profit trends* to detect seasonal changes.  
- *Analyzing shipping costs by mode* to optimize logistics expenses.  
- *Evaluating product category performance* to make better inventory decisions.  
- *Understanding order priority distribution* to improve supply chain efficiency.  

---

### *Conclusion*  
This Power BI report provides a structured way to analyze business performance using visual insights. It enables managers to make data-driven decisions by identifying profitable regions, optimizing shipping costs, and understanding sales trends effectively.
