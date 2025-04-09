Project Overview: This project focuses on building a machine-learning model to predict whether a customer review score for an order will be positive (4-5) or negative (1-3). The dataset includes customer orders, product details, payment information, and delivery metrics. The goal is to analyze key factors affecting review scores and provide actionable business recommendations.

Business Problem: Customer satisfaction is crucial for e-commerce success. Understanding what influences review scores helps businesses optimize logistics, pricing, and customer service. By predicting review scores in advance, companies can take proactive measures to improve customer experience and minimize negative feedback.

Data Sources & Preprocessing: The project utilized multiple datasets:

Orders Dataset: Order status, timestamps, and delivery times. Products Dataset: Product details such as weight, dimensions, and category. Order Items Dataset: Quantity, price, and shipping costs per order. Payments Dataset: Payment types, instalments, and complexity. Reviews Dataset: Review scores and response times.

Data Cleaning & Feature Engineering: Handled missing values and outliers. Created derived features such as delivery_delay, total_shipping_cost, payment_complexity, and order_size. Engineered interaction terms to capture relationships between features.

Algorithms Tested: Gradient Boosting Trees (GBTClassifier) – Best Performing Model, Random Forest, Logistic Regression

Final Model (GBTClassifier) Performance:  Accuracy: 81.6, AUC: 0.706

 Hyperparameter tuning was conducted using cross-validation to optimize model performance. ✔ Stacking models (GBT + RandomForest + Logistic Regression) were also tested but not implemented in this solution.

Key Insights & Business Recommendations:  Delivery delays were the most significant predictor of negative reviews.  High shipping costs and large order sizes negatively impacted satisfaction. Orders paid via vouchers showed distinct patterns compared to other payment methods.

Next Steps: Implement real-time prediction for proactive customer support.  Optimize delivery processes to reduce delays and improve satisfaction. 🚀 Test additional ensemble learning techniques to increase AUC.

Requirements: Databricks / Apache Spark Python 3.8+ PySpark, XGBoost, Imbalanced-learn
