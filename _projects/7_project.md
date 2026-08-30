---
layout: page
title: Himalayan Hazard Early Warning System
description: Autonomous 24/7 cloud-native pipeline monitoring seismic, wildfire, flash flood, and GLOF risks across the Himalayas.
img: assets/img/gee_himalayan_hazard.jpg
importance: 0
category: Applied Research & Learning Projects
related_publications: false
---

### Project Overview

An automated, serverless Decision Support System tailored for high-altitude hazard monitoring across Nepal and the broader Himalayan region. Built using Google Apps Script, Google Earth Engine, and Telegram Webhooks, the pipeline continuously ingests live telemetry from global APIs to evaluate critical environmental thresholds.

### Hazard Vectors Monitored

- **Seismic Activity:** Real-time USGS feeds filter earthquakes (>= 4.0 Mw) across the regional bounding box (26.0°N to 31.0°N, 80.0°E to 89.0°E).
- **Thermal Anomalies:** Ingests NASA VIIRS satellite telemetry to detect high-confidence forest fires.
- **Hydrological Risk:** Tracks 12 strategic Himalayan river corridors using 24-hour rainfall (>= 50 mm) and 3-day soil saturation levels.
- **GLOF Thermal Surges:** Evaluates high-altitude glacial lakes for peak daily thaw temperatures (> 2.0°C).

### Key Technical Features

- **Static Satellite Alert Cards:** Dynamically generates high-resolution satellite imagery overlays centered on event coordinates.
- **Interactive Deep Links:** Every alert delivers inline buttons directing users straight to Google Earth Engine dashboards and Google Maps.
- **Stateful Memory Management:** Utilizes Google PropertiesService to log event IDs and prevent duplicate spamming.
- **Bi-directional Webhook:** Interactive Telegram commands for live status checks.

### Links & Resources

- **GitHub Repository:** [Automated-Hazard-Weather-Check](https://github.com/yadavkeerti/Automated-Hazard-Weather-Check)
- **Interactive GEE Application:** [Live GEE Platform](https://yadavkeerti1199.users.earthengine.app/view/hazardalertinhimalayas)
