EHR Grant Proposal 

  

Identifying high-risk candidates for asthma intervention programs in the state of North Carolina, US 

 

Asthma is a common chronic medical condition that affects millions of children in the United States and leads to a high morbidity with significant healthcare resource use when not optimally managed. Childhood asthma is a heterogenous disease with many factors that are associated with the risk of exacerbation often resulting in emergency room visits and hospital admission. There are many variables that have been validated individually in prior studies that are associated with an increased likelihood of an asthma exacerbation leading to hospitalization.  

The aim of this project is to create a machine learning model using validated predictors that can determine the risk of emergency room utilization and hospital admission for individual patients. Our healthcare system will use these data to target high-risk patients with resources that are known to improve the control of asthma. We will develop an application that can be run natively within an EHR, outside of an EHR, and locally on patient’s and provider’s tablets or phones. 

Background 

Asthma is a heterogeneous inflammatory airway disease that continues to cause considerable morbidity across the world, with poor asthma control leading to hospitalizations and rehospitalization. Asthma is estimated to affect 339 million people worldwide.1−3 and approximately 25 million Americans have asthma, which is equal to about 1 in 13 people, including 8% of adults and 7% of children.4 

Being able to associate asthma patients and risk of hospitalization was key to our question and through research have found that patients with mild asthma remain at risk of severe exacerbations, accounting for 30–40% of asthma exacerbations requiring emergency care.5 Also noting that severe asthma that is inadequately controlled is associated with poor outcomes, such as diminished health-related quality of life, acute exacerbations, ER visits, and hospitalizations).6 

The health economic impact of asthma is estimated to be about $80 billion in the US, of which $50.3 billion is related to direct medical costs. 7 Subsequently, the adjusted average of asthma-related costs per patient in a follow-up year were $58,000 due to non-severe uncontrolled asthma that resulted in an asthma hospitalization and $200,000 due to severe uncontrolled asthma that resulted in asthma hospitalization.8 Finally, there are many comorbidities seen in a majority of patients, which could potentially lead to higher costs, due to increased ER visits. The most common comorbidities cited were, coexisting Type 2 Inflammatory Airway Diseases, Chronic Rhinosinusitis with Nasal Polyps (CRSwNP) (45%), non-steroidal anti-inflammatory drug-exacerbated respiratory disease (NSAID-ERD)/ aspirin-exacerbated respiratory disease (AERD) (7.2%), and Allergic Rhinitis (72.6 – 94.3% of patients).9-13 

 

“AIR-NC” Description and Application 

“AIR-NC” was developed as a predictive modeling tool to aid healthcare professionals in the evaluation of the North Carolina population to assess the likelihood of someone developing asthma and how many additional ER visits a current asthma patient can expect to have. We seek to improve the quality of preventive care for future asthma patients, a goal that includes transforming the current way we assess the North Carolina hospital system approach to healthcare and associated preventative measures. The modeling components of “AIR-NC” are rooted in predictive strategies for asthma identification and prevention of ER visits. 

 

We define Health resources/health care resources as emergency department visits, intensive care unit admissions or other hospitalizations, and scheduled and unscheduled physician appointments.14 Understanding the current US care model, visits to the emergency room incurs a great amount of patient and healthcare related costs. Therefore, our goal is to evaluate current diagnosed asthma patients through varies geographical and demographical traits to predictive future patients that would be identified as at-risk asthma patients. Thus, being able to identify these patients we could implement a preventative asthma care model allowing for less ER visits and decrease healthcare costs. Although mild to moderate asthma is manageable in the primary care setting, patients with poorly controlled, difficult-to-treat, or severe asthma may benefit from referral to a specialist.15 If current asthma patients are not receiving optimal care, or future at risk patients are not identified in a timely manner, this could lead to rising healthcare costs in North Carolina. 

 

“AIR-NC” seeks to: (1) evaluate patient characteristics (2) rapidly identify at risk patients with potential for disease prevalence, (3) generate a timely report of asthma-related ER visits and (4) provide North Carolina an option to facilitate preventative care measures. We are considering “AIR-NC” a local-based prototype and to complete our research to refine our model and implement at scale, we would require the necessary funds to do so, which we can expect to achieve this success through your grant. 

 

Having the ability to predict current undiagnosed asthma patients or those at risk of being a future asthma patient, we could help improve preventive asthma care and optimize treatment strategies. Using our predictive modeling, developed by our team of experts, and rooted in our predictive asthma initiative, we will be able to quickly identify patients who may benefit from a health intervention without requiring a potential life-threatening emergency department visit. Implementation of “AIR-NC” in North Carolina hospitals has the potential to transform the preventative care pathway and improve the quality of care for at risk asthma patients. 

 

