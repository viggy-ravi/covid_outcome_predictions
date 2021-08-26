# covid_outcome_predictions

The R-markdown for this project can be viewed [here](https://viggy-ravi.github.io/projects/).

This project consists of:

    1) Tidying dataset
    2) MANOVA Testing
    3) Randomization Test
    4) Linear Regression
    5) Bootstrapping
    6) Logistic Regression (ROC, AUC)
    7) Logistic LASSO Regression (k-fold cross validation)

For this report I will be looking into COVID-19 patient pre-condition dataset provided by the Mexican government (originally found on  [this kaggle challenge](https://www.kaggle.com/tanmoyx/covid19-patient-precondition-dataset)). The dataset contains information on **566,602 patients for 23 different attributes**, listed below. Before you get into the data, just know that the **bolded items** are the attributes that **remain** in my dataset for analysis after cleaning. Also, the original dataset uses `1's` for yes, `2's` for no, and (`97`,`98`,`99`, or `9999-99-99`) for `NA`.

1. `id` - unique number for patients

2. **`sex`** - F/M (1/2)

3. **`patient_type`** - not hospitalized/hospitalized (1/2) 

4. **`entry_date`** - date when patient entered hospital

5. **`date_symptoms`** - date when patient started showing symptoms

6. **`date_died`** - date patient died (9999-99-99 means recovered)

7. `intubed` - if patient needs ventilator

8. **`pneumonia`** - if patient has pneumonia

9. **`age`** - age of patient

10. `pregnancy` - if patient is pregnant

11. **`diabetes`** - if patient has diabetes

12. `copd` - if patient has Chronic Obstructive Pulmonary Disease (COPD)

13. `asthma` - if patient has asthma

14. `inmsupr` - if patient is immunosuppressed

15. **`hypertension`** - if patient has hypertension

16. `other_disease` - if patient has another disease

17. `cardiovascular` - if patient had a history of a heart related disease

18. **`obesity`** - if patient is obese

19. `renal_chronic` - if patient has chronic renal disease

20. `tobacco` - if patient uses tobacco products

21. `contact_other_covid` - if patient came in contact with someone else with covid

22. `icu` - if patient was admitted to the ICU

23. **`covid_res`** - if patient has resistance - tested positive (1), negative (2), or is waiting for results (3)
