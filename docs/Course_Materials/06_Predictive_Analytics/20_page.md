---
title: Understanding Predictive Modeling Techniques
author: [Wilson Loh]
date: 2022-05-01
---


Predictive models encompass mathematical equations and algorithms employed for forecasting future outcomes, including events like customer attrition or sales performance.

Various predictive modelling techniques are at one's disposal, each suited to particular scenarios:

- Regression
- Decision trees
- Neural networks (A subset of machine learning and pivotal in generative AI tools like ChatGPT)
- Random forests
- K-means clustering
- K-nearest neighbors (k-NN)
- Autoregressive integrated moving average (ARIMA)


## Regression Analysis


One valuable tool within the realm of predictive analytics is regression analysis, a technique capable of unveiling relationships between variables. Whether it's exploring the connection between two variables (single linear regression) or examining the impact of three or more variables (multiple regression), regression analysis can represent these relationships through mathematical equations. These equations become powerful instruments for predicting outcomes when one of the variables undergoes a change.

<br>
Harvard Business School Professor Jan Hammond, who instructs the online course Business Analytics, a pivotal component of the Credential of Readiness (CORe) program, highlights the significance of regression. She states that regression analysis not only offers insights into the nature of these relationships but also provides measures of how well the data align with these relationships. These insights are exceptionally valuable when scrutinizing historical trends and crafting forecasts that can inform strategic decision-making (What Is Predictive Analytics? 5 Examples | HBS Online, 2021).

<br>
Forecasting, driven by predictive analytics, equips organizations with the ability to make more informed decisions and develop data-driven strategies. To illustrate the practical utility of predictive analytics, here are several real-world examples that can inspire you to leverage this approach within your own organization.

<br>
Numerous regression algorithms are available, each tailored to different data types and modeling requirements. Some of the most widely used regression algorithms encompass:

- **Linear Regression:** A fundamental approach that establishes a linear relationship between variables.
- **Logistic Regression:** Ideal for binary classification tasks where the outcome is categorical.
- **Polynomial Regression:** Useful for modeling nonlinear relationships by incorporating polynomial terms.
- **Support Vector Regression:** Incorporates support vector machine principles for regression tasks.
- **Decision Tree Regression:** Utilizes decision tree structures to represent complex relationships.

### Linear Regression

Regression in data analytics is a statistical technique that plays a crucial role in modelling the relationship between one or more independent variables and a dependent variable. Its primary objective is to establish a functional form that effectively characterizes the association between these variables, enabling the prediction of the dependent variable's value based on the values of the independent variables.

<br>
Regression analysis operates within the framework of supervised learning, meaning it relies on labelled data for training. In this training phase, each data point provides information about both the dependent and independent variables. Subsequently, once the model is adequately trained, it becomes capable of forecasting the dependent variable's values for new data points, where only the independent variables are known.

<br>
Regression analysis finds extensive applications across various industries and fields, making it an indispensable tool in data mining and machine learning. For instance, regression can be employed to:

<br>
**1.\ Predict Future Sales:** In retail, historical sales data and additional factors like marketing expenditures, economic indicators, and competitor activity can be utilized to create a regression model that predicts future sales trends.

<br>
**2.\	Forecast Customer Demand:** Businesses can anticipate customer demand by analysing historical demand patterns alongside variables such as promotions, seasonal trends, and market conditions.

<br>
**3.\	Identify Influencing Factors on Customer Satisfaction:** By examining customer satisfaction scores in relation to various factors like product quality, customer support, and pricing, regression can uncover the most influential drivers.

<br>
**4.\	Evaluate Marketing Campaign Impact:** Regression helps assess the effectiveness of marketing efforts by correlating campaign metrics (e.g., ad spend, impressions) with outcomes such as sales or website traffic.

<br>
**5.\	Develop Pricing Models:** Companies can optimize pricing strategies by considering factors like production costs, competitor prices, and customer demand using regression models.


