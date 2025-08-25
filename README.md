# Aircraft Flight Simulation (MATLAB)

This project is a *MATLAB-based aircraft flight simulation*, created while following a YouTube tutorial.  
It models the basic dynamics of an aircraft and simulates flight behavior under different conditions.  

##Tools Used
- MATLAB 
- Simulink  

##MATLAB Code

```matlab
clc
clear all
close all

% Let's import the flight data
load simdata

% Extract the individual columns for the aircraft’s position
x = simdata(:,1);   % x position
z = simdata(:,3);   % z position

% Roll, Pitch, Yaw
roll  = simdata(:,15); % phi
pitch = simdata(:,16); % theta
yaw   = simdata(:,17); % psi

% Now we import this data to Simulink

🎯 Purpose

This repository was created for learning purposes while following a tutorial.
All code was written manually in MATLAB to replicate the results shown in the video.
