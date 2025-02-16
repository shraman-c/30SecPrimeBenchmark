# Changelog: Prime Number Benchmark Update
## Version Differences:
|            Change           |                           Previous Version                          |                        Updated Version                        |
|:---------------------------:|:-------------------------------------------------------------------:|:-------------------------------------------------------------:|
| Serial Baud Rate            | 115200                                                              | 9600                                                          |
| Prime Checking Optimization | Checked all numbers starting from 2                                 | Skips even numbers (except 2) for efficiency                  |
| Loop Execution              | Prime checking and timing are handled in a while loop inside loop() | Prime checking runs in loop(), and execution halts at the end |
| Progress Output             | Prints . every 2000 primes and \n every 50000                       | No intermediate output during execution                       |
| Handling of Even Numbers    | Checks all numbers, including even ones                             | Skips even numbers directly, except for 2                     |
| Benchmark Restart           | Waits 10 seconds, resets counters, and restarts automatically       | Runs once and stops execution permanently (while(true) {})    |
| Exit Behavior               | Resets i, found, and start after benchmark completion               | Halts execution after completion                              |

## Improvements in Updated Version:
### Performance Enhancement:
Skipping even numbers (except 2) reduces unnecessary calculations, improving efficiency.
Prime checking is limited to numbers up to the square root of num.

### Simplified Benchmark Logic:
Instead of continuous resets, the program now runs for a fixed duration and stops execution.

### More Consistent Timing Mechanism:
The running_seconds variable is recalculated inside the loop, ensuring precise benchmarking.
