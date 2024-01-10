# Trasportation Analytics using MongoDB Atlas and Compass

## Business Overview

MongoDB is a document database designed for highly accessible and scalable web applications. Its flexible schema technique is popular among agile development teams, enabling quick application launches without the hassle of setting up a traditional relational database. MongoDB's document-oriented architecture simplifies data storage for structured and unstructured data, with a format similar to JSON. 

## Objective

This project focuses on exploring MongoDB, a NoSQL database, its basic architecture, data modeling, querying, aggregations, and tools for tasks like Data Analytics, ETL, and Data Visualization.

---

## Dataset Description

The project uses a transportation dataset, including information about truck drivers, routes, cities, trucks, and historical truck schedules. The dataset is organized into several tables:

1. **driver_details**
   - `driver_id`: Unique identifier for each driver
   - `name`: Name of the truck driver
   - `gender`: Gender of the truck driver
   - `age`: Age of the truck driver
   - `experience`: Experience of the truck driver in years
   - `driving_style`: Driving style of the truck driver (conservative or proactive)
   - `ratings`: Average rating of the truck driver on a scale of 1 to 10
   - `vehicle_no`: Number of the driver’s truck
   - `average_speed_mph`: Average speed of the truck driver in miles per hour

2. **truck_details**
   - `truck_id`: Unique identification number of the truck
   - `truck_age`: Age of the truck in years
   - `load_capacity_pounds`: Loading capacity of the truck in pounds
   - `mileage_mpg`: Mileage of the truck in miles per gallon
   - `fuel_type`: Fuel type of the truck

3. **city_details**
   - `city_id`: Unique identification number of the city
   - `city_name`: Name of the city
   - `lat`: Latitude
   - `lon`: Longitude

4. **route_details**
   - `route_id`: Unique identifier of the routes
   - `origin_city_id`: City identification number for the origin city
   - `destination_city_id`: City identification number for the destination
   - `distance(Miles)`: Distance between the origin and destination cities in miles
   - `average_hours`: Average time needed to travel from the origin to the destination in hours

5. **truck_schedule_data**
   - `truck_id`: Unique identifier of the truck
   - `route_id`: Unique identifier of the route
   - `departure_date`: Departure DateTime of the truck
   - `estimated_arrival`: Estimated arrival DateTime of the truck
   - `delay`: Binary variable indicating if the truck’s arrival was delayed (0 for on-time arrival, 1 for delayed arrival)

---

## Tech Stack

- **Language:** `Python`
- **Package:** `PyMongo`
- **Services:** `MongoDB Atlas`, `MongoDB Compass`

---