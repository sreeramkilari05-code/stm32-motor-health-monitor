# STM32 Motor Health Monitoring & Protection System
A real-time embedded motor monitoring and protection system developed using
the STM32F303RE Nucleo board and FreeRTOS.

The system monitors three key motor-health parameters:

- Vibration using MPU-6500
- Current using ACS712
- Temperature using DHT11

The collected sensor data is evaluated against user-defined thresholds.
Depending on the number and severity of abnormal conditions, the system
classifies the motor state as NORMAL, EMERGENCY, or MOTOR KILL.
