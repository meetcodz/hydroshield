# HydroShield Prototype — Quick Start & PPT Walkthrough Guide

This directory contains the lightweight, static, frontend-first prototype of **HydroShield** (AI/ML-Based Integrated Heavy-Rainfall Early Warning & Inundation Prediction System) built for presentation checks, pitch demonstrations, and workflow validation.

---

## 🚀 How to Run the Prototype

No Node.js, Go backend, Python ML pipeline, or database installation is needed! All data is statically modeled and runs directly in your browser.

### Option 1: Direct File Open
Simply double-click [`index.html`](file:///C:/Users/Lenovo/Desktop/SIH2/hydroshield-prototype/index.html) or right-click and select **Open with Chrome / Edge / Firefox**.

### Option 2: Local HTTP Server (Recommended for testing `fetch`)
From PowerShell:
```powershell
cd C:\Users\Lenovo\Desktop\SIH2\hydroshield-prototype
python -m http.server 8000
```
Then navigate to: **`http://localhost:8000`**

---

## 🗺️ Prototype Pages & Features

| Page | URL / File | Key Feature Demonstrated |
|---|---|---|
| **Operations Dashboard** | [`index.html`](file:///C:/Users/Lenovo/Desktop/SIH2/hydroshield-prototype/index.html) | Interactive Leaflet risk zone heatmap, live alerts list, and the **Forecast Timeline Slider (`Now` → `+6h`)** that updates risk severity dynamically. |
| **Inundation Map** | [`inundation.html`](file:///C:/Users/Lenovo/Desktop/SIH2/hydroshield-prototype/inundation.html) | High-resolution flood probability overlay, watershed boundaries, Khan River trace, and an explainable **SHAP contributing factors breakdown** for high-risk wards. |
| **Rainfall Intelligence** | [`rainfall.html`](file:///C:/Users/Lenovo/Desktop/SIH2/hydroshield-prototype/rainfall.html) | Multi-source comparison chart (Ground Radar, IMERG Satellite, ECMWF NWP, Ground Gauge), station table, and short-term forecast. |
| **Alerts & Actions** | [`alerts.html`](file:///C:/Users/Lenovo/Desktop/SIH2/hydroshield-prototype/alerts.html) | Operational triage table, slide-in alert audit drawer, and functional **"Issue New Alert"** workflow modal with real-time UI insertion. |
| **Critical Infrastructure** | [`assets.html`](file:///C:/Users/Lenovo/Desktop/SIH2/hydroshield-prototype/assets.html) | Spatial overlay of hospitals, schools, bridges, roads, and substations, filterable by risk level with detail inspector. |
| **Analytics & Validation** | [`analytics.html`](file:///C:/Users/Lenovo/Desktop/SIH2/hydroshield-prototype/analytics.html) | Model verification metrics (POD, FAR, CSI, Nash-Sutcliffe, ROC-AUC, reliability calibration diagram, forecast error curve). |

---

## 🎬 3-Minute PPT Evaluator Demo Script

1. **Start on Dashboard (`index.html`)**:
   - Point out the institutional operations header (Indore District, Madhya Pradesh, active status).
   - Point out the 4 primary operational KPIs (Rainfall, Flood Risk %, Population at Risk, Assets at Risk).
2. **Interact with the Forecast Timeline**:
   - Drag the timeline slider from **Now** to **+1h**, **+2h**, and **+3h**.
   - Show how the risk level expands: Ward 23 (Vijay Nagar) turns deep crimson (`SEVERE`), and affected assets/population recalculate live.
3. **Inspect Explainability on Inundation Map (`inundation.html`)**:
   - Click on **Ward 23** on the map.
   - Show the panel on the right displaying **82% probability**, **0.45–0.80 m depth**, and the **SHAP contributing factors** (Forecast rainfall, low elevation, soil saturation, drainage distance).
4. **Demonstrate Operational Triage (`alerts.html`)**:
   - Click the **"Issue New Alert"** button.
   - Fill out an alert and click submit to show instant operational dispatch and logging.
5. **Close on Model Reliability (`analytics.html`)**:
   - Show the reliability curve and CSI comparison against traditional optical flow and NWP benchmarks.
