# Project Overview: Predicting Customer Churn

## Objective

The goal of this project is to create a predictive model that identifies customers who are likely to stop using a service or product, a phenomenon known as "churn." By recognizing at-risk customers, businesses can implement tailored strategies to retain them.

## Key Components

Data Collection

- **Customer Data:** We'll gather vital information such as demographics, usage habits, transaction histories, and customer interactions.

- **Churn Labels:** It’s important to identify customers who have churned over a specific timeframe.
Data Preprocessing

- **Cleaning:** We’ll tackle issues like missing values, duplicate entries, and inconsistencies in the data.
Feature Engineering: We'll create useful features that could impact churn, such as how often customers use the service, their average spending, and their interactions with customer support.
Exploratory Data Analysis (EDA)

- **Visualization:**  We’ll use graphs to explore trends and patterns in customer behavior.
Statistical Analysis: This will help us find correlations between different features and churn rates.
Model Selection

- **Algorithms:** We’ll experiment with different machine learning algorithms, including logistic regression and decision trees.

- **Performance Metrics:** To evaluate how well our models perform, we’ll look at metrics like accuracy, precision, recall, and F1-score.

- **Model Training and Validation:** We’ll split our data into training and testing sets.Our models will be trained and validated using cross-validation techniques to ensure their robustness.

- **Implementation:** Once we have a reliable model, we’ll deploy it in a production environment to monitor real-time customer data. We’ll set up alerts or dashboards for stakeholders to easily visualize churn predictions.

- **Strategies for Retention**

- **Targeted Marketing:** Insights from our model will help create personalized marketing campaigns for at-risk customers.

- **Customer Engagement:** We’ll implement feedback mechanisms to enhance overall customer satisfaction.

**Expected Outcomes**

- **Increased Retention Rates:** By proactively addressing churn, businesses can boost customer loyalty and lifetime value.

- **Data-Driven Decisions:** We’ll provide actionable insights for marketing and customer service teams.

- **Enhanced Customer Understanding:** The project will help us gain a deeper understanding of customer needs and behaviors.


## Dataset Overview

- **Columns

- **CustomerID:** A unique identifier for each customer.

- **Name:** The customer’s name.

- **Age:** The customer’s age.

- **Gender:** The customer’s gender.

- **Location:** The city or area where the customer resides.

- **Email:** The customer’s email address.

- **Phone:** The customer’s phone number.

- **Address:** The customer’s postal address.

- **Segment:** The category to which the customer belongs (e.g., Segment A, Segment B, Segment C).

- **PurchaseHistory:** A list detailing the customer’s purchases, including product names, frequency, and value.

- **Product:** Name of the product.

- **Frequency:** How often the product was purchased.

- **Value:** Cost of the product.

- **SubscriptionDetails:** Information about the customer’s subscription plan, including plan name, start date, and end date.

- **Plan:** Name of the subscription plan.

- **StartDate:** When the subscription started.

- **EndDate:** When the subscription ends.

- **ServiceInteractions:** Records of the customer’s interactions with customer service.

- **Type:** Interaction type (e.g., Call, Email, Chat).

- **Date:** Date of the interaction.

- **PaymentHistory:** Details about payment methods and any late payments.

- **Method:** Payment method (e.g., Credit Card, PayPal).

- **LatePayments:** Number of late payments.

- **WebsiteUsage:** Metrics related to the customer’s usage of a website or app, including page views and time spent.

- **PageViews:** Number of pages viewed.

- **TimeSpent:** Time spent on the website (in minutes).

- **ClickstreamData:** Actions taken by the customer on the website, like clicks and searches.

- **Action:** Type of action (e.g., Click, Search, Add to Cart).

- **Page:** Page where the action occurred.

- **Timestamp:** When the action took place.

- **EngagementMetrics:** Metrics related to customer engagement.

- **Logins:** Number of times the customer has logged in.

- **Frequency:** How often the customer logs in (Daily, Weekly, Monthly).

- **Feedback:** Customer feedback, including a rating and comments.

- **Rating:** A score from 1 to 5.

- **Comment:** Customer’s comments on their experience.

- **MarketingCommunication:** History of marketing communications with the customer.

