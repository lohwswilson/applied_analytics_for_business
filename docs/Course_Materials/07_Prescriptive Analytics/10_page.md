---
title: Introduction to Prescriptive Analytics and its applications
author: [Wilson Loh]
date: 2022-07-11
---

Prescriptive analytics represents the pinnacle of data analytics, leveraging advanced mathematical and statistical techniques to not only analyse data but also provide actionable recommendations for decision-making. Unlike descriptive analytics, which focuses on historical data, or predictive analytics, which forecasts future outcomes, prescriptive analytics takes data analysis to the next level by suggesting the best course of action to achieve desired outcomes. 
Prescriptive analytics involves using models like linear programming, sensitivity analysis, and simulation to make data-driven decisions. In the case of Fandango, these tools enable them to adjust ticket prices hourly based on demand and showtime availability, optimizing profits by identifying the most popular movie times (Asllani, A., 2015). 

<br>
Here's an in-depth look at prescriptive analytics and its applications, along with examples:

- **Retail:** In the retail industry, prescriptive analytics can help optimize inventory management. Suppose a retail chain wants to minimize carrying costs while ensuring products are available to meet customer demand. Prescriptive analytics can factor in historical sales data, seasonal trends, supplier lead times, and cost constraints to recommend reorder quantities, reorder points, and pricing strategies. This enables the business to strike the right balance between inventory costs and customer satisfaction.

- **Finance:** Financial institutions use prescriptive analytics to make investment decisions. For instance, a portfolio management system may utilize prescriptive analytics to recommend an optimal mix of assets based on risk tolerance, market conditions, and return expectations. It considers various investment options and their potential impact on the portfolio's performance to guide investment choices.

- **Healthcare:** In healthcare, prescriptive analytics can assist in treatment recommendations. For instance, a medical decision support system may analyze a patient's medical history, symptoms, lab results, and available treatment options to suggest the most effective treatment plan. It considers factors like treatment efficacy, side effects, and patient preferences to guide healthcare providers.

- **Transportation:** Transportation and logistics companies use prescriptive analytics to optimize routes, schedules, and resource allocation. For instance, a delivery company may employ prescriptive analytics to determine the most efficient delivery routes for its drivers, considering factors like traffic conditions, delivery windows, and vehicle capacities. This ensures timely deliveries while minimizing fuel costs and congestion.

<br>
Prescriptive analytics offers a wide array of benefits that can significantly impact organizations across various industries. Let's explore these benefits in more detail with examples:

<br>

**1.\ Improved Decision-Making:** Amazon's vast product catalogue requires precise inventory management. Prescriptive analytics helps Amazon determine optimal inventory levels for each product, considering factors like demand patterns, seasonality, and storage costs. This ensures that popular items are well-stocked while minimizing overstocking of less in-demand products.

<br>

**2.\ Increased Efficiency:** Example: Walmart optimizes the layout and product placement within its stores using prescriptive analytics. It considers factors such as foot traffic patterns, customer demographics, and product affinity to determine the ideal arrangement of products on store shelves. This not only enhances the shopping experience but also encourages cross-selling and impulse purchases.

<br>

**3.\ Reduced Costs:** UnitedHealthcare utilizes prescriptive analytics to identify patients who are at high risk of being readmitted to the hospital shortly after discharge. By analyzing patient data, including medical history, previous admissions, and clinical indicators, the system can pinpoint individuals at risk. This proactive approach not only lowers healthcare costs for both the insurer and the patient but also leads to better health outcomes by addressing potential issues before they escalate.

<br>

**4.\ Improved Customer Satisfaction:** Netflix employs prescriptive analytics to suggest movies and TV shows to its users. Algorithms analyse viewing history, genre preferences, user ratings, and real-time data on what other users with similar tastes are watching. This ensures that users receive tailored recommendations, keeping them engaged and less likely to cancel their subscriptions.

<br>

In each of these examples, prescriptive analytics doesn't just provide data insights; it offers actionable recommendations that organizations can implement to achieve tangible benefits. It empowers businesses to make informed decisions, streamline operations, cut unnecessary expenses, and enhance customer interactions. Ultimately, the goal of prescriptive analytics is to drive efficiency, cost-effectiveness, and customer satisfaction, leading to improved overall performance and competitiveness (Catherine, 2021).


## Travelling Salesman Problem

The Traveling Salesman Problem (TSP) has intrigued mathematicians for over a century, posing the challenge of finding the perfect route among a multitude of distant locations to minimize costs. Initially, the problem may appear straightforward, but as more locations come into play, its complexity grows exponentially. While it's commonly associated with travel, its applications extend far beyond, encompassing tasks like optimizing circuit board layouts, configuring IT networks, and, unsurprisingly, managing geographic transport logistics. The problem transcends physical distances and can be applied to any quantitative metric within a data matrix, making it versatile.

<br>

The straightforward but impractical approach is to examine every possible order combination, a technique known as the Brute Force method. However, with just 10 locations, this demands approximately 360,000 iterations, escalating to a staggering 121 million billion for 20 locations. 

<br>

The Nearest Neighbour approach, the next logical step, involves selecting the closest location sequentially, but it often falls short of finding the shortest route since it doesn't consider the holistic spatial relationships. Over time, more heuristic methods have emerged, with the Branch and Bound method standing out as arguably the most efficient. This method employs a tree-based structure, generating binary branches of location pairs to either include or exclude from the final solution, continually expanding with new pairs and locations.

<br>
Despite significant advancements, there's no universally efficient algorithm to solve the TSP for all scenarios. In fact, a substantial reward of 1 million dollars awaits anyone who can devise such an algorithm.

## Prescriptive Analytics Approach
Prescriptive analytics is complex that need investment, skills and tools. Below is the approach for company to kick-off their prescriptive analytics for their business problem (infoutkarsh, n.d) :

1.	**Data Collection:** The initial phase involves gathering data from various sources, encompassing customer locations, their specific needs, information about company warehouses, and transportation details.
2.	**Mathematical Formulation:** In this step, we craft mathematical models that effectively handle supply chain data, including variables such as customer location, time, warehouse locations, and transportation routes. Simultaneously, we define an optimization function geared towards minimizing company costs and reducing delivery times.
3.	**Optimization Process:** Leveraging optimization methodologies like linear programming or differential calculus, we tackle the mathematical models to pinpoint optimal locations and configurations.
4.	**Scenario Assessment:** To ensure robustness, we subject the models to scenario analysis, exploring various assumptions and variables to gauge their impact on the outcomes.
5.	**Decision Support:** Drawing from our data modeling efforts and the business insights derived from raw data, we construct informative dashboards and visual representations. These aids empower stakeholders in making well-informed decisions.
6.	**Implementation:** The ultimate and pivotal stage involves implementing the prescribed changes, with a focus on maximizing the company's revenue streams, thus bringing the entire process to fruition.


