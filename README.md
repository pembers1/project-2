# Anomaly Detection & Exception Reporting

## Project Summary
Developed an automated inventory analysis tool that identifies size-level stock imbalances using threshold-based exception reporting. The solution calculates each size's contribution to total inventory and flags anomalies for investigation.

## Business Problem
Retail inventory should generally be distributed across sizes in line with expected customer demand.
However, stock imbalances can develop over time where a disproportionate amount of inventory becomes concentrated in a single size.

These imbalances are difficult to identify manually because they require reviewing inventory positions across multiple sizes, styles and locations.

Prior to the development of this tool, identifying size imbalances required manual review of inventory positions across multiple styles and locations. The automated process transformed this into a streamlined exception-reporting system.

Unexpected size imbalances can indicate:
*	Marketplace listing issues
*	Online availability problems
*	Inventory inefficiencies
*	Potential recall opportunities

## Solution Developed
I developed an automated inventory analysis tool that identifies styles with abnormal size distributions.

The process imports size-level inventory data and calculates the percentage contribution of each size to the total stock position. The model automatically highlights styles where a single size exceeds predefined business thresholds.

The solution dramatically reduces the amount of manual review required and helps focus attention on styles requiring investigation.

## Methodology
Each size percentage is evaluated against predefined thresholds.
When a size exceeds the threshold, the style is automatically flagged for further investigation.
The threshold can be adjusted to align with business requirements.

## Business Impact
Faster Identification of Inventory Issues
* Automatically highlights size-level inventory anomalies across large datasets.

Reduced Manual Analysis
* Removes the need to manually review individual size distributions.

Supports Marketplace Investigations
* Helps identify styles where abnormal stock patterns may be linked to marketplace availability issues.

Recall Opportunity Identification
* Highlights styles that may benefit from inventory balancing or recall activity.

Exception-Based Management
* Allows analysts and stock controllers to focus on flagged exceptions rather than reviewing every style individually.

## Tools & Technologies Used
* MAPPER
* Microsoft Excel
* Office Scripts

## Screenshots & Workflow Evidence
The screenshots below demonstrate the workflow used to identify size-level inventory imbalances across the retail network. They show how stock data was extracted, transformed, analysed, and automated.

To protect commercially sensitive information, all screenshots used anonymized or representative data. The workflow, logic, and outputs accurately reflect the process used within the solution.

### Screenshot 1: Data Gathering in MAPPER
This screenshot shows the custom MAPPER query used to retrieve inventory data by style, size, and location across the business. The report was specifically designed to provide the detailed stock information needed for analysis.

### Screenshot 2: Data Transformed in Excel
This screenshot demonstrates the exported inventory data was imported into Microsoft Excel and prepared for automated analysis. The data structure was organised to support size-level calculations and aggregations.

### Screenshot 3: Office Script Automation
This screenshot shows the Office Script used to automate the analysis process. The script applies predefined business rules, calculates size distribution percentages, and removes the need for manual review.

The automation standardises the process, improves consistency, and significantly reduces the time required to identify potential inventory issues.

### Screenshot 4: Office Script Automation
This screenshot shows the output after the automation has been executed. The model calculates the percentage contribution of each size against the total stock position for a style and automatically flags anomalies.

Items highlighted as Overweight indicate an unusually high concentration of stock in a particular size and are automatically marked for further investigation.

These anomalies can often indicate marketplace listing issues, missing sizes on online channels, inventory imbalances, or potential stock recall opportunities

### Screenshot 5: Filtered Exception Reporting
This screenshot demonstrates how the automated output can be filtered to focus exclusively on flagged styles. This exception-based approach allows stock controllers to concentrate on potential issues.

### Screenshot 6: Adjustable Business Rules
This screenshot shows how the threshold used to generate an Overweight flag can be configured within the Office Script.

In this example, styles are flagged when a single size accounts for more than 60% of total stock for that style. By adjusting this value, the tool can be tailored to match changing business requirements.


[Add additional screenshots as needed]

## Skills Demonstrated
* Data Preparation
* Data Transformation
* Data Analysis
* Inventory Analysis
* Office Scripts
* Excel Automation
* Exception Reporting
* Business Analysis
* Business Process Improvement
* Root Cause Investigation
* Data-Driven Decision Making
