# aircraft-flight-simulation-matlab
> MATLAB project on Aircraft Flight Simulation based on a YouTube tutorial. Includes modeling of aircraft dynamics and control for basic flight analysis.

(/'/'/' Matlab.../'/'/')
clc
clear all
close all
%%
% let's import the flight data
load simdata
%now let's extract the individual columns for the aircraft's position
time = simdata(:,1)
x = simdata (:, [1,2]) %Extract the x position
y = simdata (:, [1,3]) %Extract the y position
z = simdata (:, [1,4]) %Extract the z position
Roll = simdata (:, [1,5]) %Roll is represented by the greek letter phi
pitch = simdata (:, [1,6]) %Pitch is represented by the greek letter theta
yaw = simdata   (:, [1,7]) %yaw is represented by the greek letter psi
%%
% now we import this data to simulink
