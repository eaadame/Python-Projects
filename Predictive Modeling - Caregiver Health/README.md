## About
For this project, I aim to create a model that will predict the overall health of a person based upon the level of care they provide to another individual. I will examine the effects being a caregiver plays into a person’s health. A caregiver is defined as a person, often a family member, who regularly looks after another sick, elderly, or disabled person. Many times, caregivers are unprepared for the burden of care they take on, and as such, their health suffers. Caregiving often includes the caregiver sacrificing large amounts of time during their day to provide for their recipient, foregoing time previously used to look after themselves. The CDC (CDC, 2018) reports that caregiving is an overlooked public health issue affecting millions of individuals. While caregiving can bring great satisfaction to the caregiver, it can also negatively affect their physical and mental health.

It is important to understand the relationship between the degree of caregiving provided and the health of the caregiver. Understanding this relationship will allow for better resources and help to be provided to the caregiver.

The data used for this project was aggregated by the Behavior Risk Factor Surveillance System in 2015. The dataset contains 330 unique columns as they pertain to the individual answering. The 2015 data set was specifically chosen over more recent datasets, such as the 2020 or 2021, as it contained over 20,000 data points related to Caregivers versus the 5,000 contained within the 2020/2021 datasets.

The first target from this dataset is the General Health variable, or GENHLTH. This question required respondents to the survey to provide their overall assessment of their health, from Excellent to Poor.

The second target from this dataset is the Mental Health variable, or MENTHLTH. This question required respondents to the survey to provide the number of days over the past 30 days in which they felt depressed, stressed, or had problems with emotions.

The third and final target from this dataset is the Physical Health variable, or PHYSHLTH. This question required respondents to the survey to provide the number of days over the past 30 days in which they felt their physical health was not good, to include physical illness or injury.

Citations: https://www.cdc.gov/aging/caregiving/caregiver-brief.html

## Data
Dataset Link: https://www.kaggle.com/datasets/cdc/behavioral-risk-factor-surveillance-system?select=2015.csv

## Conclusion
I fit the data to three different models which produced the following accuracy scores:

K-Nearest Neighbors: 42% Accuracy
K-Nearest Neighbors (Adjusted): 42% Accuracy
Decision Tree: 36% Accuracy
Random Forest: 42% Accuracy
The continued failure of the models to produce decent accuracy scores leads me to conclude that my hypothesis is incorrect. Caregivers' health is not worse than non-Caregivers. From Milestone 1, I saw that the trends in health for Caregives vs Non-Caregivers were very similiar. Additionally, from Milestone 1, I saw that the trends in reports of health were similar for caregivers at various levels of longevity of care-providing.

All three of these models failed to produce accuracy scores over 70%. I believe this is due to the following:

The BRFSS 2015 Survey GENHLTH question relies on a subjective assessment made on the part of the respondent. An article published in Sage Journals reported that individuals often have an unrealistic optimism about their health. This fact is supported by four different respondents (51, 90, 107, 134) who reported their General Health as 'Fair' or 'Good' despite reporting feeling physically or mentally unwell for at least 15 days or more from the past month. One of these respondents reported feeling both physically and mentally unwell for 30 days.
Dunning, D., Heath, C., & Suls, J. M. (2004). Flawed Self-Assessment: Implications for Health, Education, and the Workplace. Psychological Science in the Public Interest, 5(3), 69–106. https://doi.org/10.1111/j.1529-1006.2004.00018.x

Respondents were asked about their General Health prior to being asked questions about whether they have chronic health issues. I believe this sets the respondents up to only think about their recent past health, potentially skewing the data. I would like to find a dataset in which respondents were asked aobut their health both before and after being question about their caregiver status and chronic health issues. I would like to know if their response changes any with this information in their head.
