# ✈️ Airline Data Management and Analysis Using Power BI

This Power BI project focuses on analyzing airline operations using structured datasets to provide insights into flight schedules, passenger data, and ticket bookings. The project improves operational efficiency and supports decision-making in the airline industry.

---

## 📌 Objective

To manage and analyze flight, passenger, and ticket data using Power BI in order to:
- Optimize airline operations
- Monitor booking trends
- Improve passenger management
- Deliver interactive visual reports and dashboards

---

## 📁 Datasets Used

1. **Flight Information**:  
   Includes FlightID, FlightNumber, Airline, Destination, and Status  
2. **Passenger Information**:  
   Includes PassengerID, FlightID, SeatNumber  
3. **Ticket Information**:  
   Includes TicketID, FlightID, BookingStatus

*Source: Google Sheets (linked in the assignment)*

---

## 🧹 1. Data Preparation & Cleaning

- Data imported and transformed in **Power Query Editor**
- Cleaned: Removed duplicates, filled missing values, formatted columns
- Applied trimming and data-type changes

---

## 🔗 2. Data Modeling

- Created relationships using **FlightID** as the primary key
- Set cardinality: *Many-to-One*
- Applied proper cross-filter direction for accurate data flow

---

## 📊 3. Enhanced Data Insights

- Added **Conditional Column** to classify flights as:
  - `"Best"` → Status = "On Time"
  - `"To Be Improved"` → Else
- Used **Column from Examples** to extract numeric Flight Number from FlightNumber

---

## 🧮 4. DAX Calculations

- `TotalPassengers`: Count of PassengerIDs for a specific flight  
- `TotalTicketsBooked`: Count of Tickets booked from the Ticket Information table  
- Created a visual table showing only **Best flights** using filters

---

## 📈 5. Visualizations & Interactions

- **Passenger Count by Airline** (Clustered Column Chart)
- **Ticket Booking Status** (Pie Chart)
- **Flights by Airline and Destination** (Stacked Bar Chart)
- **Interactive Features**:
  - Slicers for Airline and Destination
  - Quick Views using Buttons & Bookmarks
  - Drill-through Pages for Airline-Specific Analysis

---

## 🧩 6. Final Dashboard and Power BI Service (Discussed)

Due to limitations on Power BI Service (e.g., account restrictions), the following features were **discussed theoretically**:

- **Dashboard**: Combined visuals into a single layout with interactive slicers and bookmarks
- **Row-Level Security (RLS)**:
  - Created a role for `Airline A` with the DAX filter `[Airline] = "Airline A"`
  - Described how to assign roles in Power BI Service
- **Scheduled Refresh**:
  - Steps discussed to configure automatic daily refresh at **5 PM**

---

## 🖼️ Dashboard Preview

> *(Please insert dashboard screenshots in `/images` folder and link here)*  
Example:  
![Dashboard Preview](./images/airline-dashboard-preview.png)

---

## 🚀 Tools Used

- Microsoft Power BI
- Power Query Editor
- DAX (Data Analysis Expressions)
- Excel / Google Sheets

---

## 🙋‍♂️ Author

**Shivam Kumar**  
[LinkedIn Profile](https://linkedin.com/in/your-profile)  
Email: your-email@example.com  

---

## 📜 License

This project is for educational and portfolio use only. No sensitive or real airline data is included.
