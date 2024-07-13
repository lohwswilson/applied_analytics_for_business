---
title: Techniques for Optimization and Decision Modeling
author: [Wilson Loh]
date: 2022-05-01
---

## Optimization

To address operational challenges like route optimization and logistics planning, business analysts have historically employed optimization techniques. However, recent technological advancements have ushered in a new era of decision support analytics through optimization. These modern optimization models can tackle larger, enterprise-wide problems and facilitate comprehensive what-if analyses. They amalgamate the entire value chain, including crucial constraints, with financial aspects, providing superior insights compared to single predictive or business intelligence models. Additionally, they ensure data consistency within the organization and identify unfeasible outcomes. These models support specialized analyses such as contribution margin assessment, activity-based costing, and the creation of Pro-forma financial statements, aiding users in making optimal business decisions.

<br>
Optimization primarily serves as a solution for intricate problems characterized by a multitude of constraints, objectives, and trade-offs, often exceeding 20 in number. The application of prescriptive analytics through optimization empowers users to navigate this complexity and identify the most favourable path while aligning with defined business objectives.
The mathematical algorithms underpinning optimization are notably intricate. What's crucial to understand is that they employ mathematical techniques to either maximize or minimize one or more objective functions while adhering to real-world business constraints, consistently yielding feasible plans.

## Linear Programming

Linear programming (LP) is a potent mathematical technique widely employed in the realm of business analytics to enhance the efficiency of decision-making processes. Its exceptional utility shines when an organization confronts the challenge of allocating finite resources across competing tasks to attain a set objective while navigating a spectrum of constraints. 
Let's delve into the fundamental elements of linear programming and delve into instances of its practical application in the sphere of business analytics.
Key Components of Linear Programming:

1.	**Objective Function:**
    
    - Definition: In linear programming, the objective function represents the primary goal or objective of a business problem. It's a mathematical expression that must be either maximized or minimized. The objective could involve maximizing profits, minimizing costs, or optimizing resource utilization.
    
    - Example: Imagine a manufacturing company that produces two products, A and B, with a goal to maximize profit. Product A yields a profit of $10 per unit, and product B yields $15 per unit. The objective function to maximize profit (P) can be formulated as:
        
        <br>
        P = 10x₁ + 15x₂

        <br>
        Here, x₁ represents the quantity of product A to produce, and x₂ represents the quantity of product B to produce.

2.	**Decision Variables:**

    - Definition: Decision variables are the unknown parameters or choices that a business needs to determine as part of its decision-making process. These variables represent the quantities or actions under consideration.
    - Example: In the manufacturing context, the decision variables are x₁ and x₂, which signify the quantities of products A and B to manufacture, respectively.

3.	**Constraints:**

    - Definition: Constraints in LP are the real-world limitations or conditions that restrict the values of decision variables. Constraints must be satisfied for the problem to have a feasible solution.

    - Example: Let's introduce constraints into our manufacturing scenario:

        1. The production capacity of a machine limits the total production of A and B to 100 units:
         
                
                x₁ + x₂ ≤ 100
            
         
        2. Availability of raw materials restricts the production of A to no more than 60 units:
                      
                x₁ ≤ 60

        3. There is a minimum production requirement for B, set at 20 units:
            
                x₂ ≥ 20

4.	**Feasible Region:**
    - Definition: The feasible region is the set of all valid combinations of decision variable values that satisfy all the constraints simultaneously. It defines the region within which the optimal solution must be located.

    - Example: In our manufacturing case, the feasible region is the overlap or intersection of the areas defined by the constraints in the x₁-x₂ plane. It includes all valid combinations that meet the capacity, material, and production requirements.

5.	**Optimization:**

    - Definition: Optimization is the central aspect of linear programming. It involves determining the values of decision variables that either maximize or minimize the objective function while staying within the feasible region.
    - Example: Solving our manufacturing LP problem will yield values for x₁ and x₂ that maximize profit (P) while adhering to all the constraints. For instance, the solution could be x₁ = 60 and x₂ = 40, leading to an optimal profit of $1,400.

6.	**Solution Interpretation:**

    - Definition: After solving the LP problem, the results need to be interpreted within the context of the business problem. Decision-makers must understand the implications of the optimal values of decision variables for the organization.
    - Example: In our manufacturing example, interpreting the solution means recognizing that to maximize profit, the company should produce 60 units of product A and 40 units of product B, resulting in a total profit of $1,400.

These elements are the foundation of linear programming, a versatile tool that empowers organizations to make informed, data-driven decisions. By systematically defining objectives, decision variables, constraints, and the objective function, businesses can optimize resource allocation and achieve specific goals efficiently (Analytics Vidhya, 2017).


### The Linear Programming Workflow:

**1.\ Formulation:** At the outset, the business outlines the objective function, decision variables, and constraints in consonance with the specific problem it seeks to unravel.

<br>

**2.\ Mathematical Modelling:** Armed with the blueprint of the objective function and constraints, the problem metamorphoses into a mathematical construct articulated as an assembly of linear equations or inequalities.

<br>

**3.\ Optimization:** Linear programming takes centre stage as it leverages algorithms to ascertain the optimal values of the decision variables. The objective here is to maximize or minimize the objective function while honouring all constraints. Myriad methods such as the simplex method or the graphical method can be employed to untangle LP conundrums.

<br>

**4.\ Solution Interpretation:** Upon arriving at a solution, the results are dissected within the context of the business predicament. This involves unravelling the optimal values of decision variables and gauging their impact on the objective function.

### Applications of Linear Programming in Business Analytics:
- **Production Planning:** Consider a manufacturing enterprise endeavouring to ascertain the optimal production volumes for its array of products to maximize profit. This intricate endeavour is tackled while grappling with constraints such as limited machine availability and raw material constraints.

- **Inventory Management:** A retailer embarks on an odyssey to minimize inventory holding costs while ensuring an adequate stockpile to meet customer demand. LP lends a hand in optimizing reorder quantities and the frequency of orders.
  
- **Transportation and Logistics:** Shipping juggernauts harness LP to streamline transportation routes and optimize cargo distribution. This endeavour helps curtail fuel expenditure and slash delivery times.

- **Media Planning:** An advertising agency strategically deploys its budget across diverse advertising channels to maximize the reach and efficacy of an advertising campaign. All the while, stringent budget constraints are strictly adhered to.

- **5. Resource Allocation:** Project managers don the hat of resource allocators, allocating limited resources such as labour, equipment, and funds across a constellation of projects. The goal is to maximize the overall return on investment while navigating the constraints imposed by resource availability.

- **6. Financial Portfolio Optimization:** Savvy investors employ LP to divvy up their investment capital among a constellation of assets to optimize returns while prudently managing risk constraints.

<br>
In each of these illustrative scenarios, linear programming unfurls its banner as an enabler of data-informed verdicts, meticulously fine-tuning resource allotment, and propelling organizations towards their designated objectives. This profound analytical tool augments decision-making, bestowing businesses with a competitive edge and bolstering overall operational excellence.