The selection of the most appropriate regression algorithm hinges on the specific problem at hand and the characteristics of the data. To illustrate, consider a marketing firm aiming to predict future sales. By leveraging historical sales records alongside data on marketing expenditures, economic conditions, and competitors' actions, a regression model can be trained. This model can subsequently forecast sales for upcoming periods, aiding the company in making informed decisions regarding budget allocation, marketing strategies, and other business activities. In essence, regression serves as a versatile and indispensable tool in data analytics, providing insights and predictions across a broad spectrum of real-world challenges where relationships between variables exist.

### Steps in Regression Analysis

Let's delve into an illustrative instance of employing regression analysis for analytics, focusing on predicting housing prices by considering various influencing factors.
<br>
Problem Statement: Consider a scenario where a real estate agency aspires to forecast the selling prices of homes within a specific neighbourhood. They have meticulously accumulated a dataset encompassing recent property sales, encompassing attributes such as the number of bedrooms, square footage, the presence of a garage, and the proximity to the nearest school. The agency's core objective is to construct a regression model capable of estimating a house's selling price predicated on these distinctive attributes.


#### Stages in Regression Analysis:

- **1. Data Gathering:** The initial phase entails collecting data on recent property transactions within the target locale. The dataset is replete with particulars pertaining to each property's unique characteristics, serving as independent variables, along with the actual sale prices, serving as the dependent variable.

- **2. Data Pre-processing:** Before commencing regression analysis, meticulous data preparation is indispensable. This may necessitate addressing data anomalies such as missing values or outliers. Additionally, categorical variables, like the "presence of a garage," might necessitate transformation into numerical representations, a process often facilitated by techniques such as one-hot encoding.


- **3. Data Splitting:** The dataset undergoes a bifurcation into two subsets: a training set and a testing set. The training set plays a pivotal role in training the regression model, while the testing set remains reserved for scrutinizing the model's predictive prowess.

- **4. Model Selection:** The agency judiciously selects a regression algorithm that aligns with the specific task at hand. In this particular case, they opt for multiple linear regression, a fitting choice given its adeptness at forecasting a continuous target variable (in this context, the selling price) by considering multiple independent features.

- **5. Model Training:** Subsequently, the multiple linear regression model undergoes training with the employment of the training dataset. During this phase, the model acquires insights into the intricate relationships existing between the independent variables (e.g., bedroom count, square footage) and the dependent variable (selling price).

- **6. Model Assessment:** To gauge the model's performance, a slew of evaluation metrics tailored to regression tasks come into play. Common metrics encompass mean squared error (MSE), root mean squared error (RMSE), and R-squared (the coefficient of determination), offering an indication of how effectively the model accounts for data variance.

- **7. Prediction:** Armed with the trained and evaluated regression model, the real estate agency is poised to generate predictions. For a novel property listing, the agency inputs the pertinent property attributes (independent variables) into the model, which, in turn, furnishes an estimated selling price (the dependent variable).

- **8. Refinement:** Depending on the outcomes of the evaluation, the agency may embark on model fine-tuning endeavours. This could entail the adjustment of hyperparameters or the exploration of feature engineering methodologies, all in pursuit of enhancing the model's predictive accuracy and utility.

<br>
By adhering to these meticulous steps, the real estate agency ultimately forges a robust regression model, thereby arming itself with the capability to appraise housing prices for prospective listings within the neighbourhood. This predictive capacity not only benefits prospective buyers but also empowers sellers with the insight needed to make judicious decisions regarding real estate transactions in an informed and data-driven manner.

### Regression in Business World

According to Redman, regression analysis is a fundamental and widely-used method in analytics that smart companies rely on for making informed decisions across various business challenges. Companies typically employ regression analysis to achieve three primary objectives: first, to elucidate and understand a phenomenon (e.g., explaining the drop in customer service calls); second, to make predictions about the future (e.g., forecasting sales trends over the next six months); and third, to make decisions (e.g., choosing between different promotional strategies). However, it's important to note the cautionary principle that "correlation is not causation" when using regression or similar analyses. Just because two factors are correlated doesn't necessarily imply a cause-and-effect relationship. For instance, while rain and monthly sales may be correlated, asserting that rain directly causes increased sales could be challenging to substantiate unless it's a product like umbrellas being sold (Amy Gallo, 2015).

## Classification

