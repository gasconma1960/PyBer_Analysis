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
  
  *9. **In Step 7,** use the provided code snippet to remove the index name ("type") from the PyBer summary DataFrame.

  *10.**In Step 8,** format the columns of the Pyber summary DataFrame to look like this:
    
    *See screenshot below after I format to look the way it was expected:*
    
  ![image](https://user-images.githubusercontent.com/112348240/199873511-c1d9f3d2-17a9-4d78-a63a-cd3f6193e8a0.png)
  
# Deliverable 2: A multiple-line chart of total fares for each city type
## Deliverable 2 Instructions
Using your Pandas skills and two new functions, pivot() andresample(), create a multiple-line graph that shows the total fares for each week by city type.
Use the step-by-step instructions below to add code where indicated by the numbered comments in the starter code file:

*1. **In Step 1,** create a new DataFrame with multiple indices using the groupby() function on the "type" and "date" columns of the pyber_data_df DataFrame, then apply the sum() method on the "fare" column to show the total fare amount for each date.

![image](https://user-images.githubusercontent.com/112348240/199874837-9888067b-a858-4696-b752-5a36549e2ac9.png)
![image](https://user-images.githubusercontent.com/112348240/199875010-41ec6ee6-db4b-4897-9a68-efccf5a592ba.png)


*2. **In Step 2,** use the provided code snippet to reset the index. This is needed to use the pivot() function in the next step (Step 3).

![image](https://user-images.githubusercontent.com/112348240/199875202-c45b2623-f7af-4648-9285-0f22e16a773f.png)

![image](https://user-images.githubusercontent.com/112348240/199875303-4129612a-4bb2-4d12-a834-7152f0d6a378.png)


*3. **In Step 3,** use the pivot() function to convert the DataFrame from the previous step so that the index is the "date," each column is a city "type," and the values are the "fare."

  - After this step, you’ll see that each cell has the total fare for the date and time, as shown in the following image.
  
  **Note:** In cells where there is no fare to be summed for that row, the cell will be filled with NaNs.
  
  ![image](https://user-images.githubusercontent.com/112348240/199875479-af506e31-1afe-4218-8828-f932247b52ee.png)
  
*4. **In Step 4,** create a new DataFrame by using the loc method on the following date range: 2019-01-01 through 2019-04-28.

*5. **In Step 5,** use the provided code snippet to reset the index of the DataFrame from the previous step (Step 4) to a datetime data type. This is necessary to use the resample() method in Step 7.


*6. **In Step 6,** use the provided code snippet, df.info(), to check that the "date" is a datetime data type.

*7. **In Step 7,** create a new DataFrame by applying the resample() function to the DataFrame you modified in Step 5. Resample the data in weekly bins, then apply the sum() method to get the total fares for each week.
  - After creating the resampled DataFrame in Step 7, confirm that your DataFrame looks like this:

*8. **Finally, in Step 8,** graph the resampled DataFrame from Step 7 using the object-oriented interface method and the df.plot() method, as well as the Matplotlib "fivethirtyeight" graph style code snippet provided in the starter code. Annotate the y-axis label and the title, then use the appropriate code to save the figure as PyBer_fare_summary.png in your "analysis" folder.

  - Confirm that your multiple-line chart looks like the following image, where each week is a peak or dip in the line graphs.

![image](https://user-images.githubusercontent.com/112348240/199876060-a0bcfb6e-efed-4a8f-ac5a-6de5277175e5.png)



