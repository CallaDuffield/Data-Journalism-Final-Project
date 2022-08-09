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
   1) To find the biggest causes of wildfires in California in 2020-2021, make a new row at the         bottom of the data and title it "Biggest Causes".
   2) Use the equation =SUM(B2:B53) for all columns.
  ![Sheet Used: 2020-2021 Fire Causes by County ](https://user-images.githubusercontent.com/109619716/183583975-caa914bb-cc82-4efa-8311-dff46612b61e.png)
    Aside from undetermined causes, Debris Burning caused the greatest number of wildfires at 579, followed by Vehicles at 449 and Equiptment use at 381.
    
    
    
# Analysis 4: Grants
    Which county recieved the most funding from CAL FIRE grants in 2020?
## Data Analysis Process:
  1) From the "2020-2021 CAL FIRE Fire Prevention Grant Awards" sheet, create a pivot table entitled "2020 Grants by County".
  2) Input "County" into rows and "Grant Amount" into values. Summarize "Grant Amount" by SUM.
  3) Filter data from Z to A by column B to find the counties that recieved the most funding from CAL FIRE Fire Prevention Grants in 2020. 
![Sheet Used: 2020 Grants by County](https://user-images.githubusercontent.com/109619716/183595878-14779b45-9ae1-46f7-b3f0-bbcbf4947f28.png)

# Analysis 5: How has funding of counties through grants changed from 2016 to 2021?
## Data Analysis Process:
   In the "Calculations" sheet, use the (New-Old)/Old x 100 formula to subtract the sum of grant funding in 2021 from the sum in 2016, then divide the result by the sum in 2016. Multiply the result by 100 to find the percent change in grnt funding from 2016 to 2021.
  1) Input the 2016 value in cell A2, and input the 2021 value in cell B2. We will use these for our calculation.
  2) In cell C2, set up the function using the formula =SUM(B2-A2).
  3) In cell D2, divide the output by A1 using the formula =DIVIDE(C2,A2).
  4) In cell E2, multiply the result by 100 to find the percent change by using the formula =MULTIPLY(D1, 100).
    
   ![Sheet Used: Calculations](https://user-images.githubusercontent.com/109619716/183440934-03356007-8dc0-4083-bed0-2d1018504f6c.png)
      
     Cal Fire's grant funding of counties rose 304.26% from 2016 to 2021.
     
 # Data Visualization
 California wildfire distribution in 2016

 
 # Story Summary and Additional Sourcing
 The data I compiled represents many communities in California that are impacted by wildfires. But how are these grants impacting individuals? Are the resources being used efficiently and effectively on the county level? Do the grants target the causes of wildfires that most need addresing? For further information on grants, I can comb through the grant project descriptions <https://www.fire.ca.gov/media/ymoohf13/final_fy-2020-21-cci-fire-prevention-grant-recipient-list-accessible-10-18-2021.pdf> and compare the goals with wildfire safety and education needs in each county.




 