Classification is a data analysis process wherein information is organized into discrete categories based on specific characteristics or attributes. This method is employed to facilitate a clearer understanding of datasets by grouping related data points together. For instance, in email filtering, classification can be used to categorize incoming emails as either "spam" or "not spam" based on features such as keywords, sender information, and message content.

<br>
Similarly, in medical diagnosis, classification algorithms can categorize patient records into different disease classes based on various clinical parameters, aiding doctors in making accurate diagnoses. In the context of predictive analytics, supervised machine learning models are often used for classification tasks, enabling automated decision-making based on data patterns. These models, through training on labelled examples, learn to distinguish between different categories and can then classify new, unseen data accordingly, making classification a valuable tool for various applications in data analysis and decision-making processes.

<br>
The practical applications of classification span a multitude of industries and problem-solving domains, rendering valuable insights and streamlining processes. Here are notable instances:

<br>

**1.	Marketing:** In marketing, classification facilitates customer segmentation, relying on diverse factors like demographics, purchase history, and online behaviour. For instance, an e-commerce platform might classify customers as "frequent shoppers," "occasional buyers," or "inactive users," enabling targeted marketing campaigns tailored to each group's preferences and behaviours.

<br>

**2.	Fraud Detection:** In the financial sector, classification aids in distinguishing fraudulent transactions from legitimate ones. By scrutinizing historical data encompassing both fraudulent and valid transactions, classification models can promptly flag suspicious activities, contributing to the prevention of financial losses and the safeguarding of consumers.

<br>

**3.	Medical Diagnosis:** Healthcare relies on classification for disease diagnosis. Medical practitioners input patient data encompassing symptoms, medical history, and diagnostic tests into a classification model. The model, in turn, categorizes patients into distinct disease categories, facilitating precise diagnoses and treatment recommendations.

<br>

**4.	Image Recognition:** Classification serves as a linchpin in image recognition tasks. For example, in autonomous vehicles, cameras categorize objects on the road into classes such as "pedestrian," "vehicle," or "traffic sign." This information is critical for real-time decision-making and road safety.

<br>

**5.	Natural Language Processing (NLP):** Within NLP, classification comes to the fore for text categorization. An email system, for instance, can classify incoming emails as "spam" or "not spam" based on content and characteristics, thereby enhancing email filtering.

<br>
_To illustrate, let's delve into a pragmatic scenario employing classification in data analytics:_

<br>
Scenario: An e-commerce platform endeavors to mitigate customer churn, which refers to the rate at which customers cancel their subscriptions. The company aggregates customer data, including attributes like age, contract duration, customer service interactions, and payment history. Each customer is designated as either "churned" or "not churned" based on historical records.

<br>
Application: Utilizing this dataset, the e-commerce platform leverages classification to construct a predictive model. This model, trained on the labeled data, becomes adept at evaluating the likelihood of churn for new customers. For instance, it can prognosticate that a newly acquired customer possesses a high probability of churning in the immediate future.

<br>
Utilization: Empowered with this predictive capability, the company can proactively target at-risk customers with tailored retention strategies. This may encompass incentives, personalized offers, or heightened customer support, all geared towards diminishing churn rates and elevating customer loyalty.

<br>
In summation, classification stands as a versatile and indispensable asset in the realm of data analytics. It empowers automated decision-making, the discernment of patterns, and adept problem-solving across multifarious domains. Whether the challenge at hand revolves around customer segmentation, fraud detection, medical diagnosis, image recognition, or text categorization, classification equips data analysts and machine learning practitioners to glean actionable insights and navigate the data landscape effectively (Rounak Sharma, 2023).

## K-Nearest Neighbors (K-NN)

K-Nearest Neighbors (K-NN) is a simple, non-parametric, and lazy learning algorithm used for classification and regression. In both cases, the input consists of the k closest training examples in the feature space.

### Key Concepts

1. **Non-parametric**: K-NN does not assume a specific form for the underlying data distribution.
2. **Lazy learning**: It does not involve any training phase and computes the results only when a query is made.
3. **Distance metric**: Determines how to measure the similarity between instances. Common metrics include Euclidean distance, Manhattan distance, and Minkowski distance.

### How K-NN Works

