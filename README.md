# NYC-Yellow-Taxi-Sept-2023
Yellow taxi trip records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts. The data used in the attached datasets were collected and provided to the NYC Taxi and Limousine Commission (TLC) by technology providers authorized under the Taxicab & Livery Passenger Enhancement Programs (TPEP/LPEP). The TLC did not create the trip data, and TLC makes no representations as to the accuracy of these data.

## Data Dictionary
- VendorID: is a code indicating the TPEP provider that provided the record.
1= Creative Mobile Technologies, LLC; 2= VeriFone Inc.
- tpep_pickup_datetime: The date and time when the meter was engaged.
- tpep_dropoff_datetime: The date and time when the meter was disengaged.
- Passenger_count: The number of passengers in the vehicle. This is a driver-entered value.
- Trip_distance: The elapsed trip distance in miles reported by the taximeter.
- PULocationID: TLC Taxi Zone in which the taximeter was engaged
- DOLocationID: TLC Taxi Zone in which the taximeter was disengaged
- RateCodeID: The final rate code in effect at the end of the trip.
1= Standard rate
2=JFK
3=Newark
4=Nassau or Westchester
5=Negotiated fare
6=Group ride
- Store_and_fwd_flag: This flag indicates whether the trip record was held in vehicle
memory before sending to the vendor, aka “store and forward,”
because the vehicle did not have a connection to the server.
Y= store and forward trip
N= not a store and forward trip
- Payment_type: A numeric code signifying how the passenger paid for the trip.
1= Credit card
2= Cash
3= No charge
4= Dispute
5= Unknown
6= Voided trip
- Fare_amount: The time-and-distance fare calculated by the meter.
Extra Miscellaneous extras and surcharges. Currently, this only includes
the $0.50 and $1 rush hour and overnight charges.
- MTA_tax: $0.50 MTA tax that is automatically triggered based on the metered
rate in use.
- Improvement_surcharge: $0.30 improvement surcharge assessed trips at the flag drop. The improvement surcharge began being levied in 2015.
- Tip_amount: This field is automatically populated for credit card tips. Cash tips are not included.
- Tolls_amount: Total amount of all tolls paid in trip.
- Total_amount: The total amount charged to passengers. Does not include cash tips.
- Congestion_Surcharge: Total amount collected in trip for NYS congestion surcharge.
- Airport_fee: $1.25 for pick up only at LaGuardia and John F. Kennedy Airports

Acknowledgments
New York City's Taxi & Limousine Commission


## Resources
https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

## Visuals 

### Four Random Categories

![image](https://github.com/MuyiwaNau/NYC-Yellow-Taxi-Sept-2023/assets/34709932/f68a3794-2f16-41f1-b71c-a2c2def7f3aa)

### Pickup Zone, Drop Zone, Time, hour,  Day

![image](https://github.com/MuyiwaNau/NYC-Yellow-Taxi-Sept-2023/assets/34709932/0c3e1d90-96b3-4127-8ac5-abc8e3448d45)

![image](https://github.com/MuyiwaNau/NYC-Yellow-Taxi-Sept-2023/assets/34709932/1e2b0539-eff2-49d1-bce5-300a58b18425)

![image](https://github.com/MuyiwaNau/NYC-Yellow-Taxi-Sept-2023/assets/34709932/8e2570d5-087e-45c3-9c62-c7c80ec13612)

### Trip Counts

![image](https://github.com/MuyiwaNau/NYC-Yellow-Taxi-Sept-2023/assets/34709932/5f8fa1ed-d154-4bc4-a2ac-85cb4492db3f)

### Passenger Counts
![image](https://github.com/MuyiwaNau/NYC-Yellow-Taxi-Sept-2023/assets/34709932/efeff83f-c50d-4164-8ba6-94d0db7fee39)

### Scatter plot for columns with numerical data types against Passenger count 

![image](https://github.com/MuyiwaNau/NYC-Yellow-Taxi-Sept-2023/assets/34709932/d3a25d01-d94e-45d7-86dc-51a9dbe211b0)


### Clustering

![image](https://github.com/MuyiwaNau/NYC-Yellow-Taxi-Sept-2023/assets/34709932/554a0bfe-415b-4949-8a7b-a155caa2786a)

![image](https://github.com/MuyiwaNau/NYC-Yellow-Taxi-Sept-2023/assets/34709932/98189234-5c37-47d9-bb83-d43cd5e4e23e)


- Cluster 0: Short Trippers:
Characteristics: Low passenger count, short trip distance, moderate fare amount, moderate tip amount, minimal tolls, moderate total amount, congestion surcharge present.

- Cluster 1: Long Haul Giants:
Characteristics: High passenger count, very long trip distance, exceptionally high fare amount, no tip, high tolls, extremely high total amount, standard congestion surcharge.

- Cluster 2: City Explorers:
Characteristics: Moderate passenger count, medium trip distance, reasonable fare amount, moderate tip amount, low tolls, moderate total amount, negative congestion surcharge, airport fee present.

- Cluster 3: Urban Adventurers:
Characteristics: High passenger count, short to medium trip distance, high fare amount, moderate tip amount, moderate tolls, high total amount, positive congestion surcharge, longer travel time.

- Cluster 4: Outliers' Odyssey:
Characteristics: Single passenger, extremely long trip distance, low fare amount, high tip amount, no tolls, moderate total amount, standard congestion surcharge.

- Cluster 5: Family Journeys:
Characteristics: Higher passenger count, short trip distance, moderate fare amount, moderate tip amount, minimal tolls, moderate total amount, congestion surcharge present.

- Cluster 6: Luxury Ventures:
Characteristics: Moderate passenger count, long trip distance, high fare amount, very high tip amount, high tolls, very high total amount, moderate congestion surcharge, extended travel time.
