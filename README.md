# 30 Seconds Prime numbers Benchmark for Arduino and ESP32

This repository provides a benchmark to measure the performance of Arduino and ESP32 boards in calculating prime numbers within a 30-second timeframe. The code is designed to be efficient and reliable, leveraging optimization techniques to maximize the number of primes found.

## Hardware Requirements

Arduino board (e.g., Uno, Mega, Nano)
ESP32 board (e.g., ESP32 Dev Kit C)
USB cable

## Software Requirements

Arduino IDE
ESP-IDF (for ESP32 development) (or install arduino-esp32 from Board Manager in Arduino IDE)


## How to Use:


### Open the Project:

Arduino: Open the .ino file in the Arduino IDE.
ESP32: Import the project into the ESP-IDF framework and configure the build environment.

### Upload the Code:

Arduino: Connect your Arduino board to the computer and upload the code using the Arduino IDE.
ESP32: Connect your ESP32 board to the computer and flash the firmware using the ESP-IDF tools.

### Run the Benchmark:

Power on the board and open the serial monitor.
The benchmark will start, and the number of primes found within 30 seconds will be displayed.

## Code Optimization

The code incorporates several optimizations to improve performance:

### Early Termination: 
The algorithm checks for divisibility by 2 early on, eliminating even numbers.

### Divisor Increment: 
The divisor is incremented by 2 in each iteration, as even numbers beyond 2 are not prime divisors.

### Efficient Prime Checking: 
The is_prime function uses a loop that iterates up to the square root of the number, reducing unnecessary checks.

## Additional Considerations

Board Performance: The performance of the benchmark can vary depending on the specific board model and clock speed.
Power Consumption: Be mindful of power consumption, especially for battery-powered devices.
Compiler Optimization: Enable compiler optimizations to further improve performance.
Memory Usage: Consider memory constraints, especially for smaller boards.

## Contributing
We welcome contributions to improve the benchmark's accuracy, performance, and user experience. Feel free to submit pull requests or report issues on the GitHub repository.
