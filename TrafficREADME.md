# new
Robert Vets
Feb 12, 2015

Traffic is a JavaScript simulation of cars travelling on a single lane road.

The simulation builds an array of car objects that maintain information about position, speed, whether they've completed the trip, who they are behind, and the time of start and finish. The output computes the average speed for all the cars that complete a specified distance of the trip. 

The simulation runs for a predetermined length of time and progresses through incremental time steps, currently set at one minute. At each time step, traffic on the road is advanced in position based upon current speed of travel and a random function determines if a new car enters the road way. The simulation runs to ensure a reasonable number of cars are used in the average.

When a new car is initiated the car array is ammended to add the new car object. Each newly created car has its initial speed (60mph or 1 mile/minute) adjusted with a random variable. As a car advances on a slower car, it checks to see if it would drive into the car in front of it and slows its speed down to match the lead car. Once the car has completed the sample distance, its trip data is calculated and it is effectively no longer part of the simulation, although it will continue to advance in position for the full duration of the simulation's run time.
