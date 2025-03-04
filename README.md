# Business-Intelligence-AtliQ-Grands-Hospitality-Project
### Project Overview
AtliQ Grands owns multiple five-star hotels across India. They have been in the hospitality industry for the past 20 years. Due to strategic moves from other competitors and ineffective decision-making in management, AtliQ Grands are losing its market share and revenue in the luxury/business hotels category. As a strategic move, the managing director of AtliQ Grands wanted to incorporate “Business and Data Intelligence” to regain their market share and revenue.

This project is part of the Codebasics resume project [challenge](https://codebasics.io/challenge/codebasics-resume-project-challenge).

Please check the - 
-  Live Report
-  Video [Presentation](https://www.loom.com/share/9151008d2af04b9b9cf86112113e1059?sid=ea44697a-0556-4e0a-89a8-23e451f93aa2)

### Key Business Metrics 
 - **Occupancy:** Occupancy means total successful bookings happened to the total rooms available(capacity).
 - **Average Rating:** Average ratings given by the customers.
 - **Total Bookings:** The Total number of Bookings happened.
 - **Total Capacity:** The Total capacity of rooms present in hotels.
 - **Total Successful Bookings:** Total succesful Bookings for all the hotels.
 - **Total Cancelled Bookings:** The "Cancelled" bookings out of all Total bookings happened.
 - **Total No Show Bookings:** No Show means who neither cancelled nor attend to their booked rooms.
 - **Total Checked Out:** Total checked out bookings of all the successful bookings happened.
 - **ADR:** Average Daily Revenue.
 - **Realisation %:** The successful checked out percentage over all bookings happened.
 - **RevPAR:** Revenue Per Available Room.
 - **DBRN:** Daily Booked Room Nights.
 - **DSRN:** Daily Sellable Room Nights.
 - **DURN:** Daily Utilized Room Nights.
 - **Day Type:** Weekday or Weekend.
### Asking the right questions to understand how the stakeholders are going to use the dashboard -
 - What impact it create on the business ?
 - What problems are we trying to solve ?
 - Is there any feedback from stakeholders on the design and views of the dashboard?
### Discovering Datasets 
Lets understand the dataset provided.

We have 3 [dimension](https://www.techtarget.com/searchdatamanagement/definition/dimension-table#:~:text=What%20is%20a%20dimension%20table,defined%20in%20a%20dimensional%20model.) tables and 2 
[fact](https://en.wikipedia.org/wiki/Fact_table) tables as follows -

 - dim_date
     - date
     - week no
     - day type
 - dim_hotels
     - property_id
     - property_name (6 types)
        - AtliQ Grands
        - AtliQ Exotica
        - AtliQ City
        - AtliQ Blu
        - AtliQ Bay
        - AtliQ Palace
     - category (2 types)
        - Luxury
        - Business
     - city (4 cities)
        - Delhi
        - Mumbai
        - Hyderbad
        - Bangalore
  - dim_rooms
     - room_id
     - room_class (4 classes)
         - Standard
         - Elite
         - Premium
         - Presidential

 - fact_aggregated_bookings
     - This table is normalized and contains total successful bookings by total capacity.
 - fact_bookings
     - This table is also normalized and has more details which will help further in building reports.
         - booking date
         - booking status
         - check in date
         - check out date
         - no of guests
         - booking platforms
         - room category
         - ratings given
         - revenue generated
         - revenue realized

  ### Importing the dataset to Power BI
 These datasets are CSV file format. We will import them to Power BI using the folder connector.
  ### Data Model
  For this project Star schema model is used.
<img width="838" alt="Data Model" src="https://github.com/user-attachments/assets/ff735093-96d9-4f54-89eb-39850a65a615" />

### Designing the Dashboard
We have been provided a mock up from the stakeholders as follows - 
<img width="838" alt="Mockup" src="https://github.com/user-attachments/assets/7979e24c-2397-4ffb-b8cd-327ee9b6296c" />

### Now the Output
Here is the 1st page.

<img width="838" alt="Mockup" src="https://github.com/Suy27/Business-Intelligence-AtliQ-Grands-Hospitality-Project-/blob/main/H1.gif" />

And the second page. Everthing is same as the 1st page except the visuals which I have added Donut chart, and stacked column chart.
<img width="838" alt="Mockup" src="https://github.com/Suy27/Business-Intelligence-AtliQ-Grands-Hospitality-Project-/blob/main/H2.gif" />

### Insights and Recommendation  
- **Weekend Pricing Strategy:** 
   - **Observation:** Occupancy rates are significantly higher on weekends compared to weekdays, but the Average Daily Rate (ADR) remains the same.
   - **Recommendation:** The hotel should consider implementing dynamic pricing during weekends to capitalize on higher demand. This will help maximize revenue and avoid potential losses.

- **Performance of Atliq Grands (16558), Delhi:**
  - **Observation:** Atliq Grands in Delhi generated the lowest revenue of 36 million with an average rating of 4.25 and an occupancy rate of 65%.
  - **Recommendation:** To boost revenue, the hotel could offer complimentary services or promotional packages to attract more guests and improve customer satisfaction.

 - **Standard Room Performance:**
    - **Observation:** The Standard room category contributes the lowest revenue at 18% compared to other room types.
    - **Recommendation:** Management should investigate potential issues in inventory management or service quality for Standard rooms. Strategies such as targeted promotions could help improve revenue contribution.

 - **Cancellation Trends in Mumbai:**
    - **Observation:** Mumbai has the highest number of cancellations, particularly during the peak months of May, June, and July.
    - **Recommendation:** The management should analyze the reasons for cancellations (e.g., pricing, external factors, or customer preferences) and implement measures such as flexible cancellation policies or targeted retention offers to reduce cancellations during peak seasons.

Link for the [Report](https://github.com/Suy27/Business-Intelligence-AtliQ-Grands-Hospitality-Project-/blob/main/Hospitality%202.pbix)


