Statistical Analysis 

Our purpose for performing this analysis was to determine which variables were most effective at predicting pediatric asthma-related emergency department visits and hospitalizations. The most relevant variables for asthma ED predictions were identified through a thorough literature review. 16-18 The algorithm is trained on the distinct variables of; Rhinitis, Seasonal Rhinitis, Chronic Bronchitis, ER follow-up visits (> 3), Race, Poverty rates, Air quality, current medication/therapy (ACTUAT, Fluticasone), Food Allergies, and Environment allergies. 

 

The model is simulated as a distinct combination of these variables, optimized to cover a comprehensive set of plausible patient-case scenarios. In the experiment, predictive models, including regularized linear regression, random forest, support vector machine (SVM), and Naïve Bayes were trained with data set of asthma patients to predict whether there would be an ED visit or no ED visit. Model selection was done using the mean cross validation score of area under precision-recall curve.  

 

Ensemble learning techniques were used to determine the number of subjects who experienced a subsequent asthma-related emergency department during the time of our analysis. SVM analyses were then performed to determine which variables had an impact on subsequent asthma-related emergency department visits and which variables were most effective at predicting a subsequent asthma-related emergency department visit. Regularized linear regression was unable to appropriately classify patients due to a shrinking coefficient toward zero and therefore was disregarded. Naïve Bayes relied on independent variables and from our literature research, we understood our variables to be correlated and therefore was disregarded from the final model. The best performing algorithm across all experiments was the support vector machine. The decision making within our model contains a gradient confusion matrix SVM model, cross-validated on a 10-k fold of the training data set. The C and gamma tunning parameters in our SVM model were a great fit for our large dataset, as a lower value of C corresponds to a higher tolerance to classification errors on the training data and to a larger margin, while a higher value of C impacts the tolerance to error on the training data to be progressively smaller. Gamma offered another feature that we could optimally tune the SVM model to the data and to maximize its predictive accuracy. 

 

Variables cited in the literature but chosen to disregard from our algorithm was age (specifically childhood asthma, defined as 5 – 11 years old). Age was omitted rather than imputed because all encounters for an individual patient are collapsed into one observation; such that the modeled data is not regarding all encounters but per patient. 

 

Variables contained in the original data set that were exempt from input in our model were due to lack of literature coverage as a viable predictor variable. The ability to remove variable noise from our model, it allowed us to predict more accurately because our chosen variables had some correlation and see how closely related, they are. 

 

“AIR-NC” seeks input of the following questions to effectively and accurately predict whether a patient is at risk for a future ED visit: 

 

Does the patient have an initial asthma diagnosis? 

The success of our model is first determined by the factor of whether a patient had an initial hospital, ambulatory, or otherwise, admission that led to a diagnosis of asthma. Factors not assessed in our model of why a patient was not included in the analysis that did not have an asthma diagnosis led to poor results of predictability. Being able to accurately assess ER-associated visits were directly correlated to if a patient had an initial diagnosis of asthma. 

Has the person had a prior asthma related ER visit? 

Frequent ER visits due to an asthma related event increases the risk of higher associated healthcare costs and subsequent economic burden. The importance of limiting ER visits is highlighted by the finding of if a person has already been admitted to the ER, due to a prior asthma related event. To which the degree of ER visits is equivalent to >1 visits. Another key item to note is that if a person has had >1 ER visit recorded, there is greater potential for identifying a comorbid patient, which could potentially be linked to increased ER (or another point of care; PCP, specialty) visit and associated costs. 

 

Which variables has an impact on asthma-related ER visits? 

Identifying common comorbidities associated with asthma (Rhinitis, Seasonal Rhinitis, Chronic Bronchitis, and allergies) we seek to predict patient ER visits based on these variables. Race, poverty rates, air quality, and current medications were also used to assess the potential for subsequent ER visits of an asthma patient. By performing an in-depth literature search of known predicting variables, we sought to include similar variables in our model all at once to assess whether a patient did or did not have an ED visit. 

 

 

 

 

Methods for data management 

