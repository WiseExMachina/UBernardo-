UBernardo: Data-Driven Driver Insights
💡 Project Overview
Welcome to UBernardo, my inaugural data science project driven by over two years of firsthand experience as an Uber driver in Mexico City, Mexico. My journey, from navigating a Chevrolet Aveo 2016 to optimizing rides with an EV BYD Dolphin Mini (qualifying for Comfort and Uber Black), has provided me with invaluable, granular insights into the complexities of ride-sharing logistics and economics.

This project is a direct application of the data science skills I'm acquiring through my certificate program at ITESM, as I pursue my dream of becoming a Data Scientist at Uber. My unique perspective as a driver allows me to approach Uber's operational data with an unparalleled understanding of its real-world implications and challenges.

🎯 The Problem: Unpredictable Driver Earnings
A critical observation from my 3000+ rides is the persistent discrepancy between the upfront payment offered to me by Uber and the actual net earnings I ultimately receive. In approximately 99% of cases, my final payout is less than the initial offer, with the adjustment mechanism remaining largely opaque.

My core hypothesis, derived from extensive operational experience, is that I am often penalized for efficiency. When I complete trips significantly faster than Uber's estimated time, my earnings tend to be reduced. Conversely, during periods of heavy traffic where I take longer than estimated, my earnings are more likely to align with the original offer. This suggests a complex interplay between estimated vs. realized trip metrics and the final driver payout.

The goal of this project is to build a predictive model that accurately forecasts my actual net earnings for each ride, given the upfront offer and estimated trip parameters. This model aims to provide actionable insights for drivers, enabling more informed decision-making on which rides to accept.

📊 Data & Methodology
The foundation of this project is my personal Uber driver data, meticulously collected over 3000+ rides.

Key Variables (Currently Available)
My current dataset from Uber's export provides the following critical information for each trip:

Rider Fare Price: The gross amount the rider was charged for the trip.

Distance: The actual distance covered during the trip (Realized Distance).

Duration: The actual time taken for the trip (Realized Time).

Hour of Day: The hour the trip began (e.g., to capture peak/off-peak patterns).

Day of Week: The day the trip began (e.g., for weekday/weekend differences).

Missing Critical Data & Data Augmentation Strategy
Crucially, Uber's data export does not include the Upfront (suggested) Driver Payment offered to me, nor the Estimated Time and Estimated Distance provided at the moment of the ride offer. These are vital to directly test my hypothesis regarding efficiency penalties.

To overcome this, I am embarking on a manual data collection initiative. For future rides, I will systematically record the upfront driver payment, estimated time, and estimated distance at the point of the ride offer. My immediate goal is to collect approximately 200 such observations to begin validating patterns and enriching my dataset for model training.

Analytical Approach
Data Preprocessing: Cleaning and preparing the raw data, including deriving Hour of Day and Day of Week from timestamps.

Feature Engineering: Creating new variables like the actual net earnings (from Rider Fare and calculated commissions/fees) and, critically, Time_Deviation_Minutes and Distance_Deviation_KM once the estimated values are collected.

Exploratory Data Analysis (EDA): Visualizing relationships, especially focusing on how Time_Deviation_Minutes correlates with the difference between Upfront (suggested) Driver Payment and Realized Driver Payment.

Model Building: Developing regression models (e.g., Linear Regression, Random Forest, XGBoost) to predict Realized Driver Payment.

Model Evaluation & Interpretation: Assessing model accuracy using metrics like MAE and RMSE, and deriving actionable insights to explain the payment discrepancies.

🚀 Future Work
As this project evolves, its robustness will strengthen with the integration of new manually collected variables. Future enhancements include:

Directly incorporating Upfront (suggested) Driver Payment, Estimated Time, and Estimated Distance into the model.

Quantifying the "efficiency penalty" and its specific impact on earnings.

Potentially exploring external data sources (e.g., real-time traffic, weather) if feasible.

Developing a simple tool or app that allows me (and potentially other drivers) to input ride offer details and receive a predicted actual payout.

🤝 Connect With Me
This project represents my passion for applying data science to real-world problems and my commitment to a career at Uber. I'm eager to discuss my findings, challenges, and future iterations.

[Link to your LinkedIn Profile]

[Link to your Portfolio Website, if you have one]

Wise Ex Machina, Opus 1
