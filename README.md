# 🛍️ Customer Segmentation using K-Means Clustering

## 📌 Overview  
This project applies **K-Means clustering** to segment customers of a retail store based on their purchasing behavior. By analyzing **Annual Income, Spending Score, Age, and Gender**, we identify different customer groups and provide **personalized marketing insights**.  

## 🚀 Features  
✔️ **Customer Segmentation** based on spending habits & income  
✔️ **Elbow Method** to determine optimal `K` clusters  
✔️ **Visualizations** for insightful analysis  
✔️ **Predict New Customer’s Cluster** using the trained K-Means model  
✔️ **Personalized Offers** for each segment based on spending patterns  

---

## 📂 Dataset  
The dataset used in this project is the **Mall Customers Dataset**. It contains:  
- **Customer ID** – Unique ID for each customer  
- **Gender** – Male/Female  
- **Age** – Customer’s age  
- **Annual Income (k$)** – Estimated income  
- **Spending Score (1-100)** – Score assigned based on spending behavior  

🔹 **Data Source**: [Mall Customers Dataset](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python)  

---

## 📊 Tech Stack & Libraries  
- 🐍 **Python** – Data processing & model building  
- 📊 **Pandas, NumPy** – Data handling & preprocessing  
- 🎨 **Matplotlib, Seaborn** – Data visualization  
- 🤖 **Scikit-Learn** – K-Means clustering  

---

## ⚡ Installation & Setup  

### 🔹 1️⃣ Clone the Repository  
```sh
git clone https://github.com/your-username/Customer-Segmentation-KMeans.git
cd Customer-Segmentation-KMeans
```
🔹 2️⃣ Install Dependencies
```sh
pip install -r requirements.txt
```

🔹 3️⃣ Run the Script
```sh
python customer_segmentation.py
```

🔍 Exploratory Data Analysis (EDA)
Before applying K-Means clustering, we performed EDA to understand the data better:
✅ Age vs. Spending Score Analysis – Younger customers tend to have higher spending scores.
✅ Annual Income vs. Spending Score – Identifies different spending groups.
✅ Gender Analysis – No major impact, but slight variations in spending trends.

📌 K-Means Clustering Implementation
🔹 Step 1: Finding Optimal K (Elbow Method)
We tested K values from 1 to 10 and plotted the inertia vs. K curve.
The Elbow Point suggests K = 5 is optimal for segmentation.
🔹 Step 2: Applying K-Means Algorithm
After choosing K = 5, the customers were divided into 5 distinct clusters.
Each cluster represents a unique spending & income group.
📊 Cluster Visualizations
📌 Annual Income vs. Spending Score (Customer Segments)
📌 Age vs. Spending Score (Age-based Spending Patterns)

Example Visualization:

🔮 Predicting New Customer’s Segment
You can predict the cluster for a new customer based on their attributes:

```sh
new_customer = [70, 85, 25, 1]  # (Income: 70k, Score: 85, Age: 25, Gender: Female)
predicted_cluster = predict_cluster(new_customer)
print(f"Predicted Cluster: {predicted_cluster}")
```

🎯 Personalized Marketing Insights
Cluster	Description	Marketing Strategy
0	High-income, high spenders	Premium memberships, luxury discounts 💎
1	High-income, low spenders	Investment offers, financial plans 💰
2	Low-income, high spenders	Cashback, loyalty points 🎁
3	Young frequent shoppers	Student discounts, trend-focused ads 🛍️
4	Balanced mid-range shoppers	General discounts, targeted emails ⚖️
🔹 Retailers can use this segmentation to improve customer targeting and retention! 🚀

📌 Future Improvements
✅ Deploy as a web app with interactive dashboards
✅ Integrate recommendation system for product suggestions
✅ Use Hierarchical Clustering for better segmentation insights

🤝 Contributing
Contributions are welcome! Feel free to fork the repo and submit a PR.

📬 Connect with Me
📧 Email: atharva2004.rajoba@gmail.com
🔗 LinkedIn: www.linkedin.com/in/atharva-rajoba

📌 Star this repository ⭐ if you found it useful! 🚀
