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
      
| Feature | Definition |
|:--------|:-----------|
|tenure| How many months the customer has been a customer|
|monthly_charges| How much the customer pays monthly|
|Contract type ID| The total the customer has paid|
|gender_Male| Whether the customer is male or not (0:no, 1:yes)|
|senior_citizen_Yes| Whether the customer is a senior citizen or not 0:no, 1:yes|
|partner_Yes| Whether the customer has a partner or not (0:no, 1:yes)|
|dependents_Yes| Whether the customer has dependents or not (0:no, 1:yes)|
|phone_service_Yes| Whether the customer has phone service or not (0:no, 1:yes)|
|multiple_lines_No phone service| Whether the customer has multiple lines of service w/o phone service|
|multiple_lines_Yes| Whether the customer has multiple lines of service or not|
|online_security_No internet service|Whether the customer has online security w/o internet service or not|
|online_security_Yes|Whether the customer has online security or not|
|online_backup_No internet service|Whether the customer has online backup w/o internet service or not|
|online_backup_Yes|Whether the customer has online backup or not|
|device_protection_No internet service|Whether the customer has device protection w/o internet service or not|
|device_protection_Yes|Whether the customer has device protection or not|
|tech_support_No internet service|Whether the customer has tech support w/o internet service or not|
|tech_support_Yes|Whether the customer has tech support or not|
|streaming_tv_No internet service|Whether the customer has tv streaming services w/o internet service or not|
|streaming_tv_Yes|Whether the customer has tv streaming services or not|
|streaming_movies_No internet service|Whether the customer has movie streaming services w/o internet services or not|
|streaming_movies_Yes|Whether the customer has movie streaming services or not|
|paperless_billing_Yes|Whether the customer is enrolled in paperless billing or not|
|churn_Yes|Whether the customer churned or not 0:no, 1:yes|


## Steps to Reproduce

    1. Clone this repo
    2. Acquire the data from CodeUp, Telco_churn
    3. Put the data in the file containing the cloned repo
    4. Run notebook
    
## Takeaways and Conclusions

Gender doesn't seem to be strongly associated with churn. There is a stronger relationship between churn and whether the customers are senior citizents, have children, and/or partners.

## Recommendations

Offer discounts to senior citizens to reduce churn, and family bundle discounts to fortify the lower churn rate of those with partners and dependents.