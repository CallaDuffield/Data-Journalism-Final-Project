# Data-Journalism-Final-Project
This repository documents my analysis of change in California's wildfire spread from 2016 to 2021 and Cal Fire's grant response.


# Analysis 1: How many acres were burned by California wildfires in 2016 and 2021? What is the percent change between the two years?
## Data Analysis Process: 
  1) Select the "2021" sheet.
  2) Find the sum of the "ACRES" column by selecting it, clicking "data", and selecting "column stats." Scroll down to where "sum" is listed to find value.
  3) Replicate this process with the "2016" sheet.

  ![Sheet Used: 2021](https://user-images.githubusercontent.com/109619716/183370110-8155d6a1-f98f-4f9f-b070-87b2ef294efa.png)
     
    2,610,049 acres were burned by wildfires in California in 2021
     
  ![Sheet Used; 2016](https://user-images.githubusercontent.com/109619716/183372881-33c9ba6f-3a03-466b-8e70-745327405d40.png)
     
    500,281 acres were burned by wildfires in California in 2016
     
## Data Analysis Process Continued:
In a new sheet called "Calculations", use the (New-Old)/Old x 100 formula to subtract the sum in 2021 from the sum in 2016, then divide the result by the sum in 2016. Multiply the result by 100 to find the percent change in total wildfire acreage from 2016 to 2021.
  1) Input the 2016 value in cell A1, and input the 2021 value in cell B1. We will use these for our calculation.
  2) In cell C1, set up the function using the formula =SUM(B1-A1).
  3) In cell D1, divide the output by A1 using the formula =DIVIDE(C1,A1).
  4) In cell E1, multiply the result by 100 to find the percent change by using the formula =MULTIPLY(D1, 100).
  
  ![Sheet Used: Calculations](https://user-images.githubusercontent.com/109619716/183372744-5de74448-7154-4f9f-af3f-d6432ed42697.png)
  
    California's yearly wildfire burn acreage rose 421.72% from 2016 to 2021.


# Analysis 2: Which counties had the greatest number of wildfires in 2016 and 2021?
## Data Analysis Process: 
  1) Pay attention to fires that spanned multiple counties. Duplicate sheet "2016".
  2) Sort rows alphabetically from A to Z by "COUNTIES" column. In row 32, El Dorado and Placer are listed in the same cell. Duplicate the row by inserting   a row above and pasting the data. Isolate El Dorado in one "COUNTIES" cell and Placer in the other, with the rest of the cells staying the same.
  3) Do the same for sheet "2021". Duplicate it, and sort rows aphabetically from A to Z by "COUNTIES" column. In row 9, Butte, Plumas, Shasta, Lassen and      Tehama are all listed in the same cell. Repeat the process of step 2, and isolate all 5 counties in seperate rows. Do the same for the clustered            counties in row 23, 89, 92, 116, 158 and 169.
  4) Make a pivot table with the sheet "2016" and lable it "2016 Fire by Counties".
  5) Insert "COUNTIES" into rows and "ACRES" into values. Summarize "ACRES" by COUNTA.
  6) Filter "ACRES" from Z to A to find the county with the greatest number of wildfires. 
  7) Repeat these steps with the sheet "2021," and lable the pivot table "2021 Fire by Counties".
  
  ![Sheet Used: Copy of 2016](https://user-images.githubusercontent.com/109619716/183381227-030e470f-834e-43db-9469-43a1ae559002.png) 
    
    Fresno and Kern both had 12 wildfires in 2016, the largest number.
    
  ![Sheet Used: Copy of 2021](https://user-images.githubusercontent.com/109619716/183386139-539a79e0-886f-4222-8a87-b7415c3d01c4.png)
     
    Riverside had 18 wildfires in 2021, the largest number.
    
    
# Analysis 3: Which county recieved the most funding from Cal Fire grants in 2016 and 2021?
## Data Analysis Process:
  1) From the "2016 Grants by County" sheet, create a pivot table entitled "2016 County Cal Fire Funding".
  2) Input "COUNTIES" into rows and "AMOUNT" into values. Summarize "AMOUNT" by SUM.
  3) Filter data from Z to A by column B to find the county that recieved the most funding from Cal Fire grants in 2016. 
  4) Repeat these steps after making a pivot table for the "2021 Grats by County" sheet, and entitle it "2021 County Cal Fire Funding" to find the county        with the greatest grant funding from Cal Fire in 2021.

  ![Sheet Used: 2016 Grants by County](https://user-images.githubusercontent.com/109619716/183435498-5a0cf251-6083-4db0-b366-9d2cdd7cbece.png)
  
    Fresno received $1,000,000 in grant funding from Cal Fire, the greatest sum of 2016.
    
   ![Sheet Used: 2021 Grants by County](https://user-images.githubusercontent.com/109619716/183437483-50de81bd-2d9c-47d3-a9b3-d6ca65942035.png)

    San Luis Obispo received $4,483,721.09  in grant funding from Cal Fire, the greatest sum of 2021.

# Analysis 4: How has funding of counties through grants changed from 2016 to 2021?
## Data Analysis Process:
   In the "Calculations" sheet, use the (New-Old)/Old x 100 formula to subtract the sum of grant funding in 2021 from the sum in 2016, then divide the result by the sum in 2016. Multiply the result by 100 to find the percent change in grnt funding from 2016 to 2021.
  1) Input the 2016 value in cell A2, and input the 2021 value in cell B2. We will use these for our calculation.
  2) In cell C2, set up the function using the formula =SUM(B2-A2).
  3) In cell D2, divide the output by A1 using the formula =DIVIDE(C2,A2).
  4) In cell E2, multiply the result by 100 to find the percent change by using the formula =MULTIPLY(D1, 100).
    
