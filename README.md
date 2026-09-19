<div align="center">

# 💧 AquaSense IoT System Concept

**Smart irrigation architecture and delivery-planning case study**

[![Architecture](https://img.shields.io/badge/OPEN_ARCHITECTURE-B6FF00?style=for-the-badge&logo=diagramsdotnet&logoColor=07110D)](architecture/SYSTEM-ARCHITECTURE.md)
[![Project Plan](https://img.shields.io/badge/OPEN_PROJECT_PLAN-101820?style=for-the-badge&logo=libreofficecalc&logoColor=B6FF00)](planning/PROJECT-PLAN.csv)
[![Download](https://img.shields.io/badge/DOWNLOAD_CASE_STUDY-B6FF00?style=for-the-badge&logo=github&logoColor=07110D)](https://github.com/Naledi-Reed/aquasense-iot/archive/refs/heads/main.zip)

</div>

## Project position

**Status:** Concept and delivery-planning case study  
**Implementation:** Not presented as a completed hardware or cloud build

AquaSense proposes the use of soil-moisture, temperature, humidity and water-flow sensors to support better irrigation decisions and reduce unnecessary water use.

## Editable project files

| File | Purpose |
|---|---|
| [SYSTEM-ARCHITECTURE.md](architecture/SYSTEM-ARCHITECTURE.md) | Proposed data flow, components and security requirements |
| [PROJECT-PLAN.csv](planning/PROJECT-PLAN.csv) | Editable phases, tasks, dependencies and deliverables |
| [RISK-REGISTER.csv](planning/RISK-REGISTER.csv) | Editable risks, impacts, owners and mitigations |
| [system-summary.md](docs/system-summary.md) | Concise system overview |
| [evidence/](evidence/) | Gantt, fishbone, 6M and risk-matrix visuals |

CSV files can be downloaded and opened directly in Microsoft Excel, Google Sheets or LibreOffice Calc.

## Proposed architecture

```text
Sensors → Microcontroller → Secure messaging → Cloud ingestion
        → Time-series storage → Authenticated dashboard → Alerts
```

## Future milestones

1. Build and calibrate the sensor prototype
2. Add secure MQTT messaging
3. Implement cloud ingestion and storage
4. Develop an authenticated dashboard
5. Add monitoring, testing and deployment automation

## Security requirements

Unique device identity • TLS • secret protection • role-based access • validation • logging • controlled firmware updates

**Module origin:** PMM261 — Project Management  
**Status:** Honest, editable technical planning portfolio
