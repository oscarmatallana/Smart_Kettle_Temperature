# 1. Smart Kettle — Temperature Control Loop in C

A simple educational simulation of a temperature control loop for a household electric kettle.

This project demonstrates how basic control systems work using:
- loops
- conditional logic
- input validation
- process variables
- target states
- safety constraints

Although intentionally simple, the project introduces concepts widely used in real industrial and embedded systems.

---

## Features

- User-defined current and target temperatures
- Operating range validation (0°C – 100°C)
- Heating simulation step by step
- Input validation for non-numeric values
- Simple safety-oriented logic
- Beginner-friendly implementation in C

---

## Concepts Practiced

### Programming Concepts
- Command-line arguments
- Loops (`while`)
- Conditional statements (`if`)
- Integer variables
- Functions
- Input validation
- Memory-safe basic programming

---

### Engineering Concepts
- Temperature control loops
- Setpoints and process variables
- Safety limits
- State progression
- Basic automation logic
- Systems thinking

---

## How to Compile
cc -Wall -Wextra -Werror smart_kettle.c -o smart_kettle

## How to Run
./smart_kettle <current_temperature> <target_temperature>

### Example
./smart_kettle 20 80

Heating from 20°C to 80°C...

- Current temperature: 21°C
- Current temperature: 22°C
- Current temperature: 23°C
...
Current temperature: 80°C

Target temperature reached.

## Edge Cases Considered
- Invalid Temperature Range: ./smart_kettle -5 120
- Non-Numeric Input: ./smart_kettle hello 80
- Water Already Hotter Than Target: ./smart_kettle 90 60
- Missing/Extra Arguments: ./smart_kettle
