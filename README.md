Airbnb_analysis
Introduction

This project is an interactive Airbnb Data Visualization Dashboard built using Streamlit, Plotly, Pandas, and MongoDB. It allows users to explore and analyze Airbnb listings based on different filters such as country, property type, room type, and price. The dashboard provides insights into pricing trends, property distribution, host details, and availability.

Technologies Used

Python: For data processing and visualization.

Streamlit: To build an interactive web application.

Pandas: For data manipulation and querying.

Plotly: For creating dynamic visualizations.

MongoDB Atlas: As a cloud-based NoSQL database to store Airbnb listings.

Streamlit Option Menu: For sidebar navigation.

Features

1. Home Page

Displays an overview of the project, including the domain, technologies used, and key objectives.

Provides an introduction to the analysis conducted on Airbnb data.

2. Overview Page

This page contains two tabs:

Raw Data Tab

Displays raw data from MongoDB upon user request.

Users can view the dataset in tabular format.

Insights Tab

Users can filter data based on:

Country

Property Type

Room Type

Price Range

Visualizations include:

Top 10 Property Types: A horizontal bar chart displaying the most listed property types.

Top 10 Hosts with Highest Listings: A bar chart ranking hosts based on the number of properties listed.

Total Listings in Each Room Type: A pie chart showing the proportion of different room types.

Total Listings by Country: A choropleth map visualizing the distribution of Airbnb listings globally.

3. Explore Page

This page allows deeper exploration of Airbnb data through:

Price Analysis

Average Price by Room Type: A bar chart showing the average price for each type of room.

Average Price in Each Country: A scatter geo map depicting average prices across countries.

Availability Analysis

Availability by Room Type: A box plot displaying the distribution of availability across room types.

Average Availability in Each Country: A scatter geo map showing the average availability of listings in different countries.
MongoDB Connection

The project retrieves Airbnb data from MongoDB Atlas. Ensure you update the MongoDB connection string in app.py before running the application.

client = pymongo.MongoClient("your_mongodb_connection_string")
db = client.sample_airbnb
col = db.listingsAndReviews

Usage

Run the Streamlit application and navigate through different pages using the sidebar menu.

Apply filters to analyze specific trends in Airbnb listings.

Explore insights on pricing, availability, and distribution using interactive visualizations.

Conclusion

This project provides a comprehensive and interactive analysis of Airbnb data, enabling users to gain insights into pricing patterns, availability, and host performance. The dashboard enhances decision-making for property owners, travelers, and analysts.
