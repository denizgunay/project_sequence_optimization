# Car Sequence Optimization

This repository contains a Python implementation for solving a vehicle production scheduling optimization problem using Pyomo, an optimization modeling language. The goal is to assign vehicles to production stations over time slots while minimizing the overall completion time at the last station. The model takes into account the demand for each vehicle model, the processing times for each station, and setup times between different colors of vehicles.

## Problem Description

Given a set of vehicles (each with a specific model and color), we need to:

1. **Assign vehicles to time slots and production stations**: Each vehicle must be assigned to a specific station at a specific time slot.
2. **Minimize the total completion time**: The objective is to minimize the completion time at the last production station.
3. **Handle setup times**: Setup times are incurred when a station switches from one vehicle color to another.

The model uses the following data inputs:

- **Demand data**: The number of vehicles required for each model.
- **Processing times**: The time required to process each vehicle model at each production station.
- **Color distribution**: Each vehicle model has a distribution of colors, which affects the setup times between stations.

## Requirements

- Python 3.x
- Pyomo
- Pandas
- Excel (for input data)

You can install the required packages using `pip`:

```bash
pip install pyomo pandas
