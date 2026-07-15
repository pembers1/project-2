# Scenario Modelling & Profile Optimisation

## Project Summary
Developed an inventory allocation and profile optimisation tool using Excel and advanced lookup-based modelling techniques. The solution automates PPK distribution planning, generates system-ready allocation profiles, and supports data-driven inventory decisions by modelling multiple allocation scenarios against business stock targets. This reduced manual planning effort while improving consistency, scalability, and inventory control.

## Business Problem
When new product lines are received into the business, stock can arrive as either:

*	Pre-packaged assortments (PPKs)
*	Individual bulk sizes

PPKs are generally preferred because they contain a balanced size profile and are more efficient to distribute to stores, whereas bulk boxes only contain one size, and have to be broken down into individual sizes to be picked effectively by the warehouse.

Usually, the business aims to distribute approximately 80% of incoming PPK stock to stores whilst retaining enough inventory to support future replenishment requirements. This ensures stores have the full size range of a new style available to sell.

Determining the optimal allocation level manually required multiple calculations involving:

*	Number of stores
*	Number of sizes per PPK
*	Total PPK intake
*	Guessing profile requirements
*	Generating and running synthetic picks to see how many PPKs were being sent out in total.

This made the process time-consuming and increased the risk of selecting suboptimal allocation quantities.

## Solution Developed
I developed an Excel-based allocation planning tool that converts inventory intake information into a profile code that can be directly applied within the inventory management system.

Users enter:

*	Number of stores
*	Sizes contained within a PPK
*	Total PPK intake

The tool automatically calculates a range of allocation scenarios and produces the corresponding profile code required by the business system.

The model also shows the percentage of total intake being distributed, allowing planners to quickly identify the option that most closely aligns with the target allocation strategy. The options run from 1 through to 20 as I found this to be the best way of maximising tidyness within the spreadsheet whilst providing effective optionality.

## Methodology
The tool generates a range of potential allocation profiles and calculates:

*	Total PPKs distributed
*	Allocation percentage

Users can select a predefined option that best matches the desired distribution strategy.
For example:

*	PPK Intake: 500
*	Stores: 254

Option 1: 343 PPKs Sent (69%)

Option 4: 396 PPKs Sent (79%)

Option 20: 683 PPKs Sent (137% / Invalid)

The allocation percentage is calculated automatically, helping planners select the option that achieves the closest alignment to the business target. In this scenario, option 4 gives us the best result.

## Business Impact
Prior to the development of this tool, allocation planning required manual calculations and comparisons to determine how incoming PPK stock should be distributed across the store network. Planners needed to evaluate multiple allocation scenarios, estimate store coverage levels, and ensure that distribution decisions aligned with the business objective of sending approximately 80% of available PPK stock to stores.

The allocation planning tool transformed this process into a structured decision-support model, automatically generating allocation scenarios, calculating distribution percentages, and producing system-ready profile codes. This reduced the complexity of the planning process and enabled faster, more consistent inventory allocation decisions.

Faster Allocation Planning
* Eliminates the need for manual allocation calculations when distributing new product lines.

Improved Consistency
* Applies the same logic to every allocation decision.

Better Inventory Control
* Helps maintain an appropriate balance between store allocation and retained inventory.

Reduced Planner Workload
* Transforms a multi-step manual process into a simple input-and-select workflow.

System Integration
* Generates profile codes that can be used directly within the business inventory management system.

## Tools & Technologies Used
* Microsoft Excel
* XLOOKUP
* Formula-Based Modelling

## Screenshots & Workflow Evidence
The screenshots below demonstrate the workflow used to identify size-level inventory imbalances across the retail network. They show how stock data was extracted, transformed, analysed, and automated.

To protect commercially sensitive information, all screenshots used anonymized or representative data. The workflow, logic, and outputs accurately reflect the process used within the solution.

### Screenshot 1: Allocation Inputs
This screenshot shows the key business inputs required by the allocation model.

Users enter:

*	Total number of pairs contained within each PPK
*	Total number of stores receiving stock
*	Total PPK intake received

These values form the foundation of the allocation calculations and drive all subsequent distribution scenarios.

![Image Alt](https://github.com/pembers1/project-2/blob/main/Screenshot%202026-07-10%20090045%202.png?raw=true)
 
### Screenshot 2: Scenario Selection
This screenshot demonstrates the scenario selection process. 

The model generates multiple allocation options, each representing a different percentage of the incoming stock being distributed. Users can select the most appropriate option based on current business objectives, stock availability, and store requirements.

In this example, Option 4 has been selected as the preferred allocation strategy.

![Image Alt](https://github.com/pembers1/project-2/blob/main/Screenshot%202026-07-10%20090045%204.png?raw=true)
 
### Screenshot 3: System Profile Configuration
This screenshot shows the allocation profile mapping used by the model.

The configuration table links allocation outputs to the profile codes required by the system. This allows the model to automatically generate system-ready outputs rather than requiring planners to guess profile codes.

The profile codes are calculated based on the number of sizes in a PPK, and the number of PPKs going out to stores.

![Image Alt](https://github.com/pembers1/project-2/blob/main/Screenshot%202026-07-10%20090045%205.png?raw=true)
 
### Screenshot 4: Allocation Modeling Engine
This screenshot shows the output from the users decisions.

The tool automatically calculates a range of distribution scenarios, displaying:

*	The percentage of PPKs going out against the total PPKs
*	The number of PPKs going out

This enables users to double check their approaches and identify whether the option they selected most closely aligns with the business target.

In the example shown, the selected allocation profile distributes 393 PPKs, representing approximately 79% of available intake, closely matching the business objective of distributing around 80% of incoming PPK stock.

![Image Alt](https://github.com/pembers1/project-2/blob/main/Screenshot%202026-07-10%20090045%206.png?raw=true)
 
## Skills Demonstrated
*	Business Analysis
*	Inventory Planning
*	Process Improvement
*	Excel Modelling
*	Advanced Excel Functions
*	Decision Support Systems
*	Inventory Optimisation
*	Operational Analytics
