




# Customer Churn Prediction & Retention System

This project is an AI-powered system designed to identify customers who are likely to churn (cancel their insurance policies) and recommends targeted retention strategies based on customer segmentation, satisfaction levels, and cost-value analysis.

##  Features

-  **Churn Prediction**: Uses a machine learning model to predict whether a customer will churn.  
- **Interactive Dashboard**: Built with Streamlit to visualize churn trends, segment customers, and make individual predictions.  
- **Customer Segmentation**: Classifies customers into segments for targeted interventions.  
-  **Retention Strategy Suggestions**: Recommends personalized actions based on customer behavior and value.  
- **Seasonality Consideration**: Accounts for seasonal churn patterns.  
- **Cost vs Value Optimization**: Balances retention cost against lifetime customer value.  

## 🗂Project Structure

```
Customer_Churn_Retention_Updated/
├── customer_data/
│   ├── customers.csv            # Sample customer dataset
│   └── load_data.py             # Data loading utility
├── churn_prediction/
│   └── model.py                 # ML model training script
├── segmentation/
│   └── segment.py               # Segments customers based on churn risk
├── retention_strategy/
│   └── strategy.py              # Suggests retention strategies
├── campaign_execution/
│   └── execute.py               # (Optional) Campaign automation logic
├── dashboard.py                 # Streamlit app for dashboard
├── requirements.txt             # Python dependencies
├── main.py                      # Main entry (optional)
└── README.md                    # You’re reading it!
```

##  Dashboard Preview

Launch the dashboard with:

```bash
streamlit run dashboard.py
```

Features:
- Predict churn for new customers via sidebar form  
-  Visualize churn rates, satisfaction levels, and spending trends  
-  View personalized retention suggestions for each at-risk customer  

##  How It Works

1. **Input**: Customer behavior and profile data  
2. **Prediction**: Trained ML model predicts churn risk  
3. **Segmentation**: Customers are grouped by risk, satisfaction, and value  
4. **Retention Strategy**:
   - High value + high risk → Priority retention
   - Low value + low risk → Minimal action
   - Seasonal churners → Time-based campaigns  
5. **Dashboard**: Displays insights and supports new predictions  

##  Installation

```bash
# Install dependencies
pip install -r requirements.txt

# Run the dashboard
streamlit run dashboard.py
```

## Data Fields (Sample)

- `Age`, `Gender`, `Tenure`, `MonthlySpend`  
- `SupportTickets`, `SatisfactionScore`  
- `PolicyType`, `HasCompetitorPolicy`, `Region`  
- `Churn` (label)  

##  Use Cases

- Insurance companies improving customer retention  
- CX teams identifying at-risk clients  
- Automating churn reduction campaigns  

##  Built With

- **Python**
- **Streamlit** – for dashboard
- **scikit-learn** – for ML model
- **pandas** – for data processing
- **joblib** – for model serialization

## Contributors

- 👤 SiriChandanaNagasai  
- 🎓 Woxsen University

