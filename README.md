# Data-Journalism-Final-Project
This repository documents my analysis of change in California's wildfire spread from 2016 to 2021 and Cal Fire's funding and legislation response.
### Data Analysis Process: 
1) Select the "2021" sheet.
2) Find the sum of the "ACRES" column by selecting it, clicking "data", and selecting "column stats." Scroll down to where "sum" is listed to find value.
3) Replicate this process with the "2016" sheet.
## Analysis 1: How many acres were burned by California wildfires in 2016 and 2021? What is the percent change between the two years?
![Sheet Used: 2021](https://user-images.githubusercontent.com/109619716/183354096-08fbe292-3b3e-4ccd-b42c-14f10d8e5b22.png)
# 2,610,049 acres were burned by wildflowers in California in 2021
![Sheet Used; 2016](https://user-images.githubusercontent.com/109619716/183360610-7848ab9a-1f3c-486b-aa59-a9c0ddf6c7f0.png)
# 492,171 acres were burned by wildflowers in California in 2016

### Data Analysis Process:
In a new sheet called "Calculations", use the (New-Old)/Old x 100 formula to subtract the sum in 2021 from the sum in 2016, then divide the result by the sum in 2016. Multiply the result by 100 to find the percent change in total wildfire acreage from 2016 to 2021.
1) Input the 2016 value in cell A1, and input the 2021 value in cell B1. We will use these for our calculation.
2) In cell C1, set up the function using the formula =SUM(B1-A1).
3) In cell D1, divide the output by A1 using the formula =DIVIDE(C1,A1).
4) In cell E1, multiply the result by 100 to find the percent change by using the formula =MULTIPLY(D1, 100).
![Sheet Used: Calculations](https://user-images.githubusercontent.com/109619716/183369221-6beff603-14f7-4a30-a731-b4e496c75a9b.png)
# California's yearly wildfire burn acreage rose 430.31% from 2016 to 2021.
