# The Multiplier Effect: Gamma GLM Modeling for Medical Insurance

### Objective
The goal of this project is to analyze the primary cost drivers of medical insurance charges. Using Generalized Linear Models, I aimed to move beyond simple linear trends and capture the complex, multiplicative way that risk factors such as smoking and high BMI actually interact to drive up healthcare costs.

### The Problem
In insurance pricing, risk is rarely additive. For example, being an older adult adds a certain cost, and smoking adds another. However, when an individual is both older and a smoker, the cost doesn't just "add up" but instead it snowballs. Standard linear regression often fails to capture this exponential behavior, leading to inaccurate premium pricing and under-reserved risk pools.

### Methodology
* Data Source: Comprehensive medical insurance dataset including age, BMI, smoking status, and regional factors.
* Gamma Generalized Linear Model: Medical charge data is heavily right-skewed and non-negative. I utilized a Gamma distribution with a log-link function to ensure the model respected these statistical boundaries.
    * Multiplicative Interactions:The log-link function allows the model to treat risk factors as multipliers rather than flat additions, which better mirrors real-world actuarial tables.
* Comparative Risk Scenarios: Developed a predictive framework to compare "Healthy Youth" vs. "High-Risk Adult" scenarios to visualize the cost disparity.



### Key Findings
* The Smoking Catalyst: Smoking was identified as the single most significant driver of cost. For a 40-year-old with an average BMI, smoking alone increased predicted annual charges from ~$6,800 to ~$28,000.
* Compounding Risks: The model proved that high BMI acts as a "multiplier" for age. Every year of aging becomes significantly more expensive for individuals in the high-BMI category compared to those in the healthy-weight category.
* Actuarial Application: This project demonstrates the necessity of using non-linear models for pricing. By identifying where costs "snowball," insurance providers can set more accurate premiums and develop targeted wellness incentives.

