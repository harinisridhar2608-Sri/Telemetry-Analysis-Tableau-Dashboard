This project analyzes machine telemetry data from Daikibo’s 4 factories using Tableau Desktop.
Each factory contains 9 different machine types that send a status message every 10 minutes.
The goal of this analysis is to answer two key business questions:

1️.Which factory experienced the most machine downtime?
2. Which machine types contributed the most to downtime in that factory?
Tools Used

Tableau Desktop
JSON Telemetry Dataset
Calculated Fields
Interactive Dashboard Filters

Methodology

Imported a unified JSON containing 160k+ telemetry records
Expanded nested JSON fields (location, status)
Converted epoch timestamps to DateTime
Created custom measure Unhealthy = 10 minutes per unhealthy event

Built two bar charts:
Down Time per Factory (DTF)
Down Time per Device Type (DTD)
Used DTF as a filter to dynamically update DTD
Selected the factory with the highest downtime to analyze device-level causes

Key Findings

Daikibo Shenzhen experienced the highest downtime in May 2021

The machines most responsible were:
LaserWelder
LaserCutter
HeavyDutyDrill


Files Included

Tableau workbook (.twbx)
Dashboard screenshot (.png)

Outcome

This dashboard allows leadership to quickly identify high-risk factories, target machine maintenance, and reduce future downtime.
