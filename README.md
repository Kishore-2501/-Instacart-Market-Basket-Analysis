#  Instacart Market Basket Product Reordering Prediction

This project applies deep learning to predict whether a user will reorder a product based on their past purchase behavior.

---

##  Overview

Reordering prediction is essential for e-commerce platforms to optimize inventory, recommend products, and improve customer retention. This project builds a deep learning model using structured historical purchase data to classify if a product will be reordered.


---

##  Dataset

This project uses the [Instacart Market Basket Analysis dataset](https://www.instacart.com/datasets/grocery-shopping-2017), which includes:

| File Name                    | Description                                   |
|-----------------------------|-----------------------------------------------|
| `orders.csv`                | Order-level metadata (user ID, order number)  |
| `order_products__prior.csv` | Products from all prior orders                |
| `order_products__train.csv` | Products and labels used for training         |
| `products.csv`              | Product names and IDs                         |
| `aisles.csv`                | Aisle categories                              |
| `departments.csv`           | Department categories                         |

---

##  Objectives

- Build a model to predict if a user will reorder a product.
- Perform feature engineering on user, product, and user-product levels.
- Address class imbalance using class weighting.
- Evaluate the model using ROC AUC, F1-score, and classification metrics.

---

##  Features Created

###  User Features
- Total number of orders
- Average days between orders
- User-level reorder ratio

###  Product Features
- Total number of purchases
- Reorder rate (product-level)

###  User-Product Interaction Features
- Number of times user reordered product

---

##  Evaluation Metrics

- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **ROC AUC Score**

---

## 📝 Results

| Metric       | Score |
|--------------|-------|
| Accuracy     | 83%   |
| F1-score     | 0.83  |
| ROC AUC      | 0.88  |


---

## Files uploaded
- Feature_Engineering.ipynb # All Feature creation
- Model.ipynb # Model training & evaluation
- Final_Project.ipynb # Complete workflow
- reorder_prediction_model.h5 # Trained model
- README.md # Project overview (this file)
