# Distribution_Network_Analysis_for_Power_Charge_Utilities
Using python to perform Distribution Network Analysis. Working with popular Python Libraries such as Numpy, Pandas, Matplotlib, Seaborn and GeoPandas - For Distribution Network Geographics


## Key learning points(Learning Skills)
Explore Exploratory Data Analysis
Capacity Assessment
Network Optimization
Geographics Analysis & Visualization
Data Transformation
Reporting and Recommendations

## Tech Stack:
- Programming Language – Python
__Libraries:__
- __Numpy:__ For performing Mathematical operations over data
- __Pandas:__ For Data Analysis and Manipulation
- __Matplotlib.pyplot:__ For Data Visualization
- __Seaborn:__ For Data Visualization
- __GeoPandas:__ For Distribution of Network Geographics (Visualization)
- __Jupyter Notebook:__ For Documenting and presenting the analysis

## Business Introduction:
PowerCharge Utilities is a prominent electric utility provider operating in a dynamic and evolving energy landscape. The company’s primary mission is to ensure the reliable delivery of electrical power to millions of customers across urban and suburban areas. PowerCharge Utilities has established itself as a key player in the energy sector, focusing on sustainability and adapting to emerging technologies.
The energy sector has witnessed a significant transformation in recent years driven by environmental concerns, regulatory changes, and technological advancements. One of the most notable developments has been the rapid adoption of electric vehicles (EVs) as part of global efforts to reduce carbon emissions and combat climate change.

## Business Overview/Problem:
Power Charge Utilities encounters several critical challenges due to the growing adoption of electric vehicles:

__A. Increased Load Demand:__ Widespread EV adoption has caused a significant spike in electricity demand, particularly during peak charging times. This strains the existing distribution network infrastructure.

__B. Grid Overloads:__ Frequent overloads in the distribution network leads to voltage fluctuations and outages in specific areas, affecting overall grid reliability.

__C. Customer Satisfaction:__ EV owners expect reliable and convenient charging services. Ensuring this level of service is essential to maintaining customer satisfaction and loyalty.

__D. Cost Management:__ Balancing increased load demands and grid reliability comes at a significant cost. PowerCharge Utilities must optimize network investments to manage expenses effectively.
 
## Rationale for the Project:
Distribution Network Analysis in the energy industry refers to the process of studying and evaluating the electrical distribution networks that deliver electricity from high-voltage transmission lines to end-users, such as homes, businesses, and industrial facilities. This analysis becomes even more critical with the rise of EVs, as it transforms the energy landscape. 

## Top Five Reasons for the Project's Significance:
 
- A. Customer Retention: Maintaining a reliable EV charging experience is essential for retaining existing customers who have embraced EVs.
- B. Revenue Growth: Accommodating the growing demand for EV charging services opens new revenue streams and capitalizes on the expanding EV market.
- C. Sustainability Goals: Supporting EVs aligns with the company's sustainability objectives, contributing to reduced greenhouse gas emissions.
- D. Regulatory Compliance: Meeting regulatory standards for grid reliability and capacity planning is vital to avoid penalties and ensure operational excellence.
- E. Technological Innovation: Embracing data analytics empowers PowerCharge Utilities to stay at the forefront of technological innovation in the energy sector.

## Aim of the Project:
_The project aims to achieve the following objectives:_
A. Assess Network Capacity: Conduct a comprehensive analysis of the distribution network's current capacity to handle increased load from EV charging stations
B. Identify Bottlenecks: Identify potential bottlenecks and vulnerabilities within the distribution network that could hinder reliable electricity delivery to EV charging stations
C. Optimize Network Upgrades: Develop a data-driven strategy for network upgrades that maximizes efficiency, minimizes costs, and ensures grid reliability.

## Data Description:
__Distribution Network Analysis:__
- _A. Electric Vehicle (EV) Distribution Data:_
- Timestamp: Date and time of data points.
- Geographical Area: Location of each data point.
- Customer Type: Categorization of customers (e.g., residential, commercial).
- Electricity Consumption (kWh): Amount of electricity consumed.
- EV Charging Station Location: Latitude and longitude of charging stations.
- EV Charging Station Specifications: Details about charging stations.
- EV Type: Type of electric vehicles.
- Charging Habit: Charging behavior (e.g., daily, weekly).
- Number of EVs: Count of electric vehicles.
 
_B. Geospatial Data (Distribution Network Geographies):_ 
- Substation ID: Unique identifier for distribution substations. (Primary Key)
- Substation Location: Geographic coordinates of substations.
- Transmission Line Capacity (MW): Capacity of transmission lines.
 
