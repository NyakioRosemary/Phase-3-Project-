# Terry-Traffic-Stops-Project

![istockphoto-1388637792-170667a](https://github.com/NyakioRosemary/Terry-Traffic-Stops-Project/assets/127243987/175f575d-0253-4ae6-8206-0301be7ca7d9)

# Problem Statement: Predicting Arrest Flag in Law Enforcement Data
![image](https://github.com/NyakioRosemary/Terry-Traffic-Stops-Project/assets/127243987/68002356-5b06-4f8a-a506-57ace2fa00f8)

# Problem Description:

The aim of this project is to develop a classification model that can predict the likelihood of an arrest flag being raised during law enforcement incidents. The dataset contains various attributes related to law enforcement incidents, such as location, time, officer details, and other relevant factors. The target variable, "Arrest Flag," indicates whether an arrest was made during the incident.

The goal is to build a predictive model that can accurately classify incidents as either resulting in an arrest or not. This model can be used by law enforcement agencies to identify high-risk incidents or allocate resources more effectively.

## Objective:
The objective is to build a classification model that can predict the likelihood of an arrest flag being raised during law enforcement incidents. The model should be able to accurately classify incidents as either resulting in an arrest or not, based on the available attributes in the dataset.

# Business Understanding
A Terry stop, also known as a stop and frisk, is a legal principle that originates from the United States Supreme Court case Terry v. Ohio (1968). It refers to a brief detention or stop by law enforcement officers of an individual based on reasonable suspicion that the person has committed, is committing, or is about to commit a crime. The name "Terry" comes from the name of the petitioner in the aforementioned court case.

During a Terry stop, an officer is permitted to briefly detain an individual for questioning and may conduct a pat-down search (frisk) of the person's outer clothing if they have reasonable suspicion that the person is armed and dangerous. The purpose of a Terry stop is to allow law enforcement officers to protect themselves and others by ensuring their safety during interactions with potentially dangerous individuals.

It's important to note that a Terry stop is a lower level of intrusion compared to an arrest. While an arrest requires probable cause, a Terry stop requires only reasonable suspicion. The scope and duration of a Terry stop should be reasonable and limited to the circumstances that justified the stop in the first place.

The legality and specific procedures surrounding Terry stops can vary based on jurisdiction, as laws may differ in different countries and regions. It's essential to consult the laws and regulations of the specific jurisdiction in question to understand the exact legal framework and guidelines for Terry stops in that area.


## Evaluation:
The model is  evaluated based on its classification performance metrics, such as accuracy, precision, recall, and F1 score. The goal is to develop a model with high accuracy and balanced performance between the two classes (arrested vs. not arrested).

By successfully developing an accurate predictive model, law enforcement agencies can gain insights into the factors contributing to arrests and make informed decisions to enhance public safety and allocate resources efficiently.

# Data Understanding
This data represents records of police reported stops under Terry v. Ohio, 392 U.S. 1 (1968). Each row represents a unique stop. Each record contains perceived demographics of the subject, as reported by the officer making the stop and officer demographics as reported to the Seattle Police Department, for employment purposes.

## Data sources available for the project:

Seattle Terry Traffic Stops dataset SPD_Terry Stops

Additional datasets related to law enforcement, demographics, and geographic information (if applicable) SPD- Terry Stops by Perceived race of Subject

Expected timeline for the project:

4 Business days

### DataSet Information
         Updated
         May 18, 2023
"""Data Last Updated May 18, 2023/ Metadata Last Updated / May 18, 2023"""

         Date Created
         April 13, 2017
Frequency Daily Category Public Safety Tags Police, Terrystops, Detentions

What is in the Dataset
We have over 2million rows but we will only request for 50000rows and the 23 columns

Every row is unique identifier

# Data Preprocessing
![image](https://github.com/NyakioRosemary/Terry-Traffic-Stops-Project/assets/127243987/017f2aca-c171-41ae-90b2-feecd80783c7)

## EDA 
We found year and Officer squad and month important features in our models.


![image](https://github.com/NyakioRosemary/Terry-Traffic-Stops-Project/assets/127243987/22117f75-6710-4cf2-99b1-bc745ada1ad0)


![image](https://github.com/NyakioRosemary/Terry-Traffic-Stops-Project/assets/127243987/c531e083-ada5-4bdc-8fe9-3815546a706b)

## Model Results 
We went with Logistic Regression since it had a constant f1 score 
![image](https://github.com/NyakioRosemary/Terry-Traffic-Stops-Project/assets/127243987/b8b2b35a-05ea-482d-8ae7-8d06afe4e421)
on the confusion matrix provided, the model seems to have performed well. It correctly predicted a high number of true negatives and true positives, indicating that it has a good ability to distinguish between instances that result in an arrest and those that do not

# Conclusion
From the list of feature importance scores, we can draw the following conclusions:

The feature "officersquad_N/A" has the highest importance score, indicating that it plays a significant role in predicting arrests during Terry stops. This suggests that the absence of information about the officer's squad is an important factor in determining whether an arrest occurs.

Features related to the precinct, such as "precinct_North," "precinct_West," "precinct_Unavailable," and "precinct_Southwest," also have relatively high importance scores. This suggests that the location of the stop, specifically the precinct, can influence the likelihood of an arrest.

Other factors such as the subject's race, age group, officer's race, and the month of the stop also contribute to the prediction of arrests, albeit to a lesser extent.

Based on these conclusions, it appears that factors related to the officer's squad, precinct location, and certain demographic characteristics of the subject have the most significant impact on predicting arrests during Terry stops. These findings can provide insights for law enforcement agencies and policymakers to better understand the factors driving arrests and potentially guide decision-making processes in the context of Terry stops. However, further analysis and consideration of additional factors are necessary to fully evaluate the model's performance and draw more definitive conclusions.

# Recommendation
Focus on high-impact factors: Identify the most influential features in the models that contribute significantly to predicting arrests during Terry stops. Allocate resources and training efforts towards addressing these factors and improving outcomes. 
Improve data collection: Ensure accurate and comprehensive data collection during Terry stops. This includes capturing all relevant information such as officer squad, precinct, subject demographics, and other pertinent details. Improving data collection practices can enhance the quality of analysis and modeling, leading to more accurate predictions. 

Implement targeted training programs: Use the information from the models to develop targeted training programs for officers. Focus on areas where the models indicate a higher likelihood of arrests, such as specific precincts or officer squads. Provide training on effective communication, de-escalation techniques, and bias awareness to minimize the occurrence of arrests during Terry stops. 

Monitor and evaluate outcomes: Continuously monitor the outcomes of Terry stops, including the number of arrests made and the effectiveness of interventions. Regularly assess the performance of the models and update them as needed. Track key performance indicators and evaluate the impact of implemented measures on arrest rates and overall outcomes.

# Next Steps
Conduct further analysis: Consider conducting additional analyses to gain deeper insights into the problem. This could involve exploring different variables, conducting subgroup analyses, or using advanced modeling techniques. Continuously strive to enhance your understanding of the factors influencing arrests during Terry stops. Iterate and adapt: Treat your analysis and recommendations as an iterative process. As you gather more data, receive feedback, and assess the impact of your actions, be prepared to iterate and adapt your strategies accordingly. Continuously learn from your experiences and adjust your approach as needed

# Thank you
