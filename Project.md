# Lora Cycle Counting Project

## Background

As part of it's transport policy, Birmingham City Council aims to increase the amount of cycling in Birmingham from 2% of journeys  in 2012 to 5% in 2020. Therefore, the city has a need to monitor the number of cyclists using the road and path network in the city.

Automated counting of cyclists can be carried out in a number of different ways, by use of inductive loops, piezo sensors, radar etc. In birmingham it is mostly carried out using inductive loops, using the equipment below.

![Counter Picture](https://github.com/radforaw/cycling/blob/master/IMG_1095.JPG "A Loop Based Cycle Counter")

## Project Aims

The project aims to:
- replace the existing counter setup with an all digital approach
- make use of the Lora network to backhaul the data to an API, for onward processing by the council. 

## Technical Details

The current setup involves an inductive loop cut into the surface of the cycle track. A current runs through the loop and cycles are detected based on changes in the magnetic field. [https://www.fhwa.dot.gov/publications/research/operations/its/06108/02.cfm]. The shape of the loop should enable direction to be calculated.

The loop itself is connected to an on street cabinet, which contains a unit which measures the amount of cyclists and periodically sends the data via a 2G modem to a server.

The unit is powered by 2 battery's (a main battery and a backup). These are connected to a solar panel that sits on top of the unit, via a solar inverter.

![Counter Picture](https://github.com/radforaw/cycling/blob/master/IMG_1178.JPG "Inside the cycle counter box")

The current units have been end of life'd by the manufacturer, hence BCC is looking at options for replacement.

## The project

- BCC will provide access to an existing cabinet, with working loop and solar panel.
 
- The project will aim to use a microcontroller to detect cyclists crossing the loop and then send this data back to BCC making use of the TTN Lora, put in place by BCU.

- The benefits of this will be to avoid the use of a SIM card for sending small amounts of data and to use a microcontroller to improve the accuracy of the cycle detection.

---


