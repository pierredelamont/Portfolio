Total Data Set: 

#Average Ride Length per weekday 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.total_dataset_2023
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC
  

#Average Ride Length per month 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  member_casual,
  EXTRACT(MONTH FROM started_at) AS month,
FROM cyclistic-bike-share-409417.trip_data_2023.total_dataset_2023
GROUP BY 
  member_casual, month
ORDER BY
  month ASC


#Ride Count per weekday
SELECT 
  COUNT(ride_id) AS total_rides, 
  day_of_week,
  member_casual,
FROM cyclistic-bike-share-409417.trip_data_2023.total_dataset_2023
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


#Ride Count per month 
SELECT 
  COUNT(ride_id) AS total_rides, 
  EXTRACT(MONTH FROM started_at) AS month,
  member_casual,
FROM cyclistic-bike-share-409417.trip_data_2023.total_dataset_2023
GROUP BY 
  member_casual, month
ORDER BY
  month ASC


#Average Ride Length per weekday, filtered by rideable type. 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  member_casual,
  day_of_week,
  rideable_type,
FROM cyclistic-bike-share-409417.trip_data_2023.total_dataset_2023
GROUP BY 
  member_casual, day_of_week, rideable_type
ORDER BY 
  day_of_week ASC

  
#Average Ride Length per month, filtered by rideable type. 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  member_casual,
  EXTRACT(MONTH FROM started_at) AS month,
  rideable_type,
FROM cyclistic-bike-share-409417.trip_data_2023.total_dataset_2023
GROUP BY 
  member_casual, month, rideable_type
ORDER BY
  month ASC

  
#Ride Count per month, filtered by rideable type. 
SELECT 
  COUNT(ride_id) AS total_rides, 
  EXTRACT(MONTH FROM started_at) AS month,
  member_casual,
  rideable_type,
FROM cyclistic-bike-share-409417.trip_data_2023.total_dataset_2023
GROUP BY 
  member_casual, month, rideable_type
ORDER BY
  month ASC

  
#Ride Count per weekday , filtered by rideable type. 
SELECT 
  COUNT(ride_id) AS total_rides, 
  day_of_week,
  member_casual,
  rideable_type,
FROM cyclistic-bike-share-409417.trip_data_2023.total_dataset_2023
GROUP BY 
  member_casual, day_of_week, rideable_type
ORDER BY 
  day_of_week ASC
