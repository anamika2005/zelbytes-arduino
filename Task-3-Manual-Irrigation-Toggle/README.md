Task 3 - Manual Irrigation Toggle (Phase 1 Capstone)

Objective

Develop a manual irrigation controller using Arduino, a push button, relay module, and status LED.

Features

- Debounced push button input
- Relay-controlled irrigation valve
- Status LED indication
- Configurable irrigation duration
- Serial event logging with timestamp
- Release version: v0.1-manual

Hardware Used

- Arduino Uno/Nano
- Push Button
- Relay Module
- LED
- Jumper Wires

Pin Configuration

Component| Pin
Button| D2
Relay| D8
Status LED| D13

Operation

1. Press the manual button.
2. Relay valve activates.
3. Status LED turns ON.
4. Irrigation event is logged in Serial Monitor.
5. After 5 seconds, irrigation stops automatically.
6. Relay and LED turn OFF.

Serial Output Example

[EVENT] Irrigation Started | Timestamp=15 sec since boot

[EVENT] Irrigation Ended | Timestamp=20 sec since boot

Release Tag

v0.1-manual
