<img src=https://github.com/sularaperera/Fleet-Data-Integration-System-Python/blob/main/images/banner.png></img>

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

Import necessary libraries and modules:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/1.png width=800></img>
<br>
Read data from a CSV file into a pandas DataFrame using specific columns:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/2.png width=800></img>
<br>
Convert 'WoF Due' and 'Rego Due' columns from string to datetime format:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/3.png width=800></img>
<br>
Get today's date for comparison:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/4.png width=800></img>
<br>
Calculate days remaining for WOF Renewal and Rego Renewal:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/5.png width=800></img>
<br>
Clean 'Odo / Hours / Hubo' data by extracting numbers using regex:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/6.png width=800></img>
<br>
Split 'Odo / Hours / Hubo' data into 'ODO' and 'Hubometer' columns:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/7.png width=800></img>
<br>
Extract numerical values from 'Next Service Due' and 'RUC Due' columns:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/8.png width=800></img>
<br>
Calculate RUC Due in kilometers and Service Due in kilometers:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/9.png width=800></img>
<br>
Apply styling to the DataFrame for highlighting specific ranges of values:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/10.png width=800></img>
<br>
Define a file path and save the DataFrame to a CSV file:
<br>
<img src=https://github.com/sularaperera/5.Produce-Pronto-Fleet-Report-Python/blob/main/code_snippets/11.png width=800></img>
<br>
Initial Data
<br>
<img src=https://github.com/sularaperera/Fleet-Data-Integration-System-Python/blob/main/images/initial_data.png></img>
<br>
Report View
<br>
<img src=https://github.com/sularaperera/Fleet-Data-Integration-System-Python/blob/main/images/report_view_bl.png></img>

# 9. Future Enhancements

Future improvements could include real-time data syncing, advanced predictive analytics, and integration with maintenance scheduling tools. Scalability considerations should also be explored to accommodate a growing fleet.


# 10. Conclusion
The Fleet Data Integration System enhances fleet management by providing actionable insights derived from Fleet Pin data. This tool assists in making informed decisions related to maintenance, compliance, and financial planning, ultimately leading to improved operational efficiency.

[Click here to see the full project](https://github.com/sularaperera/Fleet-Data-Integration-System/blob/main/script_new_.ipynb)

