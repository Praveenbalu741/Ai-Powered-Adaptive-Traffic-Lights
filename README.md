# 🚦 AI-Powered Adaptive Traffic Lights

**Team FALCONS** — Real-Time Urban Mobility Optimizer

An AI-driven traffic signal concept that replaces fixed 30-second timers with adaptive, real-time decision-making — reducing congestion, cutting average wait times, and giving emergency vehicles automatic right-of-way.

🔗 **Live Demo:** [aipoweredadaptivetrafficlights.netlify.app](https://aipoweredadaptivetrafficlights.netlify.app/)

---

## 📌 About This Repository

This repository hosts the **front-end showcase / landing page** for the AI-Powered Adaptive Traffic Lights project, deployed automatically via Netlify.

It's the public-facing entry point for the project — where visitors can view the concept, explore the interface, and access the live demo — while the full AI/ML and simulation stack (described below in [Project Vision](#-project-vision)) is developed as the system's core engine.

### Current Contents

| File / Folder | Purpose |
|---|---|
| `index.html` | Main landing page |
| `assets/` | Static assets (images, styles, scripts) |
| `icons.svg` | Icon sprite sheet |
| `favicon.svg` | Site favicon |

---

## 🚀 Getting Started

To run this site locally:

```bash
git clone https://github.com/Praveenbalu741/Ai-Powered-Adaptive-Traffic-Lights.git
cd Ai-Powered-Adaptive-Traffic-Lights
```

Then simply open `index.html` in your browser, or serve it locally:

```bash
# Using Python
python -m http.server 8000

# Or using Node's http-server
npx http-server .
```

Visit `http://localhost:8000` to view it.

Every push to `main` is automatically deployed to the [live Netlify site](https://aipoweredadaptivetrafficlights.netlify.app/).

---

## 🎯 Project Vision

The full system this landing page represents is designed around one core idea: **traffic signals should think, not just count down.**

At a 4-way intersection (North / South / East / West), simulated CCTV and sensor feeds monitor real-time vehicle density per lane. Instead of fixed timers, an AI decision layer dynamically allocates green-light time to wherever it's needed most — and instantly clears a path for ambulances and fire trucks.

### Planned AI/ML Pipeline

```
Camera / Sensor Feeds
        │
        ▼
Vehicle Detection (OpenCV + YOLOv8)
        │
        ▼
Prediction Layer
   ├─ LSTM/GRU  → forecasts traffic density (next 5–15 min)
   ├─ Random Forest / GBM → congestion & incident risk
   └─ Genetic Algorithm → evolves optimal signal-timing patterns
        │
        ▼
Decision Engine (Deep Q-Network reinforcement learning agent)
   - Learns optimal green-light durations per lane
   - Forces emergency-vehicle priority overrides within seconds
        │
        ▼
Live Signal Actuation → real-time dashboard (WebSocket)
```

### Signature Features (Roadmap)

- 🚑 **Emergency Green Corridor** — automatic signal override with a soft amber buffer, clearing a path for ambulances/fire trucks across multiple intersections
- 🗺️ **Digital Twin Visualization** — animated, physics-based 2D intersection with realistic vehicle motion and signal transitions
- ⚖️ **Fixed-Timer vs. AI Comparison Mode** — live side-by-side proof of reduced wait times
- 🧬 **Genetic Algorithm Evolution Viewer** — watch signal-timing strategies improve across generations
- 🌡️ **Predictive Congestion Heatmap** — 10-minute-ahead forecast of road segment congestion
- 🚨 **Incident Auto-Detection** — flags stalled vehicles / abnormal congestion automatically
- 💬 **Explainable AI Query Panel** — ask "why did East get priority?" and get a plain-English answer from the model's own decision log

---

## 🛠️ Tech Stack (Planned Full System)

| Layer | Technology |
|---|---|
| Backend | Python, FastAPI (REST + WebSocket) |
| AI / ML | PyTorch (DQN, LSTM), DEAP (Genetic Algorithm), scikit-learn |
| Computer Vision | OpenCV, YOLOv8 (Ultralytics) |
| Databases | MySQL, MongoDB, Redis |
| Frontend | React, Vite, Tailwind CSS, Framer Motion, Recharts |
| Deployment | Docker Compose, Netlify (this landing page) |

> This repository currently hosts the static front-end shown above. The backend, simulation engine, and ML models are part of the broader project build and will be integrated as development progresses.

---

## 📊 Why Adaptive Traffic Control?

Fixed-timer signals treat every intersection the same regardless of real conditions. Real-world adaptive systems have shown measurable impact:

- London: up to **25% reduction** in congestion in pilot zones
- Singapore: **20% improvement** in traffic flow
- Los Angeles: **12% reduction** in average travel time
- Spain: **30% reduction** in fatalities in pilot regions

*(Cited as real-world precedent for adaptive traffic systems generally — not a claim about this project's own measured results.)*

---

## 🤝 Contributing

This is an active student/portfolio project. Issues, suggestions, and pull requests are welcome — especially around UI polish, accessibility, and documentation.

---

## 📄 License

Add your preferred license here (e.g., MIT) so others know how they can use this code.

---

## 👤 Team

**FALCONS**
Maintained by [Praveenbalu741](https://github.com/Praveenbalu741)

🔗 [Live Demo](https://aipoweredadaptivetrafficlights.netlify.app/)
