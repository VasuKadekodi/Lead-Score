<h1 align="center"> 📈 Lead-Score Analysis </h1>

<p align="center">
  <img src="https://img.shields.io/github/license/{username}/{repo-name}" alt="License">
  <img src="https://img.shields.io/github/last-commit/{username}/{repo-name}" alt="Last Commit">
  <img src="https://img.shields.io/github/issues/{username}/{repo-name}" alt="Issues">
  <img src="https://img.shields.io/github/stars/{username}/{repo-name}" alt="Stars">
</p>

<p align="center">
  Analysis done for X Education to find ways to get more industry professionals to join their courses. 
</p>

<h2 align="center"> Table of Contents </h2>

<ul>
  <li><a href="#steps-used">Steps Used</a></li>
  <li><a href="#conclusions">Conclusions</a></li>
  <li><a href="#recommendations-to-improve-the-business">Recommendations to Improve the Business</a></li>
  <li><a href="#contact">Contact</a></li>
</ul>

## Steps Used
- Cleaning data: Null values were replaced, irrelevant elements were removed.
- EDA: A quick exploratory data analysis was done.
- Dummy Variables: Created dummy variables and used the MinMax Scaler for numeric values.
- Train-Test split: Split data into training and test sets.
- Model Building: Used Recursive Feature Elimination (RFE) to obtain the top 15 relevant variables and removed rest based on VIF and p-values.
- Model Evaluation: Confusion matrix was used and ROC curve was used to find optimum cut off value for accuracy, sensitivity and specificity.
- Prediction: Test data was used for prediction with an optimum cut off of 0.42.

## Conclusions
The top variables that matter most in potential buyers are (in descending order):
1. Total number of visits
2. The total time spend on the Website
3. Lead Origin_Lead Add Form
4. Last Notable Activity_Unreachable
5. Last Activity_Had a Phone Conversation
6. Lead Source_Welingak Website
7. Lead Source_Olark Chat
8. Last Activity_SMS Sent
9. Do Not Email_Yes
10. What is your current occupation_Student
11. What is your current occupation_Unemployed

## Recommendations to Improve the Business
- Give utmost importance to the top variables while planning to achieve maximum registration/enrollment.
- Design the UI/UX of the website to be more eye-catching, informative and easy to navigate.
- Provide attractive offers/discounts on the home page to entice visitors.

## Contact
Created by [@VasuKadekodi] - feel free to contact me at [vasundharalkadekodi@gmail.com]. 

