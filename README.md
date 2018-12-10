# TempSensor
JDinhGit.github.io/TempSensor

![HTU21D-F Sensor](https://github.com/JDinhGit/TempSensor/blob/master/Documentation/HTU21DF.jpg)

## Table of Contents
1. [Introduction](#introduction)
2. [Time Schedule](#time-schedule)
3. [PCB Design Files](#pcb-design-files)
4. [Assembly for Hardware](#assembly-for-hardware)
5. [PCB Soldering](#pcb-soldering)
6. [Power Up](#power-up)
7. [Testing of Hardware](#testing-of-hardware)


## Introduction
HTU21D-F Temperature/Sensor. This sensors uses the ratio of air moisture to be able to measure and read both temperature and humidity. 
In this tutorial, the goal is to able to activate the senor and have it display readings of the temperature and humidtiy.<br>

![HTU21D-F Sensor Pins](https://github.com/JDinhGit/TempSensor/blob/master/Documentation/HTU21D-f%20sensorpin.jpg)

## Time Schedule
Following the current [budget plan](https://github.com/JDinhGit/TempSensor/blob/master/Documentation/BudgetPlan(Updated).pdf) that is in the the documentations file. Not including the CPU fan, it would take a week for all the supplies necessary for this project. The CPU fan comes in around 2-3 weeks, but it is not needed for this project at the moment. Once everything has arrived, this project would take around 3 - 8 hours to complete, which also includes raspberry pi setup, wiring, and casing. However casing can take longer depending on cutting process for it. Also the wiring images are all done on breadboard and not PCB.<br>

![Budget](https://github.com/JDinhGit/TempSensor/blob/master/Documentation/BudgetPlan(Updated%20Image).jpg)<br>
 
 <b>Wiring</b>
 
| Device Pin| Pi           |
| --------- | ------------ |
| 1 (VIN)   | [5.0v]       |
| 2 (3.3v)  | [3.3v]       |
| 3 (GND)   | [GND]        |
| 4 (SDA)   | [GPIO 2]     |
| 5 (SCI)   | [GPIO 3]     |
<br>
<b>Raspberry pi Pinouts:</b>

![Pinouts](https://github.com/JDinhGit/TempSensor/blob/master/Documentation/raspberry-pi-15b.jpg)<br>
![Wiring](https://github.com/JDinhGit/TempSensor/blob/master/Documentation/IMG_20181023_113450.jpg)<br>

## PCB Design Files
When designing the PCB you would first need a program called fritzing. Fritzing is a application that allows developers to freely design any electronic hardware they choose. With Fritizing however it only has a select amount of hardware provided, therefore the HTU21D-F sensor is not included in fritzing, but you can download it and add it with the link below. 

[Sensor Fritzing](https://github.com/JDinhGit/TempSensor/blob/master/PCB%20Fritzing/Adafruit%20HTU21D-F%20Temperature%20%2B%20Humidity%20Sensor.fzpz)<br>

[Sensor Fritzing Alternative](https://github.com/JDinhGit/TempSensor/blob/master/PCB%20Fritzing/fritzing-adafruit-HTU21DF-master(alternative).zip)<br>

Your diagram should look like this (This is using the alternative sensor).<br>
![Frizting Breadboard](https://github.com/JDinhGit/TempSensor/blob/master/Documentation/HTU21DF%20(Friziting%20Diagram).png)

Keep in mind when designing your PCB design, that the same colours should never touch, and try to use a little pins as possible. 
![PCB Design Hardware](https://github.com/JDinhGit/TempSensor/blob/master/Documentation/HTU21D-F_pcb.png)<br>

You can download the entire frizting gerber file [here](https://github.com/JDinhGit/TempSensor/blob/master/PCB%20Fritzing/HTU21D-F.zip).<br>

## Assembly for Hardware
Well let us begin assembling everything together.

1. First we have to assemble and install the proper UI for the pi. Follow the video below for an easy tutorial.<br>
 ![pi setup](https://www.youtube.com/watch?v=juHoJYX86Dg)

  

## PCB Soldering

## Power Up

## Testing for Hardware
With the code provided in this repository, this test code should get your sensor to read and write temperature/humidity.
[Test Code Link](https://github.com/JDinhGit/TempSensor/tree/master/HTU21D%20-%20Test%20Code/c)<br>
Copy and save it onto your documents using:
insert image code here
