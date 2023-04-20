<h1 align="center"> # 📈 Lead Score Analysis for X Education 🎓 </h1>


This analysis was conducted to help X Education increase their enrollment by finding ways to attract more industry professionals to their courses. The provided data gave us insights into how potential customers visit the site, the time they spend there, how they reach the site, and the conversion rate.

## Table of Contents
* [Steps Used](#steps-used)
* [Conclusions](#conclusions)
* [Recommendations](#recommendations)
* [Contact](#contact)

## Steps Used

#### - Cleaning Data 🧹
The data was partially clean, but a few null values had to be handled, and the "Select" option was replaced with a null value since it did not provide much information. Some null values were changed to "not provided" to avoid losing too much data, although they were later removed when creating dummy variables. Since there were many entries from India and few from outside, the elements were grouped into "India", "Outside India", and "not provided".

#### - EDA 📊
A quick exploratory data analysis was performed to check the condition of the data. It was found that many elements in the categorical variables were irrelevant, while the numeric values seemed good and had no outliers.

#### - Dummy Variables 🤖
Dummy variables were created, and dummies with "not provided" elements were removed. For numeric values, the MinMax Scaler was used.

#### - Train-Test Split 🚂🧪
The data was split into 70% for training and 30% for testing.

#### - Model Building 🏗️
Firstly, RFE was used to obtain the top 15 relevant variables. Later, the rest of the variables were manually removed depending on the VIF values and p-value (keeping variables with VIF < 5 and p-value < 0.05).

#### - Model Evaluation 📈
A confusion matrix was created, and the optimum cutoff value (using the ROC curve) was used to find accuracy, sensitivity, and specificity, which were all around 80%.

#### - Prediction 🤖
Predictions were made on the test data frame, and an optimum cutoff of 0.42 was used with accuracy of 78%, precision around 77%, and recall around 78%.

## Conclusions 📊📉
We found that the variables that mattered the most for potential buyers were (in descending order):
1. Total number of visits
2. Total time spent on the website
3. Lead Origin_Lead Add Form
4. Last Notable Activity_Unreachable
5. Last Activity_Had a Phone Conversation
6. Lead Source_Welingak Website
7. Lead Source_Olark Chat
8. Last Activity_SMS Sent
9. Do Not Email_Yes
10. What is your current occupation_Student
11. What is your current occupation_Unemployed

## Recommendations 🚀
- We recommend giving utmost importance to the above variables while planning to achieve maximum registration/enrollment to X Education.
- As total number of visits and total time spent on the website have a very positive impact on enrollment, we recommend designing a UI/UX of the website that is easy, eye-catching, and informative about the courses.
- It is also recommended to provide attractive offers/discounts on the home page to pique visitors' curiosity and encourage them to learn more.

## Contact 📧
Created by [@VasundharaLK](https://github.com/VasundharaLK) 💻
For any questions or feedback, feel free to reach
