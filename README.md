# CyberShield — Security Operations & Threat Intelligence Dashboard

An advanced, high-performance Security Operations Center (SOC) dashboard designed to visualize and mitigate real-time infrastructure threats, network anomalies, and cyber attacks.

## 🚀 Overview
CyberShield strikes the perfect balance between robust backend data processing and an intuitive, minimalist UI/UX. It converts chaotic, high-volume raw security logs into scannable, actionable intelligence for security analysts, minimizing cognitive fatigue during intense incident responses.

## 🛠️ Architecture & Tech Stack
- **Frontend:** React.js, Tailwind CSS, WebSockets (Asynchronous live-telemetry streaming).
- **Backend (Pipeline):** Python, FastAPI, Docker containers (Log ingestion and filtration layer).
- **Database:** PostgreSQL / TimeScaleDB (Optimized for time-series log retention).

## 💡 Key Features & UX Decisions
- **Data Aggregation & Filtration:** Incoming high-volume noise is filtered at the ingestion layer using Python scripts, compressing thousands of repetitive raw events into lightweight telemetry payloads before rendering.
- **Semantic Color Coding:** Uses a strict dark-mode grid optimized with distinct high-contrast indicators (Critical Red, Warning Orange) to establish immediate visual hierarchy during brute-force or SQL injection attacks.
- **DOM Performance Optimization:** Implements dynamic pagination and selective rendering to guarantee the browser remains 100% responsive even under massive network stress (e.g., 800+ requests/min tracking).

## 🔧 Power-User Features
- **Scalable Design Tokens:** Built entirely using reusable components and modular layouts in Figma, ensuring the UI can scale seamlessly without breaking grid alignment.
- **Dynamic Threshold Rules:** Ingestion filters can be modified on-the-fly via backend environment variables without touching a single line of frontend code.
