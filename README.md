# 1. Introduction

This project documentation outlines the development and implementation of Fleet Data Integration System. The purpose of this system is to analyze data from the Fleet Pin online system, enabling the customization of crucial information related to vehicle maintenance, registrations, and road charges. The integration process involves transforming raw data into a structured format that aids decision-making for timely vehicle servicing and compliance renewals.

# 2. Current System Overview

The Fleet Pin online system is the current platform used to track various data points of the fleet, including GPS locations, registration information, Road User Charges (RUC) details, Warrant of Fitness (WOF) and Certificate of Fitness (COF) expiration dates, as well as temperature readings from chiller units.

# 3. Project Scope

The scope of the project encompasses the development of a data integration system that takes Fleet Pin data, processes it using Python scripts, and applies specific transformations to produce customized outputs. These outputs include insights into upcoming service due dates based on kilometer readings, renewal dates for WOF/COF and vehicle registrations, and for RUC purchases.

# 4. Data Integration Process

The data integration process involves fetching data from Fleet Pin, organizing it using pandas data frames, and applying transformations to derive meaningful insights. These transformations include data formatting, filtering, and calculations to determine key dates and thresholds for service and renewal requirements.

# 5. Key Features
The integrated data provides SGM Ltd with several key benefits:

-   Predictive maintenance: Highlights upcoming service due dates based on vehicle kilometers
-   Compliance management: Reminders for WOF/COF and registration renewals
-   Financial planning: Notifications for RUC purchases to manage charges efficiently

<br>

Here's a breakdown of the code, explaining each step

# 9. Future Enhancements

Future improvements could include real-time data syncing, advanced predictive analytics, and integration with maintenance scheduling tools. Scalability considerations should also be explored to accommodate a growing fleet.


# 10. Conclusion
The Fleet Data Integration System enhances fleet management by providing actionable insights derived from Fleet Pin data. This tool assists in making informed decisions related to maintenance, compliance, and financial planning, ultimately leading to improved operational efficiency.

