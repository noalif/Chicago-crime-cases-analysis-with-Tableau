# Chicago-crime-cases-analysis-with-Tableau

Preparation - Please set up a GCP account and add the Chicago Crime Data dataset: 
https://console.cloud.google.com/marketplace/product/city-of-chicago-public-data/chicago-crime?project=marine-proposal-274718

Choose the chicago_crime --> crime, from:

![image](https://github.com/noalif/Chicago-crime-cases-analysis-with-Tableau/assets/113893406/01c305b2-1e34-41c2-8574-97c21ce3099e)


### Questions:

### Part 1- SQL
(No need to attach the query result, only your SQL query)
Write a SQL query to calculate the month-over-month percentage change in the total number of
reported “Robbery” (primary_type) crimes in Chicago for the years 2018 to 2020.
The output should be the columns: year, month, pct_chg

#### Answer:
![image](https://github.com/noalif/Chicago-crime-cases-analysis-with-Tableau/assets/113893406/a584ed78-4b8a-4d25-b030-9e35a5cf17fc)


### Part 2- Python and SQL

### a. Think about questions you would try to answer using the Chicago Crime dataset.

1.   In the educational institutions of which Community Area is it highly recommended to deliver lesson plans on violence and protection, sex education, personal boundaries, etc..?
(Assuming that this can reduce the scope of violence in educational institutions)
2.   In which community areas/streets is it recommended to have police patrols to prevent sexual violence?
3.   Which districts are effective in their police work and which ones need training/courses to improve results? Possible examples for measuring the efficiency of the district: amount of arrests/ percentage of reduction of different types of crimes over the years.

3.   Are there places where the city of Chicago should intervene to prevent crimes? by legislation, supervision, etc (like inside hospital or other locations that have a lot of violence reports)

1.   A question that will give value to security companies: in which places are there more break-ins/thefts, and in which areas should we contact (and market) businesses/private homes to give them our service as a security company.

### b. Choose one question, explore it, and visualize it.

*   Chosen question - In which community areas/streets is it recommended to have police patrols to prevent sexual violence?
*   explore section in colab link: https://colab.research.google.com/drive/1BtSORyqJ8OD6yo83VYBnPRN_b3-lTEQ2?usp=sharing
*   visualization with tableau:

![image](https://github.com/noalif/Chicago-crime-cases-analysis-with-Tableau/assets/113893406/cdf0e799-00be-47df-863d-69aaf5f4aa53)

### link to Tableau dashboard (interactive version):
https://public.tableau.com/app/profile/.noa.lifshitz./viz/ChicagoSexualCrimeCases-NoaLifshitzPlus500/Dashboard3?publish=yes


### c. What other fields would you suggest adding to the dataset?

*   AP/PM column to conduct analyzes based on time range (for example, when is it better to increase police patrols, at noon in a certain area or in the evening?). The data had hours up to 12 and it was not clear if AM or PM. It didn't make sense to me that the offenses took place only until 12 o'clock and not during the whole day. 

*   If I understood correctly, the "arrest" column reflects whether an arrest was made or not. Sometimes an arrest is made but the arrested person is not the culprit. If this is the case, I would add a column of "Was found guilty after a police investigation" (the meaning would be not after a legal determination, but to make sure that the person who was arrested was indeed guilty after a police investigation and not because he was simply at the scene, for example, so they assumed he was the culprit and arrested him). The section will be able to help analyze the performance of police work.

*   Perhaps I would also add who is the district commander of the police or who is responsible for the community areas to understand if the person in the position has an influence on the amount of crimes. They will be able to analyze this in a more advanced way if they see that there is an effect and then they can check if he has undergone any important training, if this is reflected in the way he behaves towards his subordinates or any other reason.

-----------------------------------------------------

### Some conclusions from the data:

1.    Most reported sexual offences occur in the streets (whether it's an alley/sidewalk)
2.   There are certain community areas and streets that clearly need enforcement and appropriate police/educational treatment

1.   There is an increase in crime cases in the months of June-August. Research on the months of the year in Chicago can bring up interesting cases, maybe there are festivals or major events or vacations that create the increase in crime cases.

-----------------------------------------------------

## Additional Comments:

This is a dataset of reports from people. It is clear to me that not all cases are reported, therefore it is not possible to rely on this data alone, and integration with data from associations, for example, which receive phone calls about sexual offenses from victims who choose not to report to the police, should be considered and carried out. Maybe in this way we will get a more realistic picture and the police will be able to provide a better service to the community.
