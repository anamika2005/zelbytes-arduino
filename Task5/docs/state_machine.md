# State Machine Diagram

## States

1. IDLE
2. MONITORING
3. IRRIGATING
4. COOLDOWN
5. FAULT

## State Transitions

IDLE → MONITORING

MONITORING → IRRIGATING

Condition:
- Soil moisture below SOIL_MIN (25%)
- Low moisture detected 3 consecutive times
- Humidity below HUMIDITY_MAX (85%)

IRRIGATING → COOLDOWN

Condition:
- Soil moisture reaches SOIL_TARGET (40%)

OR

- Maximum runtime reached

COOLDOWN → MONITORING

Condition:
- Cooldown timer expires

ANY STATE → FAULT

Condition:
- DHT sensor fails 3 consecutive readings

FAULT

- Valve OFF
- LED blinks
- System waits for sensor recovery