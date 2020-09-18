# Predicting NetPromoterScore-NPS-Manipal_hospital

The primary objective of this project was to improve the overall experience of the patients at Manipal Hospitals as Customer service was being key to sustaining sales, client loyalty and profits. It is important for every organization to know what their customers tell others about the organization.Thus they introduced the concept of “Net Promoter score” which is based on single question: How likely is that you recommend this company or product/service to a friend/colleague? The initiative was to collect data in structured manner and translate into meaningful information which could be viewed real time on a Business Intelligence platform.

# Data 
The dataset consists of variables representing Patient information like basic info and Demographics and their responses each department wise survey for Patient satisfaction. The questionnaire has response levels from 1 to 4 with 1 being Extremely satified and 4 being Not at all satisfied. Departments include Nursing services, Attendees experience Doctors experience, Admission Process, Customer Engagement etc. Data has 51 variables with 4989 observations and 1 Target predictor Net promotor score(NPS). NPS is multi- class variable with 3 labels "Promoter", "Detractor", "Passive" depending on the overall satisfaction response the Patient gave in the survey with levels 1 to 10. Promoter = score > 7, Detractor = score < 6, Passive = 6 < score < 8

# Data Analysis and Modeling
The questionnare variables are converted to Ordinal factors before performing the analysis. Performed Step-wise Logistic regression for Feature selection. Also there was an class imbalance issue and hence used oversampling and undersampling techniques to handle the class imbalance. There were variables leading to quasi-complete seperation. Dropped those variables and obtained the top significant variables and built ML models.

Built RandomForest and Adaboost models for predicting the Net promoters. Initially converted the multi class target variable to binary by combining Promoter and Passive as one single class. Compared the performance of the models on both Binary and Multi class classification problem. Random forest model gave better results.

# Final Recommendation
Organization needs to identify the areas where Detractor customers were dissatisfied based on the scores provided in the survey and work toward improvement in those areas. If many Detractors unanimously provide negative feedback for a particular service, then maybe that service needs to be looked into. Offer promotions with highlights for the kind of Hospital services the Detractors are looking for.  