_C. Weather Data:_
- Timestamp: Date and time of weather data
-  Temperature (°C): Ambient temperature.
- Precipitation (mm): Precipitation amount (rainfall or snowfall).
- Weather Conditions: Categorization of weather conditions (e.g., Clear, Rainy).

## Project Scope:
_A. Exploratory Data Analysis:_ Conduct EDA to gain insights into electricity consumption patterns and network performance. 
 
_B. Capacity Assessment:_ Utilize historical data to assess the current distribution network's capacity and identify areas with high demand growth. 

_C. Network Optimization:_ Utilize optimization algorithms to identify cost-effective network upgrades that address capacity shortfalls.
 
_D. Reporting and Recommendations:_ Present findings, including capacity assessments and upgrade recommendations, to the executive team for decision-making. Exploratory Data Analysis: Explore the data to understand its characteristics and discover patterns. 
 
_E. Data Transformation:_ Prepare the data for analysis by transforming, encoding, or normalizing it. 
 
_F. Data Analysis:_ Analyze data to understand pattern in order to generate insights that will be visualized. 
 
_G. Data Visualization:_ Create visual representations to communicate insights effectively. Interpretation and Insight Generation: Extract meaningful insights and interpret the results.

### Observations:
There seems not to be any correlation between betwen the plot values:abs
- For Electricity Vs Temperature there is no clear relationship as the data points are all scattered.
- Same Applies for Electricity Vs Precipitation as the data points are also scattered.

Based on the current temperature and precipitation factors, they do not have correlation with electricity consumption, this suggests, these factors do not influence electricity consumption in the distribution network.
It is still important to consider temperature and precipitation which are weather data for network analysis as extreme weather conditions can have impact on distribution network and its component, potentially leading to outages and other issues. 


## INSIGHTS:

_a. Electricity Consumption:_ The Electricity consumption is mostly centered around 500kWh, with with instances of higher and lower consumptions. This indicates varied demand at different times and locations.

_b. EV Types and Charging Habits:_ Electric scooters is the most common types of EVs. Most customers charge thier EVs daily, indicating a consistent daily load on the distribution network

_c. Consumer Type:_ Commercial Customers malke up the most consumer types.

_d. Geospatial Distribution:_ The spatial distribution od substations and EV charging stations is widespread.

_e. Geospatial Distribution:_ The EV charging station seems to be far from its corresponding substation

_f. Network Capacity:_ Some substations have high Consumption_to_Capacity_Ratio, indicating potentialbottlenecks and overloads in the network. There is also no correlation with the number of EVs per station and the Consumption_to_Capacity_Ratio, this shows that Number of EVs is not a factor for overload.
                                                                                                                                                                     
_g. Weather Correlation:_ The correlation between weather conditions (temperature and precipitation) is weak inthe current dataset, suggesting that other factors might be more influencial in affecting electricity consumption


## The Optimization Strategy/Recommendation
Based on the analysis of the busniess problem at hand, the following should be incoporated into the business;
_1. Potential Substation Upgrades:_ Prioritize upgrades at substations where the Consumption_to_Capacity_Ration is high, indicating potential overloads, upgrade the transmission lines because the EV Charging Stations are too far from thier corresponding Substations.

_2. Geospatial Analysis for Upgrade Planning:_ Use geospatial nalysis to determine the optimal locations for new substations or upgrade to existing ones. Consider factors like the proximity to high load demand areas(areas with high consumption to capacity ratio) and geograpical constraints.

_3. Demand Side Management:_ Implement demand-side management strategies to manage the load on the grid. Encourage customers to change thier EVs during off-peak hours through incentives to dynamic pricing.

_4. Advanced Monitoring and Analytics:_ Deploy advanced Monitoring systems to continously monitor the health and performance of distribution network. Use analytics to predict increased capacity and take preventive action.

_5. Cost-Benefit-Analysis:_ Conduct a comprehensive cost benefit analysis to differentiate upgrade options, Consider factors like the cost of upgrades, operational costs, poetential revenue from increased capacity and the impact on service relativity and customer satisfaction

_6. Customer Engagemen:_ Enage with customers to undersatnd thier needs and expectations. Provide Clear communication about network upgrades and how they will enhance service relaibility and meet the growing demand for EV charging.

_7. Continous Improvement:_ Continously monitor and assess the performance of the didtribution network. Gather feedback from the customers and other stakeholders and use this feedback to make urhter improvements and optimizations.

__By Following these steps, Power Charge Utilities can develop an effective optimization startegy to maintain the increased load demand from EV charging stations, ensure the relaibility and resilience of the ditribution network and meet the expectations of customers while all optimizing costs and ensuring regulatory compliance.__
                                                                                                                                                                                                                    



