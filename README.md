January Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.jan_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


February Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.feb_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


March Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.mar_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


April Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.apr_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


May Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.may_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


June Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.jun_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


July Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.jul_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


August Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.aug_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


September Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.sep_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


October Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.oct_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


November Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.nov_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


December Calculations: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.dec_tripdata
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC


Total Data Set: 
SELECT 
  avg(timestamp_diff(ended_at, started_at, MINUTE)) as avg_ride_length,
  MAX(timestamp_diff(ended_at, started_at, MINUTE)) AS max_ride_length,
  COUNT(ride_id) AS total_rides,
  member_casual,
  day_of_week
FROM cyclistic-bike-share-409417.trip_data_2023.total_dataset_2023
GROUP BY 
  member_casual, day_of_week
ORDER BY 
  day_of_week ASC
