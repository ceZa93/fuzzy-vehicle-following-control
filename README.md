# fuzzy-vehicle-following-control
Fuzzy logic based vehicle following control system using MATLAB/Simulink
This project implements a fuzzy logic controller for maintaining a safe distance between two vehicles.
The following vehicle adjusts its acceleration based on distance error and change of error.

Implementation
  MATLAB / Simulink
  Fuzzy Logic Toolbox

System Overview:
  Reference distance: 100 m
  Initial distance: 70 m
  Lead vehicle speed profile:
    0–10 s: 150 km/h
    10–25 s: linear deceleration to 20 km/h
    25–160 s: 20 km/h

Fuzzy Controller:
  Inputs:
    Distance error (e)
    Change of error (de)
  
  Output:
    Acceleration (a) ∈ [-10, 10] km/h/s
  
  The controller successfully:
    Prevents collision
    Maintains safe following distance
    Handles sudden deceleration of the lead vehicle

How to Run
  Open the .slx file in Simulink
  Run the simulation
  Observe results in Scope blocks
