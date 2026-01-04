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


