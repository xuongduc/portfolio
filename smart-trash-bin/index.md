---
title: "Portfolio - Phương Xương Đức"
description: "Smart Trash Bin"
---


# Smart Trash Bin

---

## Overview

The **Smart Trash Bin** is an AI-powered prototype that detects and classifies waste items in real time, displays results with a simple GUI, and controls an Arduino-driven sorting mechanism via serial communication. The project demonstrates an end-to-end integration of computer vision (YOLOv8), a lightweight GUI (Pygame), and embedded control (Arduino).

## Key features

- Real-time object detection and classification using a pre-trained **YOLOv8** model (Ultralytics).
- Simple visualization GUI implemented with **Pygame**.
- Serial communication from Python to **Arduino** to command the sorting mechanism.
- Example Arduino sketch to actuate servos or motors based on AI classification.

---

## My role

I was responsible for:

- Implementing the detection pipeline with **YOLOv8** and **OpenCV**.
- Building a simple **Pygame** GUI to visualize detections.
- Sending classification results to Arduino over **serial** and designing the serial message protocol.
- Writing the Arduino code to control the bin compartments (servo/motor control).

---

## Technologies

- Python 3.11+
- ultralytics (YOLOv8)
- OpenCV (cv2)
- Pillow (PIL)
- Pygame
- pyserial
- Arduino (basic C++)

---

## Demonstration Video

<iframe src="https://drive.google.com/file/d/1-wqpGlxZnTiOzT2HyFA41_EjQ1HWaNsS/preview" 
        width="640" height="480" allow="autoplay"></iframe>