---
layout: page
title: Himalayan Hazard Early Warning System
description: Autonomous 24/7 cloud-native pipeline monitoring seismic, wildfire, flash flood, and GLOF risks across the Himalayas.
importance: 1
category: Applied Research & Learning Projects
related_publications: false
---

### 🛰️ Project Overview

An automated, serverless Decision Support System tailored for high-altitude hazard monitoring across Nepal and the broader Himalayan region. Built on a cloud-native architecture using Google Apps Script, Google Earth Engine (GEE), and Telegram Webhooks, the pipeline continuously ingests live telemetry from global APIs to evaluate critical environmental thresholds.

---

### Hazard Vectors Monitored

 🌋 Seismic Activity: Real-time USGS feeds filter earthquakes ($\ge 4.0\text{ Mw}$) across the regional bounding box ($26^\circ\text{N}\text{--}31^\circ\text{N}, 80^\circ\text{E}\text{--}89^\circ\text{E}$).
 🔥 Thermal Anomalies: Ingests NASA VIIRS (SNPP) satellite telemetry to detect high-confidence forest fires.
 🌧️ Hydrological Risk: Continuously tracks 12 strategic Himalayan river corridors (e.g., Seti, Narayani, Saptakoshi, Kavre/Roshi Khola) using 24-hour rainfall ($\ge 50\text{ mm}$) and 3-day soil saturation levels.
 🧊 GLOF Thermal Surges: Evaluates high-altitude glacial lakes (Imja Tsho, Tsho Rolpa, Thulagi) for peak daily thaw temperatures ($> 2.0^\circ\text{C}$).

---

### Key Technical Features

 Static Satellite Alert Cards: Dynamically generates high-resolution satellite imagery overlays centered on event coordinates.
 Interactive Deep Links: Every alert delivers inline buttons directing users straight to Google Earth Engine dashboards and Google Maps.
 Stateful Memory Management: Utilizes Google `PropertiesService` to log event IDs and prevent alert duplicate spamming.
 Bi-directional Webhook: Interactive Telegram commands (`/status`, `/check`, `/basins`).

---

### 🔗 Links & Resources

 GitHub Repository: [Automated-Hazard-Weather-Check](https://github.com/yadavkeerti/Automated-Hazard-Weather-Check)
 Interactive GEE Application: [Live GEE Platform](https://yadavkeerti1199.users.earthengine.app/view/hazardalertinhimalayas)