1. **Choose the number of neighbors \( k \)**:
:    \( k \) is the number of nearest neighbors to consider.
:    \( k \) is typically an odd number to avoid ties in classification.

2. **Calculate the distance**:
:   - Compute the distance between the query point and all the points in the training set using a chosen distance metric.

3. **Identify the nearest neighbors**:
:   - Sort all the distances and pick the k smallest ones.

4. **Classification/Regression**:
:   - **Classification**: Assign the class label that is most frequent among the k nearest neighbors.
:   - **Regression**: Average the values of the k nearest neighbors to predict the output.

### Example: K-NN for Classification

Let's say we have a dataset of fruits characterized by their weight and color. We want to classify a new fruit based on these features.

#### Dataset

| Fruit  | Weight (g) | Color (scale: 1 to 5) | Class  |
| ------ | ---------- | --------------------- | ------ |
| Apple  | 150        | 3                     | Apple  |
| Orange | 160        | 4                     | Orange |
| Lemon  | 120        | 2                     | Lemon  |
| Banana | 110        | 5                     | Banana |
| Apple  | 140        | 3                     | Apple  |
| Orange | 170        | 4                     | Orange |
| Lemon  | 130        | 2                     | Lemon  |

#### New Fruit

- **Weight**: 145 g
- **Color**: 3

#### Steps

1. **Choose k**: Let's choose \( k = 3 \).

2. **Calculate distances**: Using Euclidean distance:
    
    \[ \text{Distance} = \sqrt{(x_1 - x_2)^2 + (y_1 - y_2)^2} \]

    For each fruit in the dataset:

    \[\begin{align*}
     \text{Distance to Apple (150, 3)} & = \sqrt{(150 - 145)^2 + (3 - 3)^2} = 5 \\
     \text{Distance to Orange (160, 4)} & = \sqrt{(160 - 145)^2 + (4 - 3)^2} = \sqrt{225 + 1} = \sqrt{226} \approx 15.03 \\
     \text{Distance to Lemon (120, 2)} & = \sqrt{(120 - 145)^2 + (2 - 3)^2} = \sqrt{625 + 1} = \sqrt{626} \approx 25.02 \\
     \text{Distance to Banana (110, 5)} & = \sqrt{(110 - 145)^2 + (5 - 3)^2} = \sqrt{1225 + 4} = \sqrt{1229} \approx 35.07 \\
     \text{Distance to Apple (140, 3)} & = \sqrt{(140 - 145)^2 + (3 - 3)^2} = 5 \\
     \text{Distance to Orange (170, 4)} & = \sqrt{(170 - 145)^2 + (4 - 3)^2} = \sqrt{625 + 1} = \sqrt{626} \approx 25.02 \\
     \text{Distance to Lemon (130, 2)} & = \sqrt{(130 - 145)^2 + (2 - 3)^2} = \sqrt{225 + 1} = \sqrt{226} \approx 15.03 \\
     \end{align*}
     \]

1. **Identify the nearest neighbors**:
   - The three nearest neighbors are:
     - Apple (150, 3) with distance 5
     - Apple (140, 3) with distance 5
     - Orange (160, 4) with distance ≈ 15.03

2. **Classify**:
   - The majority class among the nearest neighbors is "Apple".

Thus, the new fruit is classified as an **Apple**.

### Choosing the Right k

- A small \( k \) might be sensitive to noise in the dataset.
- A large \( k \) might smooth out the boundary between classes too much.

### Applications of K-NN

1. **Image Recognition**: K-NN can classify images based on pixel intensity features.
2. **Recommendation Systems**: It can recommend items based on user similarity.
3. **Anomaly Detection**: It can identify anomalies by comparing new instances to known ones.
4. **Medical Diagnosis**: K-NN can classify medical conditions based on patient history and symptoms.

### Advantages and Disadvantages

**Advantages**:
- Simple to understand and implement.
- No training phase (useful for small datasets).

**Disadvantages**:
- Computationally expensive as it stores all training data.
- Performance degrades with large datasets.
- Sensitive to irrelevant or redundant features.

K-NN is a foundational algorithm in machine learning that is intuitive and easy to implement, making it a useful tool for many basic classification and regression tasks.