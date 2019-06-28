# Maximizing the Opportunity to be Hired

By Beverly Huang

### Business Understanding
As a marketplace connecting freelance labor with local demand, the company is not only building a digital supply chain network, but also creating a reliable ecosystem in your local community. Thus, to increase the supply chain sustainability, we need to increase the success in the matching process - allowing consumers to find immediate help and allowing taskers to be selected more frequently. Currently, whenever a Client searches for Taskers, the customer will be given a recommendation of up to 15 Taskers from which the Client can choose one to book. In this project, I want to understand what makes a Client choose a tasker, and thus how can a Tasker maximize the opportunity to be hired.

### Data Preparation
The sample dataset contains information about "recommendations". For each recommendation, the position of the Tasker in the recommendation set, the hourly rate for the Tasker when they were shown, the number of Tasks the Tasker had completed in that category, whether the Tasker was hired or not, and the category of work the Client needs help with are collected. Since every recommendation has 1 “hired” and 14 “not hired”, the dataset is highly imbalanced. This will cause bias in the classification model. To solve this problem, I oversampled the minority class by duplicating “hired” entries 14 times.

### Model Deployment: Conclusion for Management
This project uses furniture assembly category as an example to understand what makes a Client choose a tasker, and thus how can a Tasker maximize the opportunity to be hired. The same method can be applied to the other two categories.
From both correlation heat map and feature importance, I found that position is the most important feature in determining the hiring decision. Hourly rate and Number of Tasks Completed are also correlated with the hiring decision.
Using the Random Forest and Auto ML model, we can accurately predict whether the tasker would be
  hired. Combining with Neural Network model, we can even calculate the probability of being hired of each tasker. This model can be used to suggest taskers on hourly rate. the company can even launch an intelligent recommendation tool based on this model to suggest hourly rate for each tasker.
Finally, for position, this is out of the tasker’s control. However, it can be a leverage for the company. the company can create tier program to segment taskers and launch a new campaign based on that.