- **EmailSent:** Date when an email was sent.

- **EmailOpened:** Date when the email was opened.

- **EmailClicked:** Date when the email was clicked.

- **NPS:** Net Promoter Score measuring customer loyalty (0 to 10).

- **ChurnLabel:** Indicates whether the customer has churned (1 for churn, 0 for no churn).

- **Timestamp:** When the data was recorded for the customer.

## Feature Enhancement

To improve the performance of our machine learning algorithms, particularly logistic regression and random forest, we will create additional features to better capture customer behaviors and tendencies.

### Conclusion

The analysis of customer churn reveals critical insights based on various predictive models. Below is a structured overview of the models evaluated, including their train, validation, and test scores:

#### Logistic Regression Metrics:

- **Train Accuracy**: 97.1%
- **Train Precision**: 97.7%
- **Train Recall**: 96.6%
- **Train F1 Score**: 97.1%
- **Validation Accuracy**: 96.8%
- **Validation Precision**: 96.4%
- **Validation Recall**: 96.9%
- **Validation F1 Score**: 96.7%
- **Test Accuracy**: 96.9%
- **Test Precision**: 97.3%
- **Test Recall**: 96.4%
- **Test F1 Score**: 96.9%

#### Decision Tree Metrics:

- **Train Accuracy**: 97.7%
- **Train Precision**: 97.8%
- **Train Recall**: 97.7%
- **Train F1 Score**: 97.7%
- **Validation Accuracy**: 96.7%
- **Validation Precision**: 96.2%
- **Validation Recall**: 96.9%
- **Validation F1 Score**: 96.6%
- **Test Accuracy**: 97.3%
- **Test Precision**: 97.4%
- **Test Recall**: 97.3%
- **Test F1 Score**: 97.3%

#### Random Forest Metrics:

- **Train Accuracy**: 99.9%
- **Train Precision**: 100%
- **Train Recall**: 99.9%
- **Train F1 Score**: 99.9%
- **Validation Accuracy**: 96.8%
- **Validation Precision**: 96.4%
- **Validation Recall**: 96.9%
- **Validation F1 Score**: 96.7%
- **Test Accuracy**: 97.36%
- **Test Precision**: 97.36%
- **Test Recall**: 97.36%
- **Test F1 Score**: 97.36%

#### Gradient Boosting Metrics:

- **Train Accuracy**: 97.8%
- **Train Precision**: 97.5%
- **Train Recall**: 97.5%
- **Train F1 Score**: 97.3%
- **Validation Accuracy**: 96.8%
- **Validation Precision**: 96.4%
- **Validation Recall**: 96.9%
- **Validation F1 Score**: 96.7%
- **Test Accuracy**: 97.25%
- **Test Precision**: 97.48%
- **Test Recall**: 97.48%
- **Test F1 Score**: 97.25%

### Observations

1. **Logistic Regression**: This model performs well with high accuracy and precision, though it shows slightly lower recall, indicating it may miss some positive cases which are critical for churn prediction.

2. **Decision Tree**: The decision tree demonstrates a strong balance between complexity and interpretability, achieving solid accuracy and F1 scores. However, it may be prone to overfitting, as evidenced by the high training metrics compared to validation.

3. **Random Forest**: This ensemble model exhibits exceptional performance across all metrics, particularly in training accuracy and precision. Its ability to maintain high validation and test scores highlights its robustness and effectiveness in predicting customer churn.

4. **Gradient Boosting**: This model shows competitive performance, with strong metrics across the board. Its ability to refine predictions from weak learners makes it a valuable option for capturing complex patterns in the data.

### Final Conclusion

In summary, both the Random Forest and Gradient Boosting models demonstrate outstanding performance, making them highly suitable for predicting customer churn. Their high accuracy, precision, and recall indicate their reliability and effectiveness, providing valuable insights for targeted interventions to enhance customer retention. While Logistic Regression and Decision Tree models are effective, they show slightly lower performance metrics. However, they can still serve as useful alternatives based on the need for interpretability and model simplicity. Overall, the insights derived from these models can significantly inform strategies to mitigate churn and improve customer loyalty.