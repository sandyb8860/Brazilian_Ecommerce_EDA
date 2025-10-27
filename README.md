# Brazilian E-Commerce Data Analysis (Olist Dataset)

## Project Overview

This project performs comprehensive Exploratory Data Analysis (EDA) on the Brazilian E-commerce Public Dataset from Olist, available on Kaggle. The analysis aims to uncover meaningful insights into customer behavior, sales trends, delivery performance, and market dynamics by examining orders, payments, product reviews, and logistics data.

## Objectives

The primary objectives of this analysis are:

- **Understand Customer Behavior**: Analyze purchase patterns, payment preferences, and regional demand distribution
- **Identify Revenue Drivers**: Determine high-performing product categories and seasonal sales trends
- **Evaluate Delivery Performance**: Assess shipping efficiency and its impact on customer satisfaction
- **Analyze Customer Satisfaction**: Study the relationship between delivery times, product quality, and review ratings
- **Generate Business Insights**: Provide actionable recommendations for improving operations and customer experience

## Dataset Information

**Source**: [Kaggle - Brazilian E-commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

**Description**: The dataset contains information about 100,000+ orders made at the Olist Store in Brazil between 2016 and 2018. It includes multiple dimensions:

- Orders data (order status, timestamps, delivery dates)
- Customer information (location, unique customer IDs)
- Product details (categories, dimensions, descriptions)
- Payment information (payment type, installments, values)
- Reviews and ratings (scores, comments, timestamps)
- Seller information (locations, IDs)
- Geolocation data (coordinates for customers and sellers)

## Tech Stack & Tools

**Programming Language**: Python 3.x

**Libraries**:
- **Data Analysis**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn, Plotly
- **Environment**: Jupyter Notebook

**Data Source**: Kaggle - Brazilian E-commerce Public Dataset

## Key Metrics Analyzed

### Sales & Revenue Metrics
- Total revenue generated
- Average order value (AOV)
- Revenue by product category
- Monthly and seasonal sales trends
- Order volume distribution

### Customer Metrics
- Customer distribution by state and city
- Payment method preferences
- Order frequency and repeat purchase behavior
- Customer satisfaction scores

### Operational Metrics
- Average delivery time
- Delivery time vs. estimated time
- Late delivery rate
- Review score distribution
- Correlation between delivery performance and ratings

### Product Metrics
- Top-selling product categories
- Average order value by category
- Product performance across regions
- Review scores by product category

## Analysis Process

### 1. Data Import & Integration
- Loaded multiple CSV files (orders, customers, products, payments, reviews, sellers)
- Merged datasets using appropriate keys (order_id, customer_id, product_id, seller_id)
- Created a unified analytical dataset

### 2. Data Cleaning & Preprocessing
- Handled missing values through imputation and removal strategies
- Removed duplicate records
- Standardized column names and data types
- Converted timestamp columns to datetime format
- Handled outliers in price and delivery time data

### 3. Feature Engineering
- **Temporal Features**: Extracted year, month, day of week, and hour from timestamps
- **Delivery Metrics**: Calculated actual delivery time, delivery delay, and on-time delivery indicators
- **Revenue Metrics**: Computed total order value including freight
- **Customer Segmentation**: Created customer lifetime value and frequency indicators

### 4. Exploratory Data Analysis

#### Sales Analysis
- 📈 **Sales Trend Analysis**: Monthly and yearly revenue patterns, identifying peak seasons
- 💰 **Revenue Distribution**: Analysis of order value distribution and high-value segments
- 📊 **Category Performance**: Revenue contribution by product categories

#### Geographical Analysis
- 🌎 **Regional Distribution**: Orders and revenue by state and city
- 🗺️ **Market Concentration**: Identification of high-demand regions
- 📍 **Customer-Seller Distance**: Analysis of logistics efficiency

#### Payment Analysis
- 💳 **Payment Methods**: Distribution of payment types (credit card, boleto, debit, voucher)
- 💵 **Installment Patterns**: Analysis of payment installment preferences
- 💲 **Payment Value Analysis**: Relationship between payment method and order value

#### Delivery Performance
- 📦 **Delivery Time Analysis**: Average, median, and distribution of delivery times
- ⏱️ **On-time Delivery Rate**: Percentage of orders delivered within estimated time
- 🚚 **Carrier Performance**: Analysis of shipping efficiency

#### Customer Satisfaction
- ⭐ **Review Score Distribution**: Analysis of 1-5 star ratings
- 📝 **Satisfaction Drivers**: Correlation between delivery performance and ratings
- 😊 **Category Satisfaction**: Review scores by product category

## Key Insights & Findings

### Geographic Insights
- **São Paulo (SP)** dominates with the highest number of orders and revenue contribution
- **Southeast region** (SP, RJ, MG) accounts for the majority of e-commerce activity
- Strong market concentration in major metropolitan areas
- Opportunity exists to expand in underserved regions (North and Northeast)

### Sales & Revenue Insights
- **Steady growth trend** observed from 2016 to 2018
- **Seasonal peaks** during specific months (Black Friday, holiday seasons)
- **Health & beauty**, **watches & gifts**, and **bed, bath & table** are top-performing categories
- **Electronics and furniture** show higher average order values but lower volume

### Payment Insights
- **Credit card** is the overwhelmingly preferred payment method (70%+)
- Customers frequently use **installment payments** for higher-value purchases
- **Boleto** (Brazilian payment method) is second most popular
- Average order value varies significantly by payment method

### Delivery Performance Insights
- Average delivery time: **12-15 days**
- Significant variation in delivery times across different regions
- **Distance between seller and customer** is a major factor in delivery time
- Late deliveries strongly correlate with poor review scores
- Opportunities exist to optimize logistics and reduce delivery times

### Customer Satisfaction Insights
- Overall **high satisfaction** with majority of 4-5 star reviews
- **Delivery time is the primary driver** of customer satisfaction
- Products delivered late receive significantly lower ratings
- Categories with better logistics have higher satisfaction scores
- Review comments highlight shipping delays as main complaint

## Business Recommendations

### 1. Optimize Logistics & Delivery
- **Priority**: Reduce delivery times, especially for distant regions
- **Action**: Establish regional distribution centers in high-demand areas
- **Impact**: Improved customer satisfaction and reduced late delivery rates

### 2. Regional Expansion Strategy
- **Priority**: Expand seller network in underserved regions
- **Action**: Incentivize sellers in North and Northeast regions
- **Impact**: Reduced shipping distances and faster deliveries for those regions

### 3. Category-Specific Strategies
- **High-value categories** (electronics, furniture): Focus on white-glove delivery services
- **High-volume categories** (health & beauty): Optimize for bulk fulfillment
- **Impact**: Category-specific customer experience improvements

### 4. Payment Method Optimization
- **Action**: Promote installment payment options for higher-value items
- **Action**: Offer discounts for faster payment methods (credit card vs. boleto)
- **Impact**: Increased conversion rates for high-value products

### 5. Seller Performance Management
- **Action**: Implement seller ratings based on delivery performance
- **Action**: Provide logistics support and training for sellers
- **Impact**: Improved overall marketplace quality and customer satisfaction

### 6. Customer Experience Enhancement
- **Action**: Implement proactive delivery delay notifications
- **Action**: Set realistic delivery expectations based on distance
- **Action**: Provide delivery time guarantees for premium customers
- **Impact**: Better customer expectations management and satisfaction

### 7. Seasonal Planning
- **Action**: Prepare inventory and logistics capacity for peak seasons
- **Action**: Launch targeted marketing campaigns during high-traffic periods
- **Impact**: Maximized revenue during peak periods without service degradation

## Project Structure

```
Brazilian_Ecommerce_EDA/
│
├── data/                          # Dataset files (CSV)
├── notebooks/                     # Jupyter notebooks with analysis
├── visualizations/                # Generated charts and graphs
├── README.md                      # Project documentation
└── Project Summary.docx          # Detailed project summary
```

## How to Use This Repository

1. **Clone the repository**:
   ```bash
   git clone https://github.com/sandyb8860/Brazilian_Ecommerce_EDA.git
   ```

2. **Install required libraries**:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly jupyter
   ```

3. **Download the dataset** from [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) and place it in the `data/` folder

4. **Run the Jupyter notebooks** to see the complete analysis

## Key Visualizations Included

- Sales trend over time (line charts)
- Revenue by state and city (bar charts, heatmaps)
- Payment method distribution (pie charts)
- Delivery time distribution (histograms, box plots)
- Review score distribution (bar charts)
- Correlation matrices (heatmaps)
- Category performance comparison (bar charts)
- Geographic distribution maps

## Conclusion

This comprehensive EDA project reveals critical insights into Brazilian e-commerce operations, highlighting the importance of logistics optimization and regional strategy. The analysis demonstrates that **delivery performance is the key driver of customer satisfaction**, and **geographic concentration presents both opportunities and challenges**.

The findings provide actionable recommendations for:
- Improving operational efficiency
- Enhancing customer experience
- Expanding market reach
- Optimizing category-specific strategies
- Maximizing revenue potential

These insights can guide strategic decision-making for e-commerce platforms, sellers, and logistics providers operating in the Brazilian market.

## Future Work

- Implement predictive modeling for delivery time estimation
- Develop customer segmentation using clustering algorithms
- Build recommendation systems based on purchase patterns
- Perform sentiment analysis on review comments
- Create interactive dashboards for real-time monitoring
- Analyze seller performance and marketplace dynamics

## Author

**Sandeep Batra**
- GitHub: [@sandyb8860](https://github.com/sandyb8860)

## License

This project is open source and available for educational purposes.

## Acknowledgments

- **Olist** for providing the dataset
- **Kaggle** for hosting the data
- Brazilian e-commerce community for insights and feedback

---

*Last Updated: October 2025*
