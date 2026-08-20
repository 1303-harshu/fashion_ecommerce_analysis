# 🛍️ Myntra Fashion Pricing & Brand Performance Analysis

## 📊 Power BI | DAX | Data Analytics | E-Commerce Intelligence

An interactive Power BI dashboard designed to analyze Myntra's fashion product catalog across pricing, discounts, categories, gender, ratings, and customer reviews.

The project focuses on converting raw e-commerce product data into actionable business insights that can support pricing, merchandising, promotional, and category-level decisions.

---

## 🎯 Project Objective

The objective of this project is to understand:

- How Myntra's product catalog is distributed across categories and genders
- How pricing varies across different product segments
- Which price segments receive higher discounts
- How product ratings vary across categories
- Which categories have the largest product assortment
- How customer reviews and ratings can be used as indicators of product engagement
- How an e-commerce business can use data to improve pricing and promotional strategies

---

## 📌 Key Business Questions

1. Which categories contain the largest number of products?
2. What is the overall average selling price?
3. What percentage of products are discounted?
4. Which price segment receives the highest average discount?
5. How is the product catalog distributed between men and women?
6. Which categories have the highest average ratings?
7. How broad is the brand/product assortment?
8. What pricing patterns can be identified from the catalog?

---

## 📂 Dataset

The dataset contains Myntra fashion product information including:

- Brand Name
- Category
- Individual Category
- Gender
- Product Description
- Original Price
- Discounted Price
- Discount Offer
- Ratings
- Reviews
- Size Options
- Product URL

### Dataset used in Power BI

After data cleaning and filtering incomplete pricing records, the Power BI analysis contains approximately:

**117K+ product records**

The original dataset contains a substantially larger number of raw records; the final analytical dataset depends on the cleaning and filtering steps applied in Power Query.

---

# 🧹 Data Cleaning & Preparation

Data preparation was performed using **Power Query in Power BI**.

The following steps were performed:

- Removed incomplete pricing records
- Checked and corrected numerical data types
- Converted price fields into numeric values
- Converted ratings into decimal values
- Converted reviews into whole numbers
- Created calculated pricing fields
- Created discount categories
- Created price segments
- Validated the resulting dataset before visualization

---

# 🧮 DAX Calculations

Several calculated columns and measures were created to support business analysis.

### Discount Amount

```DAX
DiscountAmount =
'Myntra Fasion Clothing'[OriginalPrice (in Rs)]
-
'Myntra Fasion Clothing'[DiscountPrice (in Rs)]
