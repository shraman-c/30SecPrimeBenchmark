# 30 Seconds Prime Numbers Benchmark for Arduino & ESP32 or similar Microcontroller based boards

This repository provides a benchmark to measure the performance of Arduino boards in calculating prime numbers within a 30-second timeframe. The code is designed to be efficient and reliable, leveraging optimization techniques to maximize the number of primes found.

## Hardware Requirements

- Arduino board (e.g., Uno, Mega, Nano),
- ESP32 board (e.g., ESP32 Dev Kit C),
- USB cable

## Software Requirements

- Arduino IDE
- ESP-IDF (for ESP32 development) (or install arduino-esp32 from Board Manager in Arduino IDE)

## How to Use

### Open the Project
Arduino: Open the .ino file in the Arduino IDE.
ESP32: Import the project into the ESP-IDF framework and configure the build environment.

### Upload the Code
Arduino: Connect your Arduino board to the computer and upload the code using the Arduino IDE.
ESP32: Connect your ESP32 board to the computer and flash the firmware using the ESP-IDF tools.

Select the appropriate board and port from the 'Tools' menu.
Click the 'Upload' button to upload the code to your board.

### Run the Benchmark
Power on the board and open the serial monitor.
The benchmark will start automatically, and the number of primes found within 30 seconds will be displayed.

## Code Optimization
The code incorporates several optimizations to improve performance:

#### Early Termination: The algorithm checks for divisibility by 2 early on, eliminating even numbers.
#### Efficient Looping: Only odd numbers are tested for primality after checking for divisibility by 2.
#### Square Root Limitation: The loop runs up to the square root of the number, reducing the number of iterations.

## Screenshots
### Arduino Uno (Clone - DIP - ATMEL MEGA16u2)

![Arduino UNO DIP](https://github.com/user-attachments/assets/588e7735-2b31-4793-84c6-542d316ee9bf)

### Arduino Uno (Clone - SMD - CH340G)

![Arduino UNO SMD](https://github.com/user-attachments/assets/7c145eba-02be-41ba-9ca1-f91a7f158d47)

### Arduino Nano (Clone -CH340G - Old Bootloader)

![Arduino Nano](https://github.com/user-attachments/assets/c067fc56-4a49-4e6d-8622-dd146ded04c8)

### Arduino Nano (Clone - CH340G - New Bootloader)
![image](https://github.com/user-attachments/assets/5a5a8047-4fe3-4d06-8d59-8185818b3312)


### ESP32-WROOM-32 WCH CH9102 USB to serial bridge chip

![ESP32-WROOM-32 WCH CH9102 USB to serial bridge chip](https://github.com/user-attachments/assets/03af563d-bbac-4f30-8939-cc8f108ad79e)

### ESP32-WROOM-CP2102

![ESP32-WROOM-CP2102](https://github.com/user-attachments/assets/9ebcc3c5-cb6f-4899-957c-9de4456c8a3f)

## Contributing
We welcome contributions to improve the benchmark's accuracy, performance, and user experience. Feel free to submit pull requests or report issues on the GitHub repository.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

**Detailed Changelog**: [Changelog.MD](https://github.com/shraman-c/30SecPrimeBenchmark/blob/main/Changelog.md)
