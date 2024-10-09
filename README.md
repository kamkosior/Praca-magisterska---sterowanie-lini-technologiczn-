Praca-magisterska---sterowanie-lini-technologiczna-
 <h2 align="center">  
Praca magisterska - sterowanie linią technologiczną do realizacji wybranych procesów produkcyjnych ram podwozi samochodów elektrycznych. 
</h2>

IN WORK! 

[![video](mgr.jpg)](https://youtu.be/ptrcTcbF7wA)

If you want watch how it works, clik on the screen.

## General Info
The project involves controlling a production line for electric vehicle frames with an emphasis on virtual commissioning. The work includes CAD modeling of the equipment, system control using PLC and industrial robots with consideration of safety, presentation of pneumatic operation, and behavior of the controller depending on the settings. Sensor, actuator, and control systems were selected. Design environments for production lines were compared. Simulation tests of the technological line operation were conducted.

## Technologies
- Tia Portal 
- RobotStudio
- Inventor
- FactoryIO
- FluidSim
- Proneta

## About the Tia Portal 
- [Hardware](#Hardware)
- [Project Tree](#Project-tree)
- [PLC Programm](#PLC-programm)
- [Safety](#Safety)
- [Main Screen](#Main-screen)
- [Fixtures](#Fixtures) 
- [Robots](#Robots) 
- [Turntable](#Turntable) 
- [Magazines](#Magazines)
- [Ground Conveyor](#Ground-conveyor)
- [Washing Machine](#Wash)
- [PID](#PID)
- [Layout](#Layout)
- other systems screens

## About the RobotStudio
- [Model](#Model)
- [Program](#Program)
- [Station Logic](#Station-logic)

## About the Inventor
- [Frame Model](#Frame-Model)
- [Turntable Model](#Turntable-Model)
- [Magazine Model](#Magazine-Model)

## About the FactoryIO
- [PID Model](#PID-Model)

## About the FluidSim
- [FluidSim Model](#FluidSim-Model)

## About the Proneta
- [Hardware Proneta](#Hardware-proneta)

## Hardware
<p align="center">
  <img src="Documentation/1.hardware.jpg">
</p>
In the picture we can see hardware with connections to PLC S7-1500, switches, safety elements, robots modules. 
All modules was addes with relevant GSDML files.

## Project Tree
<p align="center">
  <img src="Documentation/2.tree.jpg">
</p>
Project Tree have folders with operation mode and diagnostic, safety, substations such as: magazines, turntable, fixture, ground conveyor and robots. All folder has FC and FB block depending of the application. 
For each substations used structured PLC tags. In addition was created PLC data types for easier call in data.

## PLC Program
<p align="center">
  <img src="Documentation/3.plc1.jpg">
</p>
In FC block have been made all position for actuators, clamps and detected position.

<p align="center">
  <img src="Documentation/3.plc2.jpg">
</p>
In FB Block have been made steps for all substations. In this block was make also manuals to substations.

<p align="center">
  <img src="Documentation/3.plc3.jpg">
</p>
In the picture we can see Graph sequences with call transitions, positions etc. 
Graph was used, because in my opinion it is clear to find errors and make other instructions.

## Safety
<p align="center">
  <img src="Documentation/4.safety.jpg">
</p>
Safety was maked in dediacated safety block. Used E-Stops, safety doors and acknowledges.

## Main screen
<p align="center">
  <img src="Documentation/5.mainscreen.jpg">
</p>
In main screen we can see all available screens to service line. 

## Fixtures
<p align="center">
  <img src="Documentation/6.fx.jpg">
</p>
In fixtures screen worker can see positions actuators, clamps, sensors and he make control it in manual mode.

## Robots
<p align="center">
  <img src="Documentation/7. robots.jpg">
</p>
In robot screen worker can see positions robots, actual program. Additional can sent robot to home position and cleaning gripper position.

## Turntable
<p align="center">
  <img src="Documentation/30.tt.jpg">
</p>
In this screen table will be start and we can see table position.

## Magazines
<p align="center">
  <img src="Documentation/30.mag.jpg">
</p>
It is the same situation such as in fixtures.

## Ground Conveyor
<p align="center">
  <img src="Documentation/30.gc.jpg">
</p>
In this screen conveyour will be start and we can see which motor sensor is active.

## Washing Machine
<p align="center">
  <img src="Documentation/30.wash.jpg">
</p>
Washing machine is starting in this screen. Additional if sensor detect a frame - we see it on screen.

## PID
<p align="center">
  <img src="Documentation/12.pid.jpg">
</p>
This screen shows how PID works and worker can set parameters.

## Layout
<p align="center">
  <img src="Documentation/11.layout.jpg">
</p>
In this screen we can see all station with safety elements in substations - if circle is red then safety is no fulfilled, and if circle is green then safety is fulfilled. If each circle is green (safety is true) station may be started.

## Model
<p align="center">
  <img src="Documentation/13.rsmodel.jpg">
</p>
This picture show what the station looks like with all elements in simulation in RobotStudio. In this station are: handling robot on the track, handling robot, turntable with two fixtures, two magazines, washing machine and ground conveyor. All elements are fenced by protective barriers.

## Program
<p align="center">
  <img src="Documentation/14.rsprogram.jpg">
</p>
Part of the program for handling robot and turn table is in the picture above.

## Station Logic
<p align="center">
  <img src="Documentation/15.rsstationlogic.jpg">
</p>
Station Logic show how simulation works and wchich elements are conntected with other elements. 

## Frame Model
<p align="center">
  <img src="Documentation/21.rama.jpg">
</p>
This picture shows model CAD car frame with technical drawings. 

## Turn Table Model
<p align="center">
  <img src="Documentation/2.tt.jpg">
</p>
This picture shows model CAD turn table with technical drawings. 

## Magazine Model
<p align="center">
  <img src="Documentation/23.magazin.jpg">
</p>
This picture shows model CAD magaizn with technical drawings. 

## PID Model
<p align="center">
  <img src="Documentation/16.pidfio.jpg">
</p>
This picture shows PID models in Factory IO with regulator diagram in HMI Panel.

## FluidSim Model
<p align="center">
  <img src="Documentation/17.fluidsim.jpg">
</p>
In this photo we can see how actuators works in FLuidSim wit connections to PLC.

## Hardware Proneta
<p align="center">
  <img src="Documentation/18.proneta.jpg">
</p>
Proneta shows hardware in project. It is similar to hardware in Tia Portal, but it's better to make change e.g. IP adress.

## Scheme of operation
<p align="center">
  <img src="Documentation/40.tryby.jpg">
</p>
This photo shows scheme of operation mode. Each substation has individual scheme of operations.

<p align="center">
  <img src="Documentation/40.r1.jpg">
</p>
In this scheme we can see scheme of operation in handling robot no.1.  

