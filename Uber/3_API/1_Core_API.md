The list of APIs need to confirm with the in-scope functional requirements
Considering distributed system architechture, state assumption for a microservices architecture 
and define routes for each api endpoint

```
1. Request a ride : For riders to request a ride from A to B
/POST /rider/fare-estimate -> Partial <Ride>
{
    source, 
    destination
}

2. Confirm ride - Once the rider is satisfied with the estimate, can press "Book" to request a ride
/PATCH /rider/request -> 200 OK
{
    rideId, 
    True/False  
}

3. Drivers confirmation - Drivers receive a notification for new ride, can accept / reject a ride 
/PATCH /driver/accept -> 200 OK
{
    rideId,
    True/False
}

4. Drivers location - Drivers location is updated at regular intervals for map updates and search nearby drivers
/PUT /location/update
{
    lattitude,
    longitude   
}
