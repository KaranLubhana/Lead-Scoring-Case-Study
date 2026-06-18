# Lead-Scoring-Case-Study
"A Machine Learning project using Logistic Regression to build a Lead Scoring system (0-100) that optimizes the customer conversion funnel from 30% to 80% for an education platform."
# Lead-Scoring-Case-Study (Predictive Logistic Regression Model)

An end-to-end Machine Learning and Business Optimization project designed to solve a critical revenue funnel bottleneck for an online education platform (**X Education**). 

The goal of this project is to build a predictive model that filters out low-potential queries and highlights "Hot Leads" for the sales team, driving the conversion rate from a low **30% up to the target of 80%**.

---

### 📝 The Business Challenge
X Education acquires thousands of professional leads daily through search engines, social media, and word-of-mouth referrals. However, their conversion rate is quite low (~30%), meaning the sales team wastes major bandwidth chasing cold inquiries. 

By building a **Logistic Regression model**, we assign a dynamic **Lead Score (0 to 100)** to every lead. A higher score means the client is highly likely to purchase a course, helping the sales team optimize their daily outreach and prioritize high-value targets.

---

### 📊 Project Workflow & Data Approach

1. **Data Sanitization & Cleaning:** Imputed missing data and structurally handled hidden nulls like the `'Select'` drop-down values, which represented unpicked choices by prospects.
2. **Exploratory Data Analysis (EDA):** Uncovered patterns and major conversion drivers. Discovered clear indicators like how `Total Time Spent on Website` heavily influences conversion probability.
3. **Feature Engineering:** Converted categorical features into dummy variables, partitioned the data into a **70:30 Train-Test split**, and standardized numerical values using `StandardScaler`.
4. **Model Tuning & Selection:** Leveraged **Recursive Feature Elimination (RFE)** for automated column reduction, followed by manual adjustments using **P-values** and **VIF (Variance Inflation Factor)** to keep the model clean from multicollinearity.
5. **Threshold Optimization:** Shifted beyond the default 0.5 threshold by evaluating the **ROC Curve** alongside Sensitivity-Specificity and Precision-Recall tradeoffs to match the CEO’s strategic 80% target.

---

### 💡 Key Takeaways & Strategic Insights
* **Top Drivers:** Leads coming via `Welingak Website` or `References`, and individuals whose last recorded activity was an `SMS Sent` showed the strongest conversion rates.
* **Balanced Architecture:** The final model balances precision and recall perfectly, ensuring the sales team doesn't miss out on hot leads while minimizing calls to dead ends.
* **Operational Impact:** The 0-100 score gives the sales workforce a clear dashboard hierarchy to schedule their calling queues effectively.

---

### 🛠️ Technology Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, Statsmodels, Matplotlib, Seaborn

---

### 📁 Repository Deliverables
* `Lead_Scoring_Case_Study.ipynb`: The core step-by-step Jupyter Notebook containing code implementation and diagnostic graphs.
* `Lead_Scoring_Presentation.pdf`: A business-centric deck summarizing methodology and ROI findings for executive stakeholders.
* `Lead_Scoring_Questions_Answers.docx`: Solutions to dynamic business scenarios and changing constraint problems.
* `Lead_Scoring_Summary_Report.pdf`: A 500-word detailed execution report covering technical learnings.

---
*Disclaimer: This project was completed as part of a professional data science specialization curriculum (Lead-Scoring-Case-Study).*
