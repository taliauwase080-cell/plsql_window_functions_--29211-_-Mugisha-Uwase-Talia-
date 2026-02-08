# Sales Analysis Using SQL JOINs and Window Functions

## Project Overview
This project demonstrates practical mastery of SQL JOINs and SQL window functions using PostgreSQL.  
The analysis is based on a realistic retail sales scenario and focuses on customer behavior, product performance, and sales trends.

---

## Business Context
**Industry:** Retail  
**Department:** Sales & Analytics  

The company collects sales transactions across customers, products, and regions. Management needs analytical insights to understand purchasing behavior, identify top-performing products, and segment customers for strategic decision-making.

---

## Data Challenge
Sales data is distributed across multiple relational tables, making it difficult to analyze customer spending patterns, product performance, and time-based sales trends without advanced SQL techniques.

---

## Expected Outcome
The analysis provides insights into customer segmentation, product sales performance, and sales trends over time to support data-driven business decisions.

---

## Success Criteria
The project achieves the following measurable objectives using SQL window functions:
1. Identify top customers by total spending using `RANK()`
2. Calculate running sales totals using `SUM() OVER()`
3. Analyze month-over-month sales growth using `LAG()`
4. Segment customers into quartiles using `NTILE(4)`
5. Support trend and performance analysis for business reporting

---

## Tools Used
- **DBMS:** PostgreSQL  
- **Language:** SQL  
- **Concepts:** SQL JOINs, Window Functions  

---

## Database Schema
The database consists of four related tables:
- **Customers**
- **Products**
- **Orders**
- **Order_Items**

Primary keys and foreign keys are used to enforce relational integrity.  
An Entity Relationship Diagram (ERD) is included in the repository to illustrate table relationships.

---

## SQL JOINs Implementation
The following JOIN types were implemented:
- **INNER JOIN:** Retrieve transactions with valid customers and products
- **LEFT JOIN:** Identify customers who have never made a purchase
- **RIGHT JOIN:** Detect products with no sales activity
- **FULL OUTER JOIN:** Compare customers and orders including unmatched records
- **SELF JOIN:** Compare customers within the same region

These JOINs enable multi-table relational analysis required for accurate reporting.

---

## Window Functions Implementation
All required categories of SQL window functions were implemented:

### Ranking Functions
- `RANK()` to identify top customers by revenue

### Aggregate Window Functions
- `SUM() OVER()` to compute running sales totals

### Navigation Functions
- `LAG()` to analyze period-to-period (month-over-month) sales changes

### Distribution Functions
- `NTILE(4)` to segment customers into spending quartiles

---

## Results Analysis

### Descriptive Analysis
The analysis shows differences in customer spending levels and highlights products contributing most to total revenue.

### Diagnostic Analysis
Higher revenue is driven by repeat customers and specific product categories with consistent demand.

### Prescriptive Analysis
The company should focus marketing efforts on high-value customer segments and optimize inventory for top-performing products.

---

## Repository Structure
### innerjoin

![ER Diagram](/img/innerjoin)
