
# E-Commerce Shipping Performance Analysis

This project analyzes shipping performance data for an e-commerce company. The goal is to explore features affecting delivery time and build classifiers to predict whether a product will be delivered on time.

---

## 📁 Dataset Overview

The dataset contains 10,999 entries with 12 columns:

- **ID**: Order ID
- **Warehouse_block**: Source warehouse category
- **Mode_of_Shipment**: Shipping method used (e.g., Flight, Ship, Road)
- **Customer_care_calls**: Number of calls made by customer
- **Customer_rating**: Customer rating (1 to 5)
- **Cost_of_the_Product**: Cost in local currency
- **Prior_purchases**: Number of previous purchases
- **Product_importance**: Product priority (low, medium, high)
- **Gender**: Gender of customer
- **Discount_offered**: Discount given
- **Weight_in_gms**: Weight of product
- **Reached.on.Time_Y.N**: Target variable (1 = delayed, 0 = on time)

---

## 🧹 Data Preprocessing

- Handled missing/null values
- Visualized feature distribution using seaborn
- Analyzed correlations and distributions across target classes
- Label encoded categorical variables
- Feature scaling applied where needed

---

## 📊 Exploratory Data Analysis

- Distribution plots of customer ratings, discounts, weights
- Boxplots used to detect outliers
- Heatmaps used to show feature correlation
- Class imbalance checked using value counts

---

## 🧠 Model Building

The project uses various classification algorithms to predict delivery delay:

1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest**
4. **K-Nearest Neighbors (KNN)**
5. **Support Vector Machine (SVM)**

---

## 📈 Results & Evaluation

Each classifier was evaluated using:

- **Accuracy**
- **Confusion Matrix**
- **Precision, Recall, F1-Score**
- **ROC Curve**

### Sample Results:

| Classifier           | Accuracy | F1-Score |
|----------------------|----------|----------|
| Logistic Regression  | ~72%     | ~0.71    |
| Decision Tree        | ~75%     | ~0.74    |
| Random Forest        | ~81%     | ~0.80    |
| KNN                  | ~76%     | ~0.75    |
| SVM                  | ~73%     | ~0.72    |

---

## ✅ Final Output

The final model (Random Forest) achieves the best performance with **~81% accuracy**. It's effective in classifying whether an order will be delivered on time or not based on the product and customer features.

---

## 🧾 Steps Followed

1. **Load dataset** and inspect
2. **Visualize and analyze** distributions
3. **Clean and preprocess** data
4. **Encode categorical variables**
5. **Split data** into training and testing
6. **Train multiple models**
7. **Evaluate and compare** model results
8. **Conclude** with best-performing classifier

---

## 📌 Conclusion

- Random Forest is the most effective classifier for this dataset.
- Discount offered and product weight are highly influential features.
- This analysis can help logistics teams improve delivery performance forecasting.

---

