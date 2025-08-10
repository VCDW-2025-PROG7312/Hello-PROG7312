# Airport Check-In Simulation Using Custom Queue

You are tasked with developing a C# application to simulate the check-in process at an airport.
 
## Simulation Parameters

### Passenger Details
* There are 100 economy class passengers and 20 business class passengers on a flight

### Check-In Counters
* The airport has 10 check-in counters, with 5 counters are dedicated to economy class passengers, and 5 counters are for business class passengers.
* Each economy class check-in takes 10 minutes per passenger.
* Each business class check-in takes 7 minutes per passenger.

## Simulation Level 1 - No Counter Reallocation
The goal of the simulation is to calculate the total time required to check in all passengers for each class and the whole flight. Counters are not reallocated when not in use.

### Simulation Level 2 - Business Class Counter Reallocation 
The goal of the simulation is to calculate the total time required to check in all passengers for each class and the whole flight. The difference here is that if there are no business class passengers waiting, the business class counters can be reallocated to serve economy class passengers.

## Questions to answer
1. How long will it take to check in all passengers in Level 1?
2. How long will it take to check in all passengers in Level 2?