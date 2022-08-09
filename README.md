# Data-Journalism-Final-Project
This repository documents my analysis of change in California's wildfire spread and the California Department of Forestry and Fire Protection's (CAL FIRE) response during the five year period between 2017 to 2021. In this document I will broadly examine the relationship between fire damage and expenditures, and take a closer look at resource response to turbulent wildfire seasons.


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

# Analysis 4: Resources
## Data Analysis Process: 
  1) Pay attention to fires that spanned multiple counties. Duplicate sheet "2016".
  2) Sort rows alphabetically from A to Z by "COUNTIES" column. In row 32, El Dorado and Placer are listed in the same cell. Duplicate the row by inserting   a row above and pasting the data. Isolate El Dorado in one "COUNTIES" cell and Placer in the other, with the rest of the cells staying the same.
  3) Do the same for sheet "2021". Duplicate it, and sort rows aphabetically from A to Z by "COUNTIES" column. In row 9, Butte, Plumas, Shasta, Lassen and      Tehama are all listed in the same cell. Repeat the process of step 2, and isolate all 5 counties in seperate rows. Do the same for the clustered            counties in row 23, 89, 92, 116, 158 and 169.
  4) Make a pivot table with the sheet "2016" and lable it "2016 Fire by Counties".
  5) Insert "COUNTIES" into rows and "ACRES" into values. Summarize "ACRES" by COUNTA.
  6) Filter "ACRES" from Z to A to find the county with the greatest number of wildfires. 
  7) Repeat these steps with the sheet "2021," and lable the pivot table "2021 Fire by Counties".
  
  ![Sheet Used: 2016 Fire by Counties](https://user-images.githubusercontent.com/109619716/183381227-030e470f-834e-43db-9469-43a1ae559002.png) 
    
    Fresno and Kern both had 12 wildfires in 2016, the largest number.
    
  ![Sheet Used: 2021 Fire by Counties](https://user-images.githubusercontent.com/109619716/183386139-539a79e0-886f-4222-8a87-b7415c3d01c4.png)
     
    Riverside had 18 wildfires in 2021, the largest number.
    
    
# Analysis 4: Which county recieved the most funding from Cal Fire grants in 2016 and 2021?
## Data Analysis Process:
  1) From the "2016 Grants by County" sheet, create a pivot table entitled "2016 County Cal Fire Funding".
  2) Input "COUNTIES" into rows and "AMOUNT" into values. Summarize "AMOUNT" by SUM.
  3) Filter data from Z to A by column B to find the county that recieved the most funding from Cal Fire grants in 2016. 
  4) Repeat these steps after making a pivot table for the "2021 Grats by County" sheet, and entitle it "2021 County Cal Fire Funding" to find the county        with the greatest grant funding from Cal Fire in 2021.

  ![Sheet Used: 2016 County Cal Fire Funding](https://user-images.githubusercontent.com/109619716/183435498-5a0cf251-6083-4db0-b366-9d2cdd7cbece.png)
  
    Fresno received $1,000,000 in grant funding from Cal Fire, the greatest sum of 2016.
    
   ![Sheet Used: 2021 County Cal Fire Funding](https://user-images.githubusercontent.com/109619716/183437483-50de81bd-2d9c-47d3-a9b3-d6ca65942035.png)

    San Luis Obispo received $4,483,721.09  in grant funding from Cal Fire, the greatest sum of 2021.

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




 
