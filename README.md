# POLYMORPHISM-Traffic-Management-System

# Smart Traffic Management System (Polymorphism Case Study)

## Overview
This repository contains a Python implementation of a "Smart Traffic Management System" designed to demonstrate object-oriented programming principles, specifically "polymorphism" and inheritance". 

The system models various intelligent traffic devices that respond to a uniform command (`activate()`) while performing distinct, device-specific behaviors.

## Features & Implementation
* **Parent Class (`TrafficDevice`)**: Acts as the base class establishing a standard interface for all traffic devices.
* **Child Classes**: 
  * `TrafficLight`: Controls intersection signaling.
  * `SpeedCamera`: Captures speeding violations.
  * `PedestrianSignal`: Manages pedestrian crossing alerts.
  * `EmergencySiren`: Triggers emergency sound protocols.
* **Polymorphic Execution**: A single loop iterates through a collection of diverse device objects, triggering their respective `.activate()` methods without needing to check or hardcode their individual types.

## Code Structure
```python
# Core snippet 
for dev in traffic_devices:
    dev.activate()
