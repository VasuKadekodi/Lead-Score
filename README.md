# Lead-Score
This analysis is done for X Education and to find ways to get more industry professionals to join their courses. The basic data provided gave us a lot of information about how the potential customers visit the site, the time they spend there, how they reached the site and the conversion rate. 

## Table of Contents
* [Steps Used](#Steps Used)
* [Conclusions](#conclusions)
* [Recommendations to improve the business](#recommendations-to-improve-the-business)

## Steps Used
### - Cleaning data: 
The data was partially clean except for a few null values and the option select had to be replaced with a null value since it did not give us much information. Few of the null values were changed to ‘not provided’ so as to not lose much data. Although they were later removed while making dummies. Since there were many from India and few from outside, the elements were changed to ‘India’, ‘Outside India’ and ‘not provided’. 

### - EDA: 
A quick EDA was done to check the condition of our data. It was found that a lot of elements in the categorical variables were irrelevant. The numeric values seems good and no outliers were found. 

### - Dummy Variables: 
The dummy variables were created and later on the dummies with ‘not provided’ elements were removed. For numeric values we used the MinMax Scaler. 

### - Train-Test split: 
The split was done at 70% and 30% for train and test data respectively. 

### - Model Building: 
Firstly, RFE was done to attain the top 15 relevant variables. Later the rest of the variables were removed manually depending on the VIF values and p-value (The variables with VIF < 5 and p-value < 0.05 were kept). 

### - Model Evaluation: 
A confusion matrix was made. Later on the optimum cut off value (using ROC curve) was used to find the accuracy, sensitivity and specificity which came to be around 80% each. 

### - Prediction: 
Prediction was done on the test data frame and with an optimum cut off as 0.42 with accuracy78% Precision around 77% and recall around 78% on the test data frame. 

## Conclusions
It was found that the variables that mattered the most in the potential buyers are (In descending order) :

1. Total number of visits.
2. The total time spend on the Website.
3. Lead Origin_Lead Add Form.
4. Last Notable Activity_Unreachable.
5. Last Activity_Had a Phone Conversation.
6. Lead Source_Welingak Website.
7. Lead Source_Olark Chat.
8. Last Activity_SMS Sent.
9. Do Not Email_Yes.
10. What is your current occupation_Student.
11. What is your current occupation_Unemployed.

## Recommendations to improve the business
- It is recommended to give utmost importance to the above variables while planning to achieve maximum registration/enrolment to the X Education.
- As we can see Total number of visits and The total time spend on the Website are having very positive impact on the enrolment, we recommend to design UI/UX of the website more easy, eye catching and informative about the course.
- And it is recommended to provide some attractive offers/discounts in the home page so that visitors will be curious to know more.

## Created by [@VasundharaLK]
For contact - vasundharalkadekodi@gmail.com 

