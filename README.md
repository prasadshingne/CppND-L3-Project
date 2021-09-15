# CppND-L3-Project

This project is the first step in final project for the Concurrency Part of the Udacity C++ Nanodegree. This is a concurrent traffic simulation and the purpose is to simulate traffic in a city grid with vehicles, streets and intersections. Vehicles drive around randomly and change direction at each intersectoin. Each object in the city grid will run independently in its own thread.

The task is to understand the code base and complete where needed to get this first running version of traffic simulation.

## Overview

<img src="data/Screenshot from 2021-09-15 16-56-25.png" > 

## Project Tasks

* Task L3.1 : In class WaitingVehicles, safeguard all accesses to the private members _vehicles and _promises with an appropriate locking mechanism, that will not cause a deadlock situation where access to the resources is accidentally blocked.
* Task L2.2 : Add a static mutex to the base class TrafficObject (called _mtxCout) and properly instantiate it in the source file. This mutex will be used in the next task to protect standard-out.
* Task L2.3 : In method Intersection::addVehicleToQueue and in Vehicle::drive() ensure that the text output locks the console as a shared resource. Use the mutex _mtxCout you have added to the base class TrafficObject in the previous task. Make sure that in between the two calls to std::cout at the beginning and at the end of addVehicleToQueue the lock is not held.

## Dependencies

* cmake>=2.8
* make >= 4.1 (Linux, Mac), 3.81 (Windows) 
* OpenCV >= 4.1
* gcc/g++ >= 5.4

## Build Instructions

1. Clone this repository
2. Make a build directory: mkdir build && cd build
3. Compile: cmake .. && make
4. Execute: ./traffic_simulation.





