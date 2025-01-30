# **Bank Marketing Subscription Prediction**

## **Project Overview**

This project analyzes a Portuguese bank's marketing campaign to identify factors that influence customer subscription to a term deposit from direct marketing campaigns (phone calls). The dataset consists of customer information, call details, and past marketing interactions. The objective is to understand which factors contribute to a successful call, allowing the marketing team to refine their strategy. Traditional telemarketing campaigns often face challenges in efficiency, as evidenced by the low subscription rate in this dataset (\~10%). This highlights the need for data-driven strategies to improve targeting and reduce wasted effort.

### **Key Business Questions Addressed:**

* What factors contribute to a successful customer subscription?  
* How does call duration impact conversion rates?  
* Are there specific customer characteristics or behaviors that increase the likelihood of subscription?  
* How can marketing campaigns be adjusted based on these findings?

---

## **Model Selection and Results**

### **Approach:**

To analyze customer subscription patterns, three models were tested:

* Logistic Regression  
* Random Forest  
* XGBoost

After evaluating these models, Random Forest was selected due to its strong performance and interpretability. It achieved:

* \~94% accuracy  
* ROC AUC of \~0.99 (indicating strong predictive separation)  
* Balanced precision and recall, ensuring both customer groups were correctly identified.

---

## **Key Findings & Business Impact**

### **1\. Call Duration is the Most Influential Factor**

* The longer a call lasts, the more likely a customer is to subscribe.  
* This insight suggests that call agent training and scripting can significantly impact success rates.  
* **Business Action:** Train agents on strategies that increase customer engagement **time** while maintaining a positive experience.

### **2\. The Contact Method Affects Engagement**

* Customers contacted via an "unknown" method behaved differently from those contacted via known methods.  Also shows the “unknown” method has the lowest subscription rates.  
* **Business Action:** Investigate why certain contact methods work better and shift focus to more effective communication channels.

### **3\. Previous Contact History Impacts Subscription Rates**

* Customers who were contacted recently (`pdays` feature) showed different engagement patterns.  
* **Business Action:** Adjust marketing frequency—avoid over-contacting customers who were recently called, as it may reduce effectiveness.

### **4\. Subscription Rates Vary by Time of Year**

* May and July showed higher subscription success rates.  
* **Business Action:** Align marketing efforts with seasonal trends—increase campaign efforts in high-conversion months and test new strategies in lower-performing months.

### **5\. Customer Characteristics Matter**

* Customers with certain job types (e.g., blue-collar), along with marriage and housing statuses responded differently to the marketing campaign.  
* **Business Action:** Personalize marketing approaches based on demographic insights to improve customer targeting.

---

## **Final Decision & Next Steps**

* Random Forest was chosen for its accuracy and interpretability.  
* Insights will be used to refine marketing strategy, improve agent training, and optimize customer outreach.

### **Next Steps for Business Implementation**

* Refine agent scripts to keep customers engaged longer.  
* Focus on more effective communication channels  
* Adjust marketing frequency based on past engagement to avoid customer fatigue.  
* Optimize campaign timing by increasing marketing efforts in months with higher conversion rates.  
* Personalize marketing approaches based on demographics.

