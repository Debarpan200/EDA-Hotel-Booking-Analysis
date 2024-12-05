# Booking.com:Hotel Booking Analysis - EDA

## <ins> Objective </ins>
#### To conduct a comprehensive exploratory data analysis (EDA) on the provided hotel booking dataset to identify key trends, patterns, and correlations among various factors influencing hotel bookings.
## <ins> Dataset </ins>
     We get a dataset of hotel reservations. A city hotel and a resort hotel's reservations are included in this dataset. It has the following features:
     - hotel: Name of hotel ( City or Resort)
     - is_canceled: Whether the booking is canceled or not (0 for no canceled and 1 for canceled)
     - lead_time: time (in days) between booking transaction and arrival.
     - arrival_date_year: Year of arrival
     - arrival_date_month: month of arrival
     - arrival_date_week_number: week number of arrival date.
     - arrival_date_day_of_month: Day of month of arrival date
     - stays_in_weekend_nights: No. of weekend nights spent in a hotel
     - stays_in_week_nights: No. of weeknights spent in a hotel
     - adults: No. of adults in single booking record.
     - children: No. of children in single booking record.
     - babies: No. of babies in a single booking record. 
     - meal: Type of meal chosen 
     - country: Country of origin of customers
     - market_segment: What segment via booking was made and for what purpose?
     - distribution_channel: Via which medium booking was made.
     - is_repeated_guest: Whether the customer has made any booking before(0 for No and 1 for Yes)
     - previous_cancellations: No. of previous canceled bookings.
     - previous_bookings_not_canceled: No. of previous non-canceled bookings.
     - reserved_room_type: Room type reserved by a customer.
     - assigned_room_type: Room type assigned to the customer.
     - booking_changes: No. of booking changes done by customers
     - deposit_type: Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)
     - agent: Id of agent for booking
     - company: Id of the company making a booking
     - days_in_waiting_list: No. of days on waiting list.
     - customer_type: Type of customer(Transient, Group, etc.)
     - adr: Average Daily rate.
     - required_car_parking_spaces: No. of car parking asked in booking
     - total_of_special_requests: total no. of special request.
     - reservation_status: Whether a customer has checked out or canceled,or not showed 
     - reservation_status_date: Date of making reservation status.

Total 119390 rows and 32 columns in dataset
## <ins> Libraries Used </ins>
     - Pandas for data manipulation, aggregation
     - Matplotlib and Seaborn for visualisation and behaviour with respect to the target variable.
     - NumPy for computationally efficient operations
     
## <ins> Data Cleaning</ins>
     - Duplicate records were eliminated,
     - correcting improper data type format which was used in the data, and 
     - missing values were addressed.  
     
## <ins> Exploratory Data Analysis </ins>
     - Analyzing the Data
     - Plotting the DataFrame in the HeatMap to visualize the total count of null values in each column and also if there is any relationship between null values.
     - Replacing null values from Children, Country, & Agents and Dropped Country Column
     - Correcting data type
     - Removing Duplicate Rows
     - Data Visualization

     The following graphs and plots were primarily created using Matplotlib and the Seaborn package.
      - Bar Plots: Compared categorical variables against numerical variables to identify trends.
      - Heatmaps: Visualized the correlation matrix to understand the relationships between numerical variables.
      - Pair Plots: Explored pairwise relationships between some numerical variables.
      - Line Plots + Scatter Plot: line plots are used in showing the trands/count over time period and Scatterplot is used in specifing the data points.

## <ins> Questions which are answered through Visualization </ins>
      - What are the total number of hotel booked Yearly?
      - Total Monthly Booking in 2015, 2016 & 2017?
      - Which Type of Customer Booked Maximum Hotels?
      - Which Top Country Makes the most reservation?
      - Which Hotel type is the Busiest?
      - Total number of reservation cancelled in each type of Hotel?
      - Which Market Segment has maximum and Minimum number of booking?
      - Top 5 agent makes the most number of booking.
      - How many customer don't wish to make a booking with a pre-deposit.
      - Total Number of Repeated Guest both hotels combined. 
      - Correlation Heatmap of Numerical columns
      - Pair plot showing correlation between Guests and Booking Length.

## <ins> Conclusion </ins>
     - The top country with the most number of bookings is PRT.
     - The number one agent with the most number of bookings is 9. 
     - The Maximum hotel bookings are made by new guests. Only less then 5% guests returned.
     - The Online (internet) platform is used to make the majority of bookings.
     - A city hotel is busier than a resort.
     - The busiest months for hotels are August, September and October.
     - Customers do not wish to make a bookings with a pre-deposit.
     - City Hotel have maximum number of booking cancelled as compared to Resort Hotel
     - Guests often book multiple nights, especially for weekends.
     - Longer lead times can result in longer wait times.

## <ins> Challenges Faced </ins>
    - The data contained a large number of duplicates.
    - It was challenging to select the best visualization techniques.
    - The dataset contained a large number of null values.
    - The improper data type format was used for the data.
