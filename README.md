# Autonomous-Warehouse-Robot


## Overview
This project features a 3D CAD-based robot design created for automating food warehouses using Onshape. The robot includes:
- A mobile base
- Sensors (LiDAR + Camera)
- A 6-DOF robotic arm
- Communication modules

---

## Components

### Hardware
- AGV Base with industrial wheels
- 6DOF Robotic Arm
- LiDAR Sensor
- Camera Module
- Barcode/QR Reader
- Load Cell
- Lithium Battery
- Wi-Fi or ZigBee module

### Software
- ROS2 + Python for robot control
- OpenCV + YOLO for object detection
- A*/Dijkstra for path planning
- SLAM for autonomous navigation
- Flask backend with PostgreSQL

---

## Execution Algorithm

1. **Receive Order**
   - From ERP or warehouse management system

2. **Path Planning**
   - Calculate optimal route to product

3. **Navigation**
   - Use SLAM for localization
   - Avoid obstacles with LiDAR

4. **Pickup**
   - Identify item using vision and barcode
   - Use robotic arm to grab item
   - Validate using load sensor

5. **Delivery**
   - Transport item to packing/shipping zone

6. **System Update**
   - Inventory and operation logs are updated

---

## Working Envelope

### Robotic Arm
- DOF: 6
- Reach: 1.2 meters
- Payload: 10kg
- Movement: 360° base rotation, 180° vertical

### Mobile Base
- Area: up to 30m x 20m
- Speed: 0.5–1 m/s
- Turning Radius: 1m

---

## Folder Structure

- `design/onshape_3d_model/`: Placeholder for 3D model files (.STEP, .SLDPRT, .IGES, etc.)
- `code/`: Software scripts
- `hardware/`: Circuit diagrams, wiring
- `docs/`: Supporting technical documents
