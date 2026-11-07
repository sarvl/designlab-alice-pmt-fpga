# designlab-alice-pmt-fpga
A project for design laboratory 

## Problem Definition
The detector needs to be tested, which requires test input, which then requires test input driver.
A board was created to allow sending apropriate test pulses, but this board needs a controller.

Microcontrollers in general cannot have high enough timing control to drive the test input.
We will therefore use FPGA.

https://github.com/Design-Laboratory-2025-2026/PMT-SIM

Additionally, the FPGA board is supposed to control the voltage levels using DAC, likely using microprocessor core.

## Operating Environment

As the project is supposed to be a test driver in laboratory, no particularly interesting operating conditions are expected.

## Requirements and Design Constraints

TBD

## Prototype and Implementation 

The project will be implemented on ZYNQ FPGA with PYNQ.

## System Design

AMD FPGA with PYNQ will be used, enabling easy python interface to high speed features provided by FPGA.
The PYNQ will be used to communicate with FPGA based controller and to directly drive GPIO pins used for DAC control.

## Planned Timeline and Milestones

2026-11-15 - communication with DAC with python interface
2026-11-22 - DAC fully tested, finish up the rough edges of initial solution
2026-11-29 - basic plans for pulse generator
2026-12-06 - implementation of pulse generator on FPGA side
2026-12-13 - python communication with the pulse generator
2026-12-20 - finishing up all rough edges, and project finish

## Testing and Validation

TBD
