# PomonaTransitSystem_Java
Pomona Transit System using mySQL and JDBC. 


Used the following tables to design and implement the Pomona Transit System using SQL and JDBC.

  - **Trip** ( TripNumber, StartLocationName, DestinationName)

  - **TripOffering** ( TripNumber, Date, ScheduledStartTime, SecheduledArrivalTime, DriverName, BusID)

  - **Bus** ( BusID, Model,Year)

  - **Driver**( DriverName, DriverTelephoneNumber)

  - **Stop** (StopNumber, StopAddress)

  - **ActualTripStopInfo** (TripNumber, Date, ScheduledStartTime, StopNumber, SecheduledArrivalTime, ActualStartTime, ActualArrivalTime, NumberOfPassengerIn, NumberOf PassengerOut)

  - **TripStopInfo** ( TripNumber, StopNumber, SequenceNumber, DrivingTime)

The system should deal with at least the following transactions:

Display the schedule of all trips for a given StartLocationName and Destination Name, and Date. In addition to these attributes, the schedule includes: Scheduled StartTime, ScheduledArrivalTime , DriverID, and BusID.

Edit the schedule i.e., edit the table of Trip Offering as follows:

- Delete a trip offering specified by Trip#, Date, and ScheduledStartTime;

- Add a set of trip offerings assuming the values of all attributes are given (the software asks if you have more trips to enter);

- Change the driver for a given Trip offering (i.e., given TripNumber, Date, ScheduledStartTime);

- Change the bus for a given Trip offering.

- Display the stops of a given trip (i.e., the attributes of the table TripStopInfo).

- Display the weekly schedule of a given driver and date.

- Add a drive.

- Add a bus.

- Delete a bus.

- Record (insert) the actual data of a given trip offering specified by its key. The actual data include the attributes of the table ActualTripStopInfo.
