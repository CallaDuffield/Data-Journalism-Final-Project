# Data-Journalism-Final-Project
This repository documents my analysis of change in California's wildfire spread and the California Department of Forestry and Fire Protection's (CAL FIRE) budget response during the five year period between 2017 to 2021. In this document I will broadly examine the statistical relationship between wildfire damage and communities, and take a closer look at causes and grant funding response to the turbulent wildfire season of 2020. I mainly used statistics from <https://www.fire.ca.gov/stats-events/>.


# Analysis 1: Money
    How have CAL FIRE's expenditures changed from 2017 to 2021?
## Data Analysis Process: 
  1) Select the "CAL FIRE Stats" sheet.
  2) Calculate the percent change in expenditures between years by using the following formulas:
  3)    =SUM(B3-B2)
  4)    =DIVIDE(E3, B2)
  5) Format column F, "% Expenditure Change" by percent. Do the same calculations but with values in rows three through six.
  ![Sheet used: CAL FIRE Stats](https://user-images.githubusercontent.com/109619716/183568053-0c35e785-97cf-40e3-bf88-3bec5d5b1445.png)
  ### In the fiscal year 2020-2021, CAL FIRE expenditures rose 154.70% from the previous year. Let's take a look at fires by year to draw some conclusions.
  
# Analysis 2: Fire
    How has California wildfire acreage changed from 2017 to 2021?
## Data Analysis Process: 
  1) Select the "CAL FIRE Stats" sheet.
  2) Calculate the percent change in acreage between years by using the following formulas:
  3)    =SUM(D3-D2)
  4)    =DIVIDE(G3, D2)
  5) Format column H, "% Acreage Change" by percent. Do the same calculations but with values in rows three through six.
  ![Sheet used: CAL FIRE Stats](https://user-images.githubusercontent.com/109619716/183571268-2d34912a-037f-4f30-8f2f-1586a0552def.png)
  ### In the fiscal year 2020-2021, California wildfire acreage rose 1452.33%% from the previous year. Let's zoom in on the fiscal year 2020-2021.
  
  
# Analysis 3: Causes
    What were the top causes of large (300+ acres) California wildfires in 2020-2021?
## Data Analysis Process:
   1) In the sheet called "2020-2021 Fire Causes by County," create a column N entitled "Total by County."
   2) Find the sum of fires by county with the equation =SUM(B2:M2), and apply it to all rows.
   3) Sort the sheet from Z to A by column N to find the counties with the most wildfires in 2020.
  ![Sheet Used: 2020-2021 Fire Causes by County ](https://user-images.githubusercontent.com/109619716/183580701-e359fd3b-fd99-464d-9a0e-b60166ff571a.png)
    Riverside, El Dorado and Shasta were the counties with the greatest number of total wildfires.
## Data Analysis Process Continued:
   1) To find the biggest causes of wildfires in California in 2020-2021, make a new row at the bottom of the data and title it "Biggest Causes".
   2) Use the equation =SUM(B2:B53) for all columns.
   ![Sheet Used: 2020-2021 Fire Causes by County ](https://user-images.githubusercontent.com/109619716/183583975-caa914bb-cc82-4efa-8311-dff46612b61e.png)
   ### Aside from undetermined causes, Debris Burning caused the greatest number of wildfires at 579, followed by Vehicles at 449 and Equiptment use at            381.
    
    
    
# Analysis 4: Grants
    Which county recieved the most funding from CAL FIRE grants in 2020?
## Data Analysis Process:
  1) From the "2020-2021 CAL FIRE Fire Prevention Grant Awards" sheet, create a pivot table entitled "2020 Grants by County".
  2) Input "County" into rows and "Grant Amount" into values. Summarize "Grant Amount" by SUM.
  3) Filter data from Z to A by column B to find the counties that recieved the most funding from CAL FIRE Fire Prevention Grants in 2020. 
  
  ![Sheet Used: 2020 Grants by County](https://user-images.githubusercontent.com/109619716/183597755-0cfa5536-fb39-4d60-96c3-8bd37d823e67.png)
  ### Sacramento recieved the most grant funding in wildfire prevention at nearly $14 million, followed by Lassen at over $9 million.

    

# Analysis 5: Mapping
## Data Analysis Process:
  1) In a new sheet called "Fires and Funding," paste both columns from the sheet "2020 Grants by County" to columns A and B. 
  2) In the same sheet, paste column A, "County," and column N, "Total by County" from "2020-2021 Fire Causes by County" in columns D and E respectively.        Don't include row 54, "Biggest Causes." Rename "Total by County" to "Total Fires by County".
  3) Bold and Freeze the first row.
  4) Trim white space through "data cleanup" for column E, "Total Fires by County" so that the VLOOKUP equation works.
  5) Column C should be blank. Entitle it "Total Fires". Use the VLOOKUP equation =VLOOKUP(A2, $D$2:$E$53, 2, FALSE) and apply it to the whole column to combine the tables. There should be "#N/A" values because not all counties awarded grants had wildfires in 2020. Replace them with "0".
  6) Copy column C and paste values only in the same place. Then, delete columns D and E.
  7) Sort the data Z to A by SUM of Grant Amount. Keep in mind that the only wildfires totaled are those with 300+ acreage.
   
![Sheet Used: Fires and Funding](https://user-images.githubusercontent.com/109619716/183605503-97c3b9d7-cd2c-44a5-bf62-d12610ff2bc5.png)

![Sheet Used: Fires and Funding](https://user-images.githubusercontent.com/109619716/183605530-752da942-f4d8-4fa4-a3e2-7bd343682325.png)
    
 
 # Data Visualization
 California wildfire distribution in 2016

 
 # Story Summary and Additional Sourcing
 The data I compiled represents many communities in California that are impacted by wildfires. But how are these grants impacting individuals? Are the resources being used efficiently and effectively on the county level? Do the grants target the causes of wildfires that most need addresing? For further information on grants, I can comb through the grant project descriptions <https://www.fire.ca.gov/media/ymoohf13/final_fy-2020-21-cci-fire-prevention-grant-recipient-list-accessible-10-18-2021.pdf> and compare the goals with wildfire safety and education needs in each county.




 
