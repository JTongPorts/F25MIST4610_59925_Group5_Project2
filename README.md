
# Team 5 MIST 4610 Group Project 2

## Team Name:

59925 Group 5
## Team Members:

1. Whitt Bowles [@whittbowles](https://github.com/whittbowles)
2. Braxton Bray [@braxtonbray4](https://github.com/braxtonbray4)
3. Benjamin Gatchel [@bengatch](https://github.com/bengatch)
4. Jason Tong [@JTongPorts](https://github.com/JTongPorts)
5. Christie Wu [@wuchristie121](https://github.com/wuchristie121)

## Tableau Packaged Workbook:


## Dataset Description:

Source of the Dataset: https://catalog.data.gov/dataset/traffic-crashes-crashes <br>

The dataset was obtained from the City of Chicago Open Data Portal, originally published through Data.gov under the title “Traffic Crashes – Crashes.” It is maintained by the Chicago Police Department (CPD) and reflects crash records collected through their E-Crash electronic reporting system. The data includes all reported traffic crashes occurring on public roadways within Chicago city limits, excluding crashes recorded by agencies outside CPD jurisdiction (such as interstate highway authorities).

Data is continually updated as CPD finalizes crash reports or if amendments are made to existing records.

## Data Contained:
The dataset contains over 1 million rows and almost 50 columns displaying a wide range of variables describing each crash, such as the crash date and time, geographic location (street, intersection, ZIP code, and in some cases latitude/longitude), posted speed limit, roadway and environmental conditions (weather, lighting, and surface condition), traffic control device in place, and the reported cause of the crash. It also captures outcome-related fields, including total injuries, number of serious or fatal injuries, and indicators for circumstances such as hit-and-run or work-zone involvement. The columns contain a mix of data types including categorical/text fields (like weather condition and roadway surface), numeric fields (such as speed limit values and injury counts), and date/time variables.

## Data Manipulations:
There was incomplete data that ranged from 2013 – 2025, but visualizations display cleaned versions of data ranging from 2018 – 2025 that excluded any outliers or insufficient data.​ The dataset contained a lot of information with over 1 million rows and almost 50 columns of data, so we also filtered the dataset to only include data we need for analysis, eliminating columns that had too many null values or weren't relevant to data visualizations. This helped limit the amount of data we needed to work with, increasing overall efficiency. ​Other than basic filtering and data cleaning, the data was already in the data types we needed for analysis. No further manipulations were needed for the scope of the project.

## Question 1 (Descriptive/Prescriptive): What types of crashes are the most prevalent and severe, what are key contributing factors to these crashes, and how can insurance companies as well policy makers use this information to make better decisions? 
Understanding this crash data is important because it supports decision-making for both insurance companies and policy makers. For insurers, the dataset helps identify which types of crashes are most likely to result in high-cost claims, allowing for more accurate pricing and financial planning. It also improves underwriting by providing insights into which risk factors are most significant, enabling companies to make better decisions about what to insure and at what cost. Additionally, by revealing patterns behind severe or frequent crashes, insurers can develop targeted safety initiatives aimed at reducing future losses. For policy makers, the data justifies how funds should be allocated for road safety improvements, law enforcement deployment, and infrastructure changes. It also informs long-term transportation planning decisions such as where to expand roads, redesign intersections, and install or update bike lanes and crosswalks to improve public safety.

<img width="1540" height="789" alt="Q1_Crash Type   Damage" src="https://github.com/user-attachments/assets/c55415e5-0fd5-4ce2-8516-df35ce4f2410" />
<img width="1547" height="789" alt="Q1_Crash Type   Fatality" src="https://github.com/user-attachments/assets/83c6b324-8b1e-4746-9980-a030d20483dc" />

Rear-end and parked-vehicle crashes make up the majority of accidents in the dataset, resulting in frequent but generally low-severity property damage claims. In contrast, pedestrian and fixed-object crashes occur far less often but are responsible for some of the most severe and high-fatality outcomes. This divide between high-frequency minor claims and low-frequency catastrophic losses is valuable for insurers because it informs smarter pricing and risk assessment. By understanding these patterns, insurers can price premiums more accurately by balancing the cost of frequent low-severity damage with the financial risk of rare but severe crashes. It also allows them to refine underwriting criteria by focusing on factors such as driver history, vehicle safety features, and exposure to dense pedestrian areas. Additionally, insurers can better prepare loss reserves by anticipating potential increases in injury-related claims driven by these more severe crash types.

<img width="1546" height="790" alt="Q1_Crash   Primray Cause" src="https://github.com/user-attachments/assets/8b8bbc11-4e77-4dcf-b642-0a2faf85a212" />

The data shows that “Unable to Determine” is recorded as the primary cause for the majority of crashes, accounting for 41.66% of all incidents. The next most common cause is failing to yield the right of way, which makes up 11.8% of crashes, followed by following too closely at 10.15%. On the opposite end of the spectrum, texting contributes the smallest share of crashes, representing only 0.04% of all recorded incidents.

<img width="1546" height="788" alt="Q1_Crash Type   Lighting Condition" src="https://github.com/user-attachments/assets/3e179b6a-94e9-4816-9832-f23330a45ddf" />
<img width="1545" height="789" alt="Q1_Crash Type   Road Condition" src="https://github.com/user-attachments/assets/327c01e6-76c7-43bf-8cb1-6c7c3aa24a64" />

Most crashes occur during daylight hours, which is expected given that people tend to travel most frequently during the day. The second-largest share of crashes happens under dark but lighted road conditions, suggesting visibility still plays a meaningful role in crash likelihood. As a result, policy makers may consider adding more street lighting or implementing additional safety measures to help reduce crashes that occur in darker driving conditions. Similarly, most crashes take place on dry road surfaces, but wet road conditions account for the second-highest proportion of incidents. This indicates that weather-related surface changes significantly increase crash risk, and policy makers may want to deploy more signage, warnings, or roadway treatments to alert drivers during wet conditions and help lower crash rates.

Summary: <br>
The two bar charts illustrate which types of crashes are most common and which are most fatal, giving insurance companies valuable insight into both the frequency and severity of different crash categories. This information supports more accurate pricing models that balance risk and expected payouts. Additional analytical approaches could include linking this dataset with historical insurance premium and claims data to study how crash types influence actual costs, or building regression models to estimate how different factors contribute to final payout amounts. The final visualizations highlight contributing factors such as lighting conditions and roadway surface conditions, which are especially useful for policy makers. By understanding how these environmental factors correlate with crash occurrence, policy makers can design and implement targeted preventative measures—such as improved lighting or enhanced road warnings—to reduce crash rates and improve overall traffic safety.

## Question 1 (Predictive): How will the total number of traffic-related injuries change over future months based on historical crash trends and seasonal patterns? 

<img width="1547" height="791" alt="Q2_Crash   Injury Total" src="https://github.com/user-attachments/assets/7ecabfa4-4a8a-4a67-be07-c292cf3ad324" />

The predictive question is interesting because it reveals meaningful patterns in how traffic-related injuries rise and fall across the year. The model shows a clear seasonal cycle, including noticeable dips during the winter months when overall road activity decreases, followed by increases in the warmer months as traffic volume and outdoor movement rise. These recurring patterns help us see beyond individual monthly fluctuations and understand long-term trends in injury risk. This analysis is also important because forecasting future injury levels allows policymakers, emergency departments, and insurance companies to plan ahead. With predictive insights, agencies can allocate resources more efficiently, prepare for higher-demand periods, and implement timely safety interventions. For insurers, knowing when injury-related claims are likely to rise supports better financial planning and risk management. After discovering the patterns and trends from the historical data, we used Tableau's forecasting tool to forecast the total injuries per month for 2026. Based off the model, we can see that the forecast has followed the same trend as the past and that the dip for 2026 has increased even more and the peak follows through. Overall, the predictive model transforms historical crash data into actionable foresight that helps organizations make proactive, data-driven decisions.

Summary: <br>
The analysis revealed several key insights. Injury totals follow clear seasonal cycles, and long-term trends suggest meaningful shifts over time. Additionally, predictive modeling provides valuable forward-looking perspectives that can guide planning and prevention efforts. Other possible approaches to strengthen the analysis include incorporating additional time-dependent variables—such as temperature, precipitation, or holiday travel periods—and testing multiple forecasting techniques like ARIMA or machine-learning models. Segmenting forecasts by crash type or injury severity could also yield more targeted and actionable predictions.

## Conclusion:
Traffic crash data enables both insurance companies and policy makers to make data-driven, proactive decisions. Descriptive and prescriptive insights help identify the most severe crash types and key contributing factors, improving underwriting, pricing accuracy, and targeted safety programs. Predictive analytics further reveals future injury trends and seasonal patterns, supporting better planning and early intervention. Together, these analyses help organizations allocate funds and resources effectively, implement strategic road safety initiatives, and guide long-term transportation and infrastructure improvements. Overall, crash data strengthens decision-making and contributes to safer, more resilient communities.






