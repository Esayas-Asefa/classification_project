# classification_churn_project

# Churn Drivers

Project Description:
    
    Reducing churn is a perpetual challenge for non-monopoly client based businesses. Finding out what factors lead to churn will provide Telco an opportunity to reduce the causes of churn. 
    
## Project Goal:

     Identify feature(s) that drive churn
     Use those features/drivers of churn to develop a model that would identify who is most likely to churn
     The information could be used to retain clientele and maybe even increase Telco's client base
    
## Initial Thoughts 

    My initial hypothesis is demographic classification is correlated to churn.
   
## The Plan

     Acquire data from personal
     Prepare data
        From existing data
             Identify nulls/Nan and replace them with the mean or get rid of that column if there are too many nulls/Nans
             Idenfity non-numerical columns and convert them into classification columns (1 and 0)
     
## Explore data

     Answer the following initial questions:
           Is one gender more likely to affect churn than the other?
           Are senior citizens more likely to churn?
           Do people with dependents churn more?
           Do people with partners churn more?
            
## Develop a Model to predict churn

      Use drivers identified in explore to build predictive models of different types
      Evaluate models on train and validate data
      Select the best model based on the highest accuracy
      Evaluate the best model on test data

 ## Data Dictionary
      
# Data Dictionary

| **Column**          | **Description**                                           |
|---------------------|-----------------------------------------------------------|
| **Customer ID**     | Customer ID                                               |
| **Gender**          | Whether the customer is a male or a female                |
| **SeniorCitizen**   | Whether the customer is a senior citizen or not           |
| **Partner**         | Whether the customer has a partner or not                 |
| **Dependents**      | Whether the customer has dependents or not                |
| **Tenure**          | Number of months the customer has stayed with the company |
| **PhoneService**    | Whether the customer has a phone service or not           |
| **Multiplelines**   | Whether the customer has multiple lines or not            |
| **InternetService** | Customer’s internet service provider                      |
| **OnlineSecurity**  | Whether the customer has online security or not           |
| **OnlineBackup**    | Whether the customer has online backup or not             |
| **DeviceProtection** | Whether the customer has device protection or not         |
| **TechSupport**     | Whether the customer has tech support or not              |
| **StreamingTV**     | Whether the customer has streaming TV or not              |
| **StreamingMovies** | Whether the customer has streaming movies or not          |
| **Contract**        | The contract term of the customer                         |
| **PaperlessBilling** | Whether the customer has paperless billing or not         |
| **PaymentMethod**   | The customer’s payment method                             |
| **MonthlyCharges**  | The amount charged to the customer monthly                |
| **TotalCharges**    | The total amount charged to the customer                  |
| **Churn**           | Whether the customer churned or not                       |

## Steps to Reproduce

    1. Clone this repo
    2. Acquire the data from CodeUp, Telco_churn
    3. Put the data in the file containing the cloned repo
    4. Run notebook
    
## Takeaways and Conclusions

Gender doesn't seem to be strongly associated with churn. There is a stronger relationship between churn and whether the customers are senior citizents, have children, and/or partners.

## Recommendations

Offer discounts to senior citizens to reduce churn, and family bundle discounts to fortify the lower churn rate of those with partners and dependents.