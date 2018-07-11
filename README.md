# Design

## List of components
- Board

- Motor holder

- Hoop

- Rubber o-rings

- Bolts

- BLDC motor GBM6208-150T

- Metal balls, 20-24 mm in diameter

- Raspberry Pi 3

- Power supplies: 230 V to 5 V for the Raspberry, 230 V to approx. 30 V for the motor and regulator

- Box covering power supplies

-  On/Off switch

- Raspberry Pi Camera module v1

- LED EMOS 12W

- Lamp heat sink

- Raspberry Pi holder

- BLDC controller

- BUtton

- 

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
