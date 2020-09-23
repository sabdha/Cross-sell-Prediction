## Cross-sell-Prediction
 To predict, whether the customer would be interested in Vehicle insurance.  
This is an analyticsvidhya hackathon conducted from 11-09-2020 11:59 PM to 20-09-2020 11:59 PM.  
Our private score was 32 with an accuracy of 0.863422  

Algorithm: Catboost  
Feature Engineering: Label encoding   
Hyper parameter Tuning: classweight balancing   

##Problem Statement:

Building a model to predict whether a customer would be interested in Vehicle Insurance is  
extremely helpful for the company to plan its communication strategy to reach out to those customers  
and optimise its business model and revenue. In order to predict, whether the customer would be interested  
in Vehicle insurance, you have information about demographics(gender, age, region code type), Vehicles (Vehicle Age, Damage),  
Policy (Premium, sourcing channel) etc.(Lines from Analyticsvidhya problem statement)  

##train.csv
(Lines from Analyticsvidhya Data Description)  
Variable	Definition  
id:	Unique ID for the customer  
Gender:	Gender of the customer  
Age: Age of the customer  
Driving_License-- 0 : Customer does not have DL, 1 : Customer already has DL  
Region_Code:	Unique code for the region of the customer  
Previously_Insured--	1 : Customer already has Vehicle Insurance, 0 : Customer doesn't have Vehicle Insurance  
Vehicle_Age:	Age of the Vehicle   
Vehicle_Damage  
1 : Customer got his/her vehicle damaged in the past.  
0 : Customer didn't get his/her vehicle damaged in the past.  
Annual_Premium:	The amount customer needs to pay as premium in the year  
Policy_Sales_Channel:	Anonymised Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.  
Vintage:	Number of Days, Customer has been associated with the company  
Response	1 :  Customer is interested, 0 : Customer is not interested  

##test.csv  
Variable	Definition  
id:	Unique ID for the customer  
Gender:	Gender of the customer  
Age:Age of the customer 
Driving_License-	0 : Customer does not have DL, 1 : Customer already has DL  
Region_Code:	Unique code for the region of the customer  
Previously_Insured-	1 : Customer already has Vehicle Insurance, 0 : Customer doesn't have Vehicle Insurance  
Vehicle_Age:	Age of the Vehicle   
Vehicle_Damage  
1 : Customer got his/her vehicle damaged in the past.  
0 : Customer didn't get his/her vehicle damaged in the past.  
Annual_Premium:	The amount customer needs to pay as premium in the year  
Policy_Sales_Channel:	Anonymised Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.  
Vintage:	Number of Days, Customer has been associated with the company  

##sample_submission.csv  
Variable	Definition  
id:	Unique ID  
Response:	Probability of Customer being interested in Vehicle Loan  