Python 3.9.1 was used for data analysis through Jupyter Notebook. A comprehensive EHR dataset available through our health system data warehouse was used to build and test a predictive machine learning model. The response variable chosen was emergency room visit/admission; therefore the “encounters” csv file was used to merge with the “patients” csv file using the patient identifier key. Further files including “conditions”, “allergies”, “medications”, and “observations” were likewise joined using the encounter identifier key. Outside data sources were identified and added that provided zip to county conversions, census data, poverty rates, and median household income levels at the county level.19 Furthermore, air quality data at the county level was incorporated into the model.20 Dichotomous classification predictors were created from the dataset for the following as being present or absent/not indicated in Table 1. These predictors were used as they have been shown to be associated with the higher risk for asthma exacerbation, sub-optimally controlled asthma, or emergency/urgent healthcare utilization.21 This working dataset contained 12,233 patient encounters, of which 3,083 were ED related and 9,150 were non-ED related encounters.  

A classification model was created using the scikit-learn support vector machine package. The response variable chosen, emergency room admission, is the class response variable and the 16 dichotomized variables are the predictors. The dataframe was segmented into one predictor dataframe including all the predictors which was further scaled and one response dataframe including the response variable. The dataframes were further segmented into a training set (70% of data) and a test set (30% of data). Cross validation was used to train the model with the Kfold scikit-learn parameter. The scikit-learn GridsearchCV algorithm was used to identify the optimal SVM parameters for model fit. These parameters were then used in the model applied to the test data. The scikit-learn metrics package was used to calculate the confusion matrix, accuracy score, precision score, and recall score. Additional models were also developed for comparison purposes using scikit-learn regularized logistic regression and naïve Bayes classification packages. The same dataset and segmentation technique for training and testing were utilized. 

Results 

After collecting and compiling the features relevant to patients with asthma, we then processed the resulting asthma data frame through several models in the sci-kit learn metrics package. Our findings indicate that the SVM algorithm, a supervised machine learning algorithm suited to classification challenges, does indeed create a model that accurately predicts the likelihood of emergency room admission for an individual patient. 

The SVM (support vector machine) plots each instance of data as a point in n-dimensional space, with n being equal to the number of features included. The SVM then generates a hyperplane which represents the largest minimum boundary that maximizes the distance between the data points of both classes. Maximizing this marginal distance provides confidence that the model will correctly classify and differentiate future data.  

The SVM regularization (or penalty) parameter of C was optimized at 1, which separates as many distinct instances as possible while maintaining the largest possible decision boundary. The best gamma hypermeter, the curvature parameter used to optimally fit the data, was determined to be 0.0428, indicative of a low probability of model overfit. 

 

Figure 1. SVM Confusion Matrix with “ED” = Emergency Admission and “No ED” = No Emergency Admission 

 

Accuracy 

0.84 

Precision 

0.73 

Recall 

0.57 

F-1 

0.64 

 

Table 2. SVM Confusion Matrix Results 

The accuracy score of this confusion matrix is 0.84, the highest accuracy score of achieved by the models tested. An 84% accuracy score represents the performance ratio of correctly predicted positive observations to total observations.  In addition to the highest accuracy, the SVM model also exhibits higher precision than either Naïve Bayes (0.57) or the Nearest Neighbor model (0.64). While our regularized logistic model yielded an equivalent accuracy score at 84%, the F1 score of the SVM model demonstrated more balance between precision and recall, with a score of 0.64 compared to 0.61 score given by regularized logistic regression. The necessary conditions concerning collinearity and independence among variables were not necessarily satisfied and may explain why the naïve Bayes model yielded the lowest accuracy among all models tested. 

Since the support-vector machine learning algorithm is robustly designed to address classification problems, we trust that when correctly applied, this model will both recommend targeted interventions and reduce emergency room admissions among patients with asthma. 

 

Implementation Decision Options  

After the predictive model has been created, our team has a few short-term decision options and short, medium, and long-term goals based on funding. The decision options include: 

Digital Health App that can send data out to providers – estimated cost $100,000 

Build the model as a tool that integrates within Electronic Medical Record Systems as a predictive model real time alert tool – estimated cost $1,000,000 

Separate application that uses an API to communicate with Electronic Health Exchange  

 

Digital Health App with an API 

Pros:  Since our model requires 15 inputs for Asthma prediction, we would easily be able to get the tool out rapidly and into the hands of the end-users, which are those with Asthma. This would be useful as a tool that could help direct asthma patients into the right direction for intervention. We would still be able to push data when needed to providers in the form of an API or simple HL7 data feed. Development cost should be lower because we would only need to develop an app and push it out to consumers.  

