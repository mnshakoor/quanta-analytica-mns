# Africa Conflict Dashboard

An interactive dashboard for monitoring conflict zones, peacekeeping missions, and instability risks across Africa. Designed for analysts, researchers, and policymakers tracking regional security dynamics.

## 🌍 Overview

This dashboard provides insights into:
- Active conflict zones
- Peacekeeping missions
- Instability risk scores
- Weekly incident tracking
- Custom alert zones (e.g., Ghana–Burkina Faso, Benin, Cameroon)

## 🚀 Features

- Interactive map of conflict zones (Leaflet.js)
- Region filters (West, East, Central, Southern, North Africa)
- Alert notifications for high-risk zones
- Bar chart of weekly incidents
- Pie chart of peacekeeping mission types
- Scorecards for instability metrics

## 🛠️ Setup Instructions

1. Clone the repository:
   git clone https://github.com/yourusername/africa-conflict-dashboard.git
   cd africa-conflict-dashboard

2. Place all JSON data files in the root or /data folder:
   - conflict_zones.json
   - weekly_incident_tracker.json
   - peacekeeping_missions.json
   - instability_risk_scores.json
   - custom_alert_zones.json

3. Open africa_conflict_dashboard_enhanced.html in a browser.

## 📁 File Structure

/data
  ├── conflict_zones.json
  ├── weekly_incident_tracker.json
  ├── peacekeeping_missions.json
  ├── instability_risk_scores.json
  └── custom_alert_zones.json

/dashboard
  └── africa_conflict_dashboard_enhanced.html

## 🌐 GitHub Pages Deployment

1. Go to Settings → Pages in your GitHub repo.
2. Under Source, select the branch and folder (/root or /dashboard).
3. Save and access your dashboard at:
   https://yourusername.github.io/africa-conflict-dashboard
