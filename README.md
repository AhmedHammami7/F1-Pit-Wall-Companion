# 🏁 F1 Pit Wall Companion

**A real-time strategy assistant dashboard for Formula 1 races**  
Built with **Angular**, **.NET (C#)**, **Python**, and **FastF1**

---

## 🚀 Overview

**F1 Pit Wall Companion** simulates the decision-making process of a race strategist. By integrating live telemetry, lap time prediction, and tire degradation modeling, this tool offers strategic insights during an F1 race—mimicking tools used by engineers on the pit wall.

Ideal for F1 fans, data engineers, or anyone interested in motorsport analytics.

---

## 🎯 Features

- 📡 **Real-Time Telemetry Ingestion**  
  Collects and processes data using the FastF1 API (lap times, tire compounds, fuel estimates, driver gaps).

- 📊 **Lap-Time & Tire Degradation Simulation**  
  Predicts lap time evolution over a stint using physics-informed models and compound wear behavior.

- 📅 **Pit Stop Strategy Visualizer**  
  Calculates optimal pit windows and overlays them on live gap charts for decision support.

- 🔁 **Historical Strategy Playback**  
  Simulate and analyze different strategies on past races (what-if tire switches, earlier stops, etc.).

- 🧠 **Modular Architecture**  
  Decouples strategy models (Python) from the web interface (Angular) and backend API (ASP.NET Core).

- 🔐 **Session Management & Auth (Optional)**  
  Login system to save strategy sessions and compare across events.

---

## 🛠 Tech Stack

| Layer         | Technology                                               |
|---------------|-----------------------------------------------------------|
| Frontend      | Angular 16, ng2-charts (Chart.js), Tailwind CSS (optional)|
| Backend API   | ASP.NET Core Web API (C#)                                 |
| Analytics     | Python, FastF1, Pandas, NumPy, SciPy                      |
| Data Storage  | SQL Server or PostgreSQL                                 |
| API Comm      | REST (JSON over HTTP) between Python and .NET            |
| Testing       | xUnit (.NET), Pytest (Python)                            |
| CI/CD (opt)   | GitHub Actions, Docker                                   |

---

## 📁 Project Structure
f1-pit-wall-companion/
│
├── frontend/ # Angular client
│ └── src/
│ └── app/ # Lap charts, pit strategy UI
│
├── backend/ # ASP.NET Core backend
│ └── Controllers/
│ └── Services/
│
├── analytics/ # Python data processing
│ └── strategy/ # Lap time models, tire sims
│
├── database/ # SQL scripts / ORM config
│
└── README.md

## 🎥 Demo Preview

🚧 **Coming soon**  
A demo video will showcase:

- 📈 Lap-time delta chart
- 🧠 Pit strategy planner with stint comparisons
- 📡 Real-time telemetry from a selected Grand Prix

---

## 📚 Reference & Resources

- [FastF1 Documentation](https://theoehrly.github.io/Fast-F1/)
- [Pirelli Tire Data & Race Strategy Guides](https://press.pirelli.com/)
- [F1 Technical Articles & Papers](https://www.motorsportmagazine.com/)

---

## 📌 Roadmap

- ✅ Build telemetry ingestion module with FastF1
- ✅ Implement lap-time simulation model
- ✅ Create Angular dashboard interface
- ✅ Connect .NET backend to Python logic
- ⬜ Integrate authentication and user session saving
- ⬜ Add cloud deployment (Azure / Docker)
- ⬜ Build race replay mode with historical telemetry

---

## 🧪 Testing

Unit tests written using:

- ✅ `xUnit` for .NET backend logic
- ✅ `Pytest` for Python analytics modules

---

## 👤 Author

**Ahmed Hammami**  
🔗 [GitHub](https://github.com/AhmedHammami7) • [LinkedIn](https://www.linkedin.com/in/ahmedhammami7)
