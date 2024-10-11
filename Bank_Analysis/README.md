# Banking Algorithms Analysis

In this project description we will cover:

* [***Project Overview:***](#project-overview) the project goal, audience, and dataset
* [***Business Understanding:***](#business-understanding) understanding the business problem or opportunity that the project aims to address
* [***Data Understanding:***](#data-understanding) gathering, exploring, and comprehending the data that will be used to solve the business problem
* [***Conclusion:***](#conclusion) brief summary of the findings and recommendations.


### Project Overview
Responsible AI is top of mind for business leaders, along with an urgent need to understand the decision process behind these algorithms. With great potential comes great risk. Not being able to understand an AI system can lead to a “black box” effect, which limits an organisation’s ability to explain and defend business-critical decisions.

In this project, a large bank has asked us to evaluate the marketing algorithms they use for retail banking. Their sophisticated phone marketing algorithm predicts whether a certain person will subscribe to a term deposit or not. Based on that assessment, the bank then optimises its phone calling strategy.

With this algorithm, the bank has been successful in predicting which clients are more likely to subscribe to their term deposits. Our task at hand is to explain to our clients how certain models and algorithms can lead to decision-making processes and to help explain both overall decision-making and also individual choices and predictions, tailored to the perspectives of different stakeholders.

### Business Understanding
Analyzing a bank's customer data to identify key segments that are most likely to convert to the bank's term deposit. By understanding which factors influence a customer's decision to subscribe to the term deposit, it is easier to develop targeted strategies to optimize marketing efforts, and ultimately increase revenue for the bank.

### Data Understanding
In this folder, `dataset` is a dataset from 
* [Kaggle] (https://www.kaggle.com/datasets/henriqueyamahata/bank-marketing)

### Data Description
1. **age** - Age of the customer.

2. **job** - Type of job that the customer holds.

3. **marital** - Marital status of the customer.

4. **education** - Level of education of the customer.

5. **default** - Whether the customer has credit in default.

6. **housing** - Whether the cusomer has housing loan.

7. **loan** - Whether the customer has a personal loan.

8. **contact** -  Contact communication type.

9. **month** - Last contact month of the year.

10. **day_of_week** - Day of the week when the customer was last contacted.

11. **duration** - last contact duration, in seconds.

12. **campaign** - number of contact performed during this campaign.

13. **pdays** - Number of days since the client was last contacted from a previous campaign.

14. **previous** - Number of contacts performed before this campaign.

15. **poutcome** - Outcome of the previous marketing campaign.

16. **emp.var.rate** - Employment Variation rate.

17. **cons.price.idx** - Consumer Price Index.

18. **cons.conf.idx** - Consumer Confidence Index.

19. **euribor3m** - Euribor 3 month rate(European interbank offered rate)

20. **nr.employed** -  Number of employees(indicator of labor market conditions)

21. **y** - Target variable that indicates whether the customer subscribed to a term deposit(yes or no)

### Exploratory Data Anaylsis


### Modeling
In this project, I used classification modeling to predict which bank customers are most likely to subscribe to the bank deposit.
I built three models in my project:
* **Base model:** Using Logistic Regression and SMOTE
* **Random Forest Classifier**
* **Neural Network Model**

### Evaluation
These models were evaluated using metrics such as precision, recall and accuracy.

 ***Model Perfomance Metrics***

*Accuracy*: The percentage of correctly classified instances out of the total instances. For my models, I observed:
Base Model Accuracy: 91%
Random Forest Model Accuracy: 91%
Neural Network Model: 90.8%

***Feature Importances***
I used LIME library explain individual predictions. LIME will provide local interpretability, showing the effect of individual features on a single prediction. From this I was able to find that the key factors that affect the phone call marketing strategy are the duration fo the phone call and also the number of time a customer was previously contacted.

## Recommendations
Based on the findings that **phone call duration** and the **number of previous contacts** are key factors affecting the success of the phone call marketing strategy, the following recommendations can be made:

### 1. **Prioritize Longer Phone Conversations**
   - **Insight**: Customers who engage in longer phone conversations tend to have higher subscription rates. This suggests that these customers are more interested and engaged, giving the sales team a better opportunity to convert them.
   - **Recommendation**: Train agents to focus on extending meaningful conversations rather than rushing through calls. Provide them with guidelines and conversation scripts that emphasize addressing customer concerns and clearly explaining product benefits, aiming to keep the customer engaged for a longer duration.

### 2. **Target Customers with Previous Contacts**
   - **Insight**: The number of times a customer was previously contacted is a significant factor. Customers who have been contacted multiple times may be more likely to subscribe, as repeated exposure can reinforce interest or familiarity with the product.
   - **Recommendation**: Implement a follow-up strategy that focuses on customers who have been contacted before but haven't subscribed. This could involve segmenting these customers and designing specific follow-up campaigns aimed at nurturing their interest.

### 3. **Refine Contact Frequency**
   - **Insight**: While repeated contact increases subscription rates, excessive or poorly timed follow-ups could be perceived as annoying.
   - **Recommendation**: Strike a balance by designing a smart contact schedule that doesn't overwhelm customers. Use data to determine the optimal number of calls and the appropriate time intervals between contacts. You could also experiment with personalized outreach strategies based on previous call outcomes and customer preferences.

### 4. **Leverage Data for Call Optimization**
   - **Insight**: The success of phone marketing depends on both the **duration** and **previous contacts**.
   - **Recommendation**: Implement a data-driven approach to determine which customers should be prioritized for follow-up and which call durations are most effective for different segments. Use historical data to predict customer behavior and optimize future call strategies.

### 5. **Improve Call Agent Training**
   - **Insight**: Effective phone marketing involves maintaining customer interest for longer durations.
   - **Recommendation**: Invest in additional training for call agents, focusing on techniques to keep customers engaged. Agents can be trained on active listening, answering key questions effectively, and personalizing conversations based on the customer’s history and interests.

By focusing on extending phone conversations and creating strategic follow-up plans based on previous contacts, the business can improve the effectiveness of its phone call marketing campaigns.
  
