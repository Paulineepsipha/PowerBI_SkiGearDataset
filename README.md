# PowerBI_SkiGearDataset
Power Bi analyzing on the datasets for Avalanche Inc, a hypothetical premium ski gear company specializing in high-performance winter sports equipment. The datasets provide insights into product catalog, customer reviews, order history, and shipping logistics.

# Avalanche Ski Gear Company - Dataset Documentation

## 📦 Overview
This repository contains curated datasets for **Avalanche Inc.**, a fictional premium ski gear company specializing in high-performance winter sports equipment. The datasets provide insights into the product catalog, customer reviews, order history, and shipping logistics—ideal for analytics, machine learning, and data exploration projects.

---

## 📊 Datasets

### 1. 🛍 Product Catalog (`product-catalog-with-category-label`)
**Description**: A comprehensive catalog of Avalanche's premium ski equipment and apparel.

**Fields**:
- `name`: Product name  
- `description`: Detailed technical specifications and features  
- `price`: Product price (USD)  
- `category`: Product category (e.g., Skis, Apparel, Accessories)  

**Sample Products**:
- Alpine Skis  
- Performance Racing Skis  
- Thermal Gloves  
- Insulated Jacket  
- Carbon Fiber Poles  
- Ski Goggles  
- Pro Ski Boots  
- Mountain Series Helmet  
- Alpine Base Layer  
- Avalanche Safety Pack  

---

### 2. ⭐ Customer Reviews (`customer_reviews`)
**Description**: Feedback and sentiment data for Avalanche's products.

**Fields**:
- `PRODUCT`: Product name  
- `DATE`: Date of review  
- `SUMMARY`: Detailed review text  
- `SENTIMENT_SCORE`: Sentiment score ranging from -1.0 (negative) to 1.0 (positive)  

**Insights**:
- Reviews span **October to December 2023**  
- Includes testing feedback from various skiing conditions  
- Sentiment scores help monitor customer satisfaction over time  

---

### 3. 🧾 Order History (`order-history`)
**Description**: Transactional data of customer purchases.

**Fields**:
- `Order ID`: Unique order identifier  
- `Customer ID`: Unique customer identifier  
- `Product ID`: Unique product identifier  
- `Product Name`: Name of purchased product  
- `Quantity Ordered`: Number of items purchased  
- `Price`: Unit price in USD  
- `Total Price`: Total order value  
- `Date`: Order date  

**Coverage**:
- Orders placed from **October 15, 2023 to November 7, 2023**  
- Includes **25 unique orders**

---

### 4. 🚚 Shipping Logs (`shipping-logs`)
**Description**: Tracking and delivery status for customer orders.

**Fields**:
- `order_id`: Linked to Order History  
- `shipping_date`: Date of shipment  
- `carrier`: Shipping provider  
- `tracking_number`: Unique package tracking number  
- `latitude`: Delivery latitude (decimal degrees)  
- `longitude`: Delivery longitude (decimal degrees)  
- `status`: Current delivery status  

**Carriers Include**:
- SwiftWing Logistics  
- MountainRoute Express  
- AlpineSpeed Delivery  
- PeakPath Shipping  
- SnowRunner Logistics  
- SummitLine Express  

---

## 🔗 Data Relationships

- **Order History** links to **Shipping Logs** via `Order ID`.
- **Product Catalog** contains information on products referenced in **Order History** and **Customer Reviews**.
- **Customer Reviews** provide feedback on items in the **Product Catalog**.

---

## ✅ Data Quality

- All datasets are available in **CSV** and **JSON** formats  
- Uniform **date formatting**: `YYYY-MM-DD`  
- Standard **currency format**: USD  
- Complete product descriptions and technical specifications  
- Detailed shipment tracking with geographic coordinates  

---

## 📌 Usage Notes

- Product prices are listed in **USD**  
- Sentiment scores range from **-1.0** (negative) to **1.0** (positive)  
- Shipping coordinates use **decimal degree format**  
- All dates follow the **YYYY-MM-DD** format  

---

## 🔄 Data Updates

| Dataset          | Update Frequency         | Last Updated         |
|------------------|--------------------------|----------------------|
| Product Catalog  | Static                   | December 2023        |
| Customer Reviews | Updated                  | Through December 2023|
| Order History    | Periodic (Monthly)       | October–November 2023|
| Shipping Logs    | Updated with deliveries  | Through November 2023|
