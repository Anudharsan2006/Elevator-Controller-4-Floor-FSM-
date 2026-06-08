# 🛗 4-Floor Elevator Controller using Verilog

## Overview

This project implements a 4-floor Elevator Controller using Verilog HDL. The controller accepts floor requests and moves the elevator one floor at a time until the requested destination is reached.

## Features

- 4 Floor Elevator System
- Floor Request Handling
- Upward Movement
- Downward Movement
- Reset Functionality
- Simulation Testbench Included

## Working Principle

The controller compares the requested floor with the current floor.

- If request > current floor → Move Up
- If request < current floor → Move Down
- If request = current floor → Stay Idle

## Project Structure

Elevator-Controller/
│
├── elevator_controller.v
├── elevator_controller_tb.v
├── waveform.png
│
└── README.md

## Inputs

| Signal | Width | Description |
|----------|---------|-------------|
| clk | 1 | System Clock |
| rst | 1 | Active High Reset |
| request_floor | 2 | Destination Floor |

## Outputs

| Signal | Width | Description |
|----------|---------|-------------|
| current_floor | 2 | Current Elevator Position |

## Floor Encoding

| Binary | Floor |
|----------|--------|
| 00 | Floor 0 |
| 01 | Floor 1 |
| 10 | Floor 2 |
| 11 | Floor 3 |

## Example

Current Floor = 0

Request Floor = 3

Movement:

Floor0 → Floor1 → Floor2 → Floor3

## Simulation

Example Requests Tested:

- Floor 3
- Floor 1
- Floor 2
- Floor 0

## Tools Used

- Verilog HDL
- Xilinx Vivado


## Applications

- Elevator Automation Systems
- Building Control Systems
- FSM Learning Projects
- Digital System Design

## Future Improvements

- Door Open / Close Logic
- Emergency Stop
- Overload Detection
- Multi-Request Queue Handling
- Floor Display Module

## Author

**Anudharsan R R**
- VLSI Engineering Student

## License

MIT License
