# STM32 MPU6050 Library with Kalman Filter

This repository contains a complete STM32 library for interfacing with the MPU6050 IMU sensor (Accelerometer + Gyroscope),
with support for Kalman filtering to estimate roll and pitch angles more accurately.

## 🧠 Features

- I2C communication with MPU6050
- Accelerometer and gyroscope raw value readings
- Conversion of raw values to physical units (g, °/s, °C)
- Offset calibration functions
- Real-time angle calculation using:
  - Only accelerometer
  - Only gyroscope (with integration)
  - Sensor fusion with Kalman filter
- Modular C library with header and source separation

## 📁 Folder Structure

```
├── Core
│   ├── Src
│   │   └── main.c                # Example usage
│   └── Inc
│       └── main.h
├── Drivers
│   └── MPU6050
│       ├── mpu6050.c            # MPU6050 source file
│       ├── mpu6050.h            # MPU6050 header file
│       └── mpu6050_register.h   # Register definitions
```

## ⚙️ Requirements

- STM32F4 series microcontroller (tested on STM32F407VET6)
- STM32CubeIDE
- MPU6050 sensor
- I2C communication enabled
- GitHub Desktop or Git for version control

## 🚀 Getting Started

1. Clone this repository or copy the `mpu6050.c`, `mpu6050.h`, and `mpu6050_register.h` files into your STM32 project.
2. Include the necessary header in your `main.c` file.
3. Initialize I2C and MPU6050, perform offset calibration.
4. Use Kalman filter functions to read filtered roll and pitch angles.

## 📷 Demo (optional)
*Include a screenshot or gif here if you have one showing the real-time filtered angles*

## 👨‍💻 Author

- Hüseyin Yanar – [GitHub Profile](https://github.com/)

## 📜 License

This project is licensed under the MIT License.