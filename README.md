# 🚖 Ola Customer Booking Analysis (Power BI Dashboard)

## 📌 Project Overview  
This project presents an **Exploratory Data Analysis (EDA)** of Ola customer bookings using **Power BI**.  
The aim is to uncover patterns in customer ride behavior, booking success rates, cancellations, vehicle preferences, payment methods, and revenue distribution.  

By leveraging interactive dashboards, this project provides actionable insights to improve:  
- Fleet allocation  
- Customer satisfaction  
- Revenue optimization  
- Operational efficiency  

---

## 📊 Dataset Description  

The dataset contains **100,000+ booking records** with details about customers, rides, payments, and cancellations.  

### **Columns in the Dataset**

| Column Name                  | Description                                                                                  | Key Role |
|-------------------------------|----------------------------------------------------------------------------------------------|----------|
| `Date`                        | Date of the booking                                                                          | - |
| `Time`                        | Time of the booking                                                                          | - |
| `Booking_ID`                  | Unique identifier for each booking                                                           | **Primary Key** |
| `Booking_Status`              | Status of booking: *Success, Canceled by Driver, Canceled by Customer, Driver Not Found*     | - |
| `Customer_ID`                 | Unique identifier for each customer                                                          | **Foreign Key** |
| `Vehicle_Type`                | Type of vehicle booked (*Sedan, SUV, Auto, Bike, E-Bike, etc.*)                             | - |
| `Pickup_Location`             | Ride starting point                                                                          | - |
| `Drop_Location`               | Ride destination                                                                             | - |
| `V_TAT`                       | Vehicle Turnaround Time – time taken by vehicle to reach customer                           | - |
| `C_TAT`                       | Customer Turnaround Time – time taken by customer to board vehicle                          | - |
| `Canceled_Rides_by_Customer`  | Flag/Count of rides canceled by customers                                                    | - |
| `Canceled_Rides_by_Driver`    | Flag/Count of rides canceled by drivers                                                      | - |
| `Incomplete_Rides`            | Flag indicating incomplete rides (not finished successfully)                                | - |
| `Incomplete_Rides_Reason`     | Reason why the ride was incomplete (technical issue, wrong address, etc.)                   | - |
| `Booking_Value`               | Value of the booking in local currency                                                       | - |
| `Payment_Method`              | Mode of payment (*Cash, UPI, Credit Card, Debit Card*)                                      | - |
| `Ride_Distance`               | Distance travelled during the ride (in km)                                                   | - |
| `Driver_Ratings`              | Rating given to the driver by the customer                                                  | - |
| `Customer_Rating`             | Rating given to the customer by the driver                                                  | - |
| `Vehicle Images`              | Image reference for the booked vehicle type                                                  | - |

---

## 📈 Dashboard Features  

The dashboard is divided into **5 key sections**:  

### 1️⃣ Overall Performance  
- Total Bookings: **103,024**  
- Total Booking Value: **₹35M**  
- Booking Status Breakdown (62% Success, ~18% Driver Canceled, ~10% Customer Canceled, ~10% Driver Not Found)  
- Ride Volume Trend over time  

📌 **Insight:** A majority of bookings are successful, but cancellations by drivers contribute to lost revenue.  

![Ola Customer Booking Analysis_page-0001](https://github.com/user-attachments/assets/60ea4333-3fad-405a-a43c-9c1b798cc7ed)
---

### 2️⃣ Vehicle Type Analysis  
- Booking Value and Success Value split by vehicle type  
- Avg. Distance and Total Distance traveled  
- Comparison of Sedan, SUV, Auto, Bike, E-Bike performance  

📌 **Insight:** Premium vehicles (Sedan, Plus) generate higher booking values, while E-Bikes show promising efficiency with good distance coverage.  

![Ola Customer Booking Analysis_page-0002](https://github.com/user-attachments/assets/f48822e3-a744-41d9-a15e-392027ef5332)
---

### 3️⃣ Revenue Insights  
- Revenue split by Payment Method (Cash dominates, followed by UPI)  
- Top 5 Customers contributing to revenue  
- Ride Distance trend by date  

📌 **Insight:** Digital payments (UPI) are rising but still lag behind cash. Targeting loyal high-value customers can improve retention.  

![Ola Customer Booking Analysis_page-0003](https://github.com/user-attachments/assets/37e3e5d7-61cf-4f27-bc18-fd2ff3f30238)
---

### 4️⃣ Cancellation Analysis  
- Cancellation Rate: **28.08%**  
- Split of cancellations by **Drivers** vs. **Customers**  
- Reasons for cancellations (wrong address, AC not working, change of plans, driver not moving, etc.)  

📌 **Insight:** Driver-related issues are the biggest reason for cancellations, highlighting an operational challenge. 

![Ola Customer Booking Analysis_page-0004](https://github.com/user-attachments/assets/5c742594-d1cc-43f7-8135-8947c8abf223)
---

### 5️⃣ Ratings Analysis  
- **Driver Ratings vs. Customer Ratings** by Vehicle Type  
- Average Ratings hover around **4.0**, but Bikes and E-Bikes slightly underperform  

📌 **Insight:** Consistent ratings show reliability, but Bikes/E-Bikes need service quality improvement.  

![Ola Customer Booking Analysis_page-0005](https://github.com/user-attachments/assets/7d01e3da-4f00-4b22-b124-6008e7d0f20b)
---

## 🛠️ Tools & Technologies  
- **Data Source:** Excel (`Bookings-100000-Rows.xlsx`)  
- **Visualization Tool:** Microsoft Power BI (`Ola Customer Booking Analysis.pbix`)  
- **Techniques:** DAX measures, calculated columns, slicers, filters, drill-downs  

---

## ✅ Key Takeaways  
- Ola has a strong success rate, but **driver cancellations remain a concern**.  
- **Cash is still dominant** in payments, suggesting an opportunity to push digital adoption.  
- **Sedan and Premium vehicles generate the most value**, but **E-Bikes show efficiency potential**.  
- **Customer loyalty programs** can be designed targeting high-value repeat customers.  
- Reducing **operational issues** (driver delays, cancellations, AC problems) will directly boost revenue and satisfaction.  
