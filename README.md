# Case Study: Excel Retail Sales Analysis

## Project Overview  
Using Microsoft Excel, I transformed a year’s worth of retail transaction data into a multi-layered business intelligence solution.  
Spanning over 1,000 customers, 2,514 items sold, and 456,000 in revenue, the dataset allowed me to explore customer behavior, sales performance, product trends, and seasonal patterns—all structured through pivot logic, working sheets, and visual dashboards.

## Dataset Summary  
The dataset represents individual transactions across Beauty, Clothing, and Electronics categories between January and December 2023.

**Key Fields:**  
• Transaction ID, Date, Customer ID  
• Gender, Age, Product Category  
• Quantity, Price per Unit, Total Amount  

To enable deeper segmentation, I engineered custom columns:

| Column Name      | Purpose                                                                 |
|------------------|-------------------------------------------------------------------------|
| Month            | Extracted from Date for time-based pivots                              |
| Season           | Grouped into Spring, Summer, Fall, Winter                               |
| Age Group        | Categorized customers into:<br>→ Below 30, 30–50, Above 50             |
| Customer Segment | Based on spend amount:<br>→ Low (≤600), Medium (600–1200), High (>1200) |

## Data Cleaning & Transformation  

** Blank Value Checks**  
• No missing values detected in identifiers or financial columns  
• Filters and COUNTBLANK applied to validate data integrity  

** Duplicate Checks**  
• Transaction ID verified using Conditional Formatting  
• All IDs confirmed unique—no duplicates found  

** Helper Columns Created**  
• Month, Season, Age Group, and Customer Segment were generated using TEXT, IF, and LOOKUP functions  
• These powered dynamic filters and cross-tabulations  

## Analytical Sheet Structure  

I used multiple themed sheets, each focused on a unique analytic dimension:

| Sheet Name        | Purpose                                                           |
|-------------------|-------------------------------------------------------------------|
| Working Sheet     | Cleaned dataset with all helper columns                           |
| Monthly Trends    | PivotTable showing revenue & quantity over months                 |
| Product Insights  | Analysis of category performance across gender, age, and segment  |
| Gender Analysis   | Breakdown of revenue by gender and product                        |
| Customer Segments | Mapping age group & spend level interactions                      |
| Seasonal Trend    | Pivot showing how seasonality affects sales quantity and value    |
| Sales Dashboard   | Executive-level KPIs and product performance visuals              |
| Customer Dashboard| Demographic behavior and preferences visualization                |

These analytical worksheets acted as intelligence modules, each revealing specific stories before final dashboards were built.

## Deep-Dive Pivot Analysis  

### Monthly & Seasonal Trends  
• Highest revenue months: May, October, December  
• Winter season drives highest overall revenue (125,730)  
• Spring has the highest sales volume (667 units)  

### Gender Patterns  
| Gender | Revenue  | Units Sold |
|--------|----------|------------|
| Female | 232,840  | 1,298 units |
| Male   | 223,160  | 1,216 units |

• Females prefer Beauty and Clothing  
• Males dominate Electronics purchases  
• Revenue split is nearly balanced but varies by category  

### Age-Based Spend  
| Age Group  | Revenue | Units Sold |
|------------|---------|------------|
| Below 30   | 123,155 | 625        |
| 30–50      | 199,535 | 1,112      |
| Above 50   | 133,310 | 777        |

• Age 30–50 is the top contributing segment across all product categories  
• Below 30 are more frequent buyers of Clothing, but at lower spend values  

### Customer Segment Mapping  
| Segment | Revenue | Units Sold |
|---------|---------|------------|
| High    | 237,800 | 562        |
| Medium  | 151,300 | 405        |
| Low     | 66,900  | 1,547      |

• High spenders are fewer, but generate more than 50% of total revenue  

## Key Insights  

### Age Group Targeting  
• 30–50 age bracket generates 44% of revenue  
• Females drive purchases in Beauty & Clothing  
• Males spend more in Electronics  

### Product Strategy  
| Category    | Revenue | Units Sold |
|-------------|---------|------------|
| Electronics | 156,905 | 849        |
| Clothing    | 155,580 | 894        |
| Beauty      | 143,515 | 771        |

• Clothing leads in volume  
• Electronics commands higher order value  
• Beauty thrives during winter, mainly driven by females  

### Seasonal Performance  
| Season | Revenue  | Units Sold |
|--------|----------|------------|
| Winter | 125,730  | 620        |
| Spring | 116,010  | 667        |
| Summer | 109,140  | 600        |
| Fall   | 105,120  | 627        |

• Winter peaks in revenue, especially in Beauty  
• Spring sees highest unit sales, led by Clothing  

## Recommendations  
• Increase stock of Beauty products ahead of Winter peak  
• Launch tailored campaigns for 30–50 high-spend customers  
• Offer entry-level bundles for Below 30 low spenders  
• Align inventory with seasonally dominant categories  
• Use targeted promotion strategies by gender x product affinity  
