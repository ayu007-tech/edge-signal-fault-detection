## Project Overview
Industrial machines generate continuous sensor signals such as temperature and vibration.
These signals are affected by noise, drift, and communication delay.
Delayed fault detection can cause equipment damage.

This project designs an edge-based industrial signal monitoring and fault detection system
that processes signals locally using signal conditioning, filtering, and threshold-based logic.



## Sensors and Signal Characteristics

### Temperature Sensor
- Signal type: Analog
- Frequency range: < 1 Hz
- Noise: Sensor drift, low-frequency noise

### Vibration Sensor
- Signal type: Analog
- Frequency range: 10–500 Hz
- Noise: Mechanical and electrical noise

## Sampling Rate Selection

Maximum vibration frequency ≈ 500 Hz  
Nyquist rate = 1000 Hz  
Selected sampling rate = 2000 Hz to reduce aliasing and improve filter performance.

## Noise Sources

| Noise Type | Source |
|----------|--------|
| Gaussian noise | Sensor electronics |
| Drift | Temperature aging |
| Impulse noise | Mechanical shocks |



## System Architecture

The system processes raw sensor signals locally at the edge.
Signal conditioning and filtering remove noise.
Key features are extracted and compared against predefined thresholds.
Only fault alerts are transmitted using MQTT to reduce latency and bandwidth usage.


## ENTC Concepts Involved

- Signals and Systems
- Sampling and Nyquist theorem
- Noise and filtering
- Feature extraction
- Communication latency and reliability
- Embedded edge processing




