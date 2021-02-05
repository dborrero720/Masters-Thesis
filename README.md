# Modeling for Maximum Profitability for Small Business Lenders Using Misclassification Costs 

#### This was my Masters Thesis that I wrote for my degree at Central Connecticut State University.  

Here’s the link to my project available on the CCSU Library website:

https://cscu-ccsu.userservices.exlibrisgroup.com/view/delivery/01CSCU_CCSU/1287369880003453

Here’s the link to to the dataset available on Kaggle:

https://www.kaggle.com/mirbektoktogaraev/should-this-loan-be-approved-or-denied/version/1?select=SBAnational.csv
  
A majority of this analysis was done using IBM SPSS Modeler, since this is what I mainly used in my graduate program.  Therefore, there is no code to go along with this project, as SPSS Modeler does not use code.  Excel was used for some of the initial steps and Tableau was used for some of the visuals. 

This analysis focused on Small Business Administration (SBA) loans that were issued between 2005 and 2009.  Many of these loans go into default, which results in a loss for the lender.  The goal was to build and test classification models to predict default.  Misclassification costs were calculated and used to evaluate these models on the test data, with the optimal model producing the highest profit on average per loan.

I followed the Data Science Methodology (DSM), as proposed in Data Science Using Python and R (Larose, C. D., & Larose, D. T. 2019). 

After identifying the problem,  the data preparation consisted of removing variables, reclassifying variables, as well as inputing values for missing data using several methods.

The EDA phase was performed for each variable with overlays of default.

<img width="569" alt="Screen Shot 2021-02-04 at 6 02 49 PM" src="https://user-images.githubusercontent.com/56644186/106967920-ec380300-6715-11eb-8d92-68e527f60891.png">

The data was partitioned to a train and test dataset in Phase 4 and the splits were validated using statistical testing.

The following Classification models were created in Phase 5:

1. CART 
2. C5.0 
3. CHAID 
4. QUEST 
5. Neural Network (NN) 
6. Random Forest (RF) 

The Evaluation Phase listed the respective measures for each model.  Based on highest profit and other measures, we determined the C5.0 model to be the optimal model for predicting loan default.  Between all models the term of the loan, “Term”, was the most important feature in predicting loan default.

<img width="508" alt="Screen Shot 2021-02-04 at 6 11 37 PM" src="https://user-images.githubusercontent.com/56644186/106967943-f6f29800-6715-11eb-949f-42bd04cb695b.png">
