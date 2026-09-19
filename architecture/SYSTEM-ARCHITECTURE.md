# AquaSense Proposed System Architecture

## Data flow

1. Soil-moisture, temperature, humidity and water-flow sensors collect environmental readings.
2. A microcontroller validates and packages the readings.
3. A network connection publishes telemetry to a secure messaging endpoint.
4. Cloud ingestion stores time-series measurements.
5. Rules evaluate thresholds and generate alerts.
6. An authenticated dashboard presents current status, trends and device health.

## Proposed logical components

| Layer | Component | Responsibility |
|---|---|---|
| Device | Sensors | Collect environmental measurements |
| Edge | Microcontroller | Validate, timestamp and transmit data |
| Messaging | MQTT broker or managed equivalent | Receive device telemetry |
| Cloud | Ingestion service | Process and route events |
| Data | Time-series storage | Retain readings and device state |
| Application | Web dashboard | Display status, trends and alerts |
| Security | Identity, encryption and monitoring | Protect devices, data and users |

## Security requirements

- Unique identity for every device
- TLS for data in transit
- Credentials stored outside source code
- Role-based dashboard access
- Input validation and rate limiting
- Audit logs and operational alerts
- Signed or controlled firmware updates
