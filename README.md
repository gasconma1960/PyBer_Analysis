# PyBer_Analysis
## Background
  V. Isualize has given you and Omar a brand-new assignment. Using your Python skills and knowledge of Pandas, I’ll create a summary DataFrame of the ride-sharing data by city type. Then, using Pandas and Matplotlib, I’ll create a multiple-line graph that shows the total weekly fares for each city type. Finally, I’ll submit a written report that summarizes how the data differs by city type and how those differences can be used by decision-makers at PyBer.V. Isualize has given you and Omar a brand-new assignment. Using your Python skills and knowledge of Pandas, I’ll create a summary DataFrame of the ride-sharing data by city type. Then, using Pandas and Matplotlib, I’ll create a multiple-line graph that shows the total weekly fares for each city type. Finally, I’ll submit a written report that summarizes how the data differs by city type and how those differences can be used by decision-makers at PyBer.
  
# Deliverable 1: A ride-sharing summary DataFrame by city type
## Deliverable 1 Instructions

  Using the Pandas groupby() function with the count() and sum() methods on PyBer DataFrame columns, get the total number of rides, total number of drivers, and the total fares for each city type. Then, calculate the average fare per ride and average fare per driver for each city type. Finally, add this data to a new DataFrame, then format the columns.
  
  *1. Download the PyBer_Challenge_starter_code.ipynb file into your PyBer_Analysis folder and rename it PyBer_Challenge.ipynb.*
  
  ![image](https://user-images.githubusercontent.com/112348240/199862520-db2f0c26-13fe-4d4a-9ab4-fe503c516461.png)
  
  *2. Use the step-by-step instructions below to add code where indicated by the numbered comments in the starter code file.*
  
  *3. **In Step 1,** use the groupby() function to create a Series of data that has the type of city as the index, then apply the count() method to the "ride_id" column. See screenshot below*
  
  ![image](https://user-images.githubusercontent.com/112348240/199867915-238d1d79-d38a-4f61-8ed1-8d69b7d9ad81.png)
  
  *4. **In Step 2,** use the groupby() function to create a Series of data that has the type of city as the index, then apply the sum() method to the "driver_count" column.
   
   ![image](https://user-images.githubusercontent.com/112348240/199862827-50d72174-7a52-49a2-a01c-275cb78c19de.png)
   
   *5. **In Step 3,** use the groupby() function to create a Series of data that has the type of city as the index, then apply the sum() method to the "fare" column.
   
   ![image](https://user-images.githubusercontent.com/112348240/199868676-c822efd7-cbae-45cb-a726-cd7959045dd1.png)

  *6. **In Step 4,** calculate the average fare per ride by city type by dividing the sum of all the fares by the total rides.
  
  ![image](https://user-images.githubusercontent.com/112348240/199872185-cb95ee7e-ffb1-4ed7-a242-00940de0dc84.png)
  
  *7. **In Step 5,** calculate the average fare per driver by city type by dividing the sum of all the fares by the total drivers.
  
  ![image](https://user-images.githubusercontent.com/112348240/199873107-42ce3aaf-3d06-4408-8a69-3dd060d82e5c.png)

  *8. **In Step 6,** create a PyBer summary DataFrame with all the data gathered from Steps 1-5, using the column names shown below:
  
  ![image](https://user-images.githubusercontent.com/112348240/199873444-9b617434-0ab7-497c-8b53-ee35b1230f99.png)
  
    *See screenshot below after I format to look the way it was expected:*
    
  ![image](https://user-images.githubusercontent.com/112348240/199873511-c1d9f3d2-17a9-4d78-a63a-cd3f6193e8a0.png)


