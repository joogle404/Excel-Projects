# Data Exploration
### 1. To start with data exploration, I first added a pivot table with the following fields.

![image](https://user-images.githubusercontent.com/97116496/150915830-a29bc2fa-4e84-4048-8b43-73523b6bdae8.png)

### 2. I then applied some basic formatting and inserted a pivot chart (line graph) to get a basic understanding of the data.

![image](https://user-images.githubusercontent.com/97116496/150917140-f681d25d-5671-41a1-857e-07306aeb4328.png)

### 3. On further expanding the line graph to show by months of each quarter, following graph was obtained and it showcased some seasonality.

![image](https://user-images.githubusercontent.com/97116496/150918297-cdde3ae7-bfad-4f9c-a258-aca71aefe473.png)

### 4. Next up, I decided to do a variance analysis to see the year over year growth of Q1 and Q2.

![image](https://user-images.githubusercontent.com/97116496/150921015-512498f9-969f-497e-9c8b-83681317bb0d.png)

### 5. I did a basic forecasting of what Q2 data would be based on the year over year growth percentage of Q1 (Q2 of 2020/(1-growth rate Q1))

![image](https://user-images.githubusercontent.com/97116496/150925039-80637317-e56e-4f29-9336-6d7c90b6cbd1.png)

The result shows that 61% of total volume should've consisted of NAM in Q2. However, a variance(forecasted Q2 data - actual Q2 data) of 4,416 existed, which is 30.6% of total variance.
Here, it is noted that LATAM shows the highest percentage of the total variance to our forecasted data (56.5%).

### 6. After that, By adding CLID to the pivot table, I realized some CLID were missing in certain quarters.

![image](https://user-images.githubusercontent.com/97116496/150968120-46d89b62-af15-44d9-a2eb-fc03d3ca08f4.png)

### 7. I counted the number of clients by region using the COUNTIFS() formula to count the values >0 for each quarter.

![image](https://user-images.githubusercontent.com/97116496/150968243-fe402eaf-976b-4b27-9542-92b8d3883d63.png)

### 8. Looking at the year over Q2 growth rate of LATAM, I find that first two client contribute to the most of the growth.

![image](https://user-images.githubusercontent.com/97116496/152827978-2eae69d2-fc29-4744-84c5-35d1bc5a7072.png)

### 9. Two major clients of LATAM region left in Q2 2021 resulting in major loss of volume (7k).

![image](https://user-images.githubusercontent.com/97116496/152830257-c229e7c1-6980-43ac-8f73-f49e1cba8cbc.png)


