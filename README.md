# Introduction
Hoop and ball model is, as the name suggests, a model consisting of a ball and hoop. The ball can freely rotate in the hoop and the hoop is attached to a motor which allows us to exert a torque on the hoop. This model is used for demonstration and teaching of linear control theory where the goal is to damp the undesired oscillations of the ball. In other words, the goal is to calculate a torque acting against the oscillations based on the measured position of the ball.

The main aim of this page is to provide a thorough manual that would help you to build your own model of 'Ball in hoop'. This model has been developed at the Faculty of Electrical Engineering of the Czech Technical University in Prague in order to demonstrate *numerical optimal control*.

To acquire a more specific notion of what we have been doing, watch these videos: [VIDEOS]

Currently, we have got a fully-functioning model *version 1*, which we would like to redesign to *version 2* and build once again. Subsequent lines describe the model *version 1*. Design changes and developing of the *version 2* will be discussed later.

# Design

## Model Description
[PICTURE]

As it is easily seen in the picture, the main parts of the model are: *hoop* (a holder with motor and its controller is behind the hoop), *Raspberry Pi*, *camera & LEDs module* and a *box of electronics* (containing two power supplies and a module for LEDs control). Everything is attached to an aluminium board by bolts nad nuts. Several parts have been printed in a 3D printer: Raspberry Pi holder, the hoop and a part of the motor controller holder.

The wiring is depicted in the schematic below.
[SCHEMATIC]

## Functions
Raspberry Pi processes an image from the camera, measures the position of a ball, runs a control algorithm and controls the BLDC motor which rotates the hoop. The Raspberry also lits the light. The whole model is switched on by the red switch and the algorithm itself is run by the run button connected to the Raspberry.

## List of components
- Aluminium board

- Motor holder

- BLDC motor GBM6208-150T

- BLDC controller

- Hoop

- Rubber gaskets/o-rings (in the hoop, preventing friction)

- Raspberry Pi holder

- Raspberry Pi 3

- 'Run' button

- Power supplies covering box

- Power supplies: 230 V to 5 V for the Raspberry, 230 V to 27 V for the motor and its regulator

- On/Off switch

- Raspberry Pi Camera module v1

- LED EMOS 12W

- Lamp heat sink

- Metal balls, 20-24 mm in diameter

- Bolts

- Wires

# Software files

## bldc_controller

### controller_board
Includes controller board data.

### py
- commands.py includes definitions of functions

- commandsCAN.py contains defintions of functions

- runFile.py opens serial port

### sensor_board
Includes camera board data.

## cad

### hoop
Pictures and cad files of motor, hoop, bolts, materials etc.

### lampHeatSink
Data of heat sink and light diffuser.

### motorHolder
Cad data of motor holder.

### raspiHolder
Cad data of the holder of the Raspberry Pi.

## doc
A photo of the whole model and its scheme.

## m
Various Matlab files: control, estimation (Kálmán), optimization etc.

## model
Model derivation, Matlab files...

## rpi_posMeas
Position measurement.