Cons: Since data is collected from the Asthma end users the onus will be on providers (and their accompanying EMR systems) willing to accept the data and work with patients for their interventions. If providers are not appropriately reimbursed or there is no incentive to integrate additional technology stacks into their workflow, the likelihood of this solution being scaled out is low from the provider side.  

 

Integrate into Electronic Health Record Systems (Population Health workflows) as a real time alert tool 

Pros: If data can be collected at the point of care, real time alerts can be sent through providers, health insurance companies, and other touchpoints of the care cycle where interventions could be done. Because it is integrated within the EMR platform, little extra work would need to be done by providers and the integration should align very with population health programs and disease management programs. 

Cons: Working with EMR companies can be challenging as they are likely to have their own in-house solutions. If providers were wanting to have this integration, an EMR company would need to be willing to configure those platforms and systems for a tool that may not bring in enough additional revenue to justify the development costs. 

  

Separate Application that uses an API to communicate with EHR Systems via Electronic Health Exchange 

Pros: The standalone tool could be built as a website that patients can access and if the patients are at elevated risk, the data could be sent via API to a central system or electronic health exchange (similar to how the CDC collects influenza data). 

Cons:  Electronic health exchanges face tons of interoperability problems and data sharing between different providers, health systems, and patients could be difficult.  

 

Recommendation 

We recommend starting with a digital health platform in the form of a mobile app that patients can use. This is because development costs are lower, it is easier to scale, data can be sent to providers, and because it offers more interoperability potential. Upon user acceptance of the digital health predictive modeling app, we could then expand to and integrate within EHR systems. While sharing data with an electronic health exchange is ideal, it does not make as much sense in the short term because asthma is not a public health disease such as influenza or COVID-19 where it is much more imperative that the information exists on a localized and time- sensitive level.  

 

References 

Global Asthma Network. The global asthma report 2018. Available at: http://www.globalasthmareport.org.  

Global Health Data Exchange. Global burden of disease study 2016. Available at: http://ghdx.healthdata.org/gbd-results-tool. 

Chanez P, Humbert M. European respiratory review: asthma: still a promising future? Eur Respir Rev. 2014; 23(134):405-407. 

Centers for Disease Control and Prevention. (2020). 2019 National Health Interview Survey data. U.S. Department of Health & Human Services. Retrieved from: https://www.cdc.gov/asthma/nhis/2019/data.htm. 

Dusser D, et al. Mild asthma: an expert review on epidemiology, clinical characteristics and treatment recommendations. Allergy. 2007; 62(6):591-604. 

Luskin AT, Chipps BE, Rasouliyan L, et al. Impact of asthma exacerbations and asthma triggers on asthma-related quality of life in patients with severe or difficult-to-treat asthma. Allergy Clin Immunol Pract. 2014; 2(5):544-552. 

Nurmagambetov T, et al. Ann Am Thorac Soc. 2018; 15:348–356. 

Zeiger RS, et al. J Allergy Clin Immunol Pract. 2016; 4:120–129. 

Heffler E, et al. J Allergy Clin Immunol Pract. 2019; 7:1462–1468. 

Shaw DE, et al. Eur Respir J. 2015; 46:1308–1321 

Maio S, et al. Allergy. 2018; 73:683–695. 

Micheletto C, et al. Eur Ann Allergy Clin Immunol. 2010; 42:120–124. 

Rajan JP, et al. J Allergy Clin Immunol. 2015; 135:676–681. 

Sullivan SD, et al. Extent, patterns, and burden of uncontrolled disease in severe or difficult-to-treat asthma. Allergy. 2007; 62(2):126-133. 

Price D, et al. Asthma referrals: a key component of asthma management that needs to be addressed. J Asthma Allergy. 2017; 10: 209–223. 

Tolomeo C, et al. Predictors of Asthma-related Pediatric Emergency Department Visits and Hospitalizations. J Asthma. 2009; 46(8):829-34. 

Franklin JM, et al. Predictors of emergency department use in children with persistent asthma in metropolitan Atlanta, Georgia. Ann Allergy Asthma Immunol. 2017; 119(2):129-136 

Wang X, et al. Deep Learning Models to Predict Pediatric Asthma Emergency Department Visits. arXiv:1907.11195v1 [stat.ML] 2019. 

Office of State Budget Management, North Carolina. Available at: https://linc.osbm.nc.gov/pages/home/  

AirNow. Available at: https://www.airnow.gov/state/?name=north-carolina  

Gallucci M, et al. Use of Symptoms Scores, Spirometry, and Other Pulmonary Function Testing for Asthma Monitoring. Front Pediatr. 2019; 5; 7:54. 
