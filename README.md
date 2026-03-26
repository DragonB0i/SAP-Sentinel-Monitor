# 🛡️ SAP Sentinel: Intelligent Error Monitoring & Resolution

### *AI-Powered Observability for SAP ERP & Master Data Governance (MDG)*

---

## 🚀 Overview

**SAP Sentinel** is a centralized, AI-powered monitoring solution designed to eliminate manual SAP log analysis. It transforms fragmented system logs into **actionable intelligence**, enabling faster detection, smarter root cause analysis, and real-time decision-making.

By leveraging **Large Language Models (LLMs)**, SAP Sentinel continuously scans SAP logs and error tables, correlates related issues, identifies root causes, and recommends corrective actions — all in near real-time.

---

## 🚩 The Problem

SAP ERP and MDG systems rely heavily on manual monitoring across transactions like `ST22`, `SM21`, and `MDG_BS_UI`, which leads to:

* ⏱️ **Delayed Detection** – Critical errors impact downstream processes before being noticed
* 🧑‍💻 **Manual Fatigue** – Thousands of log entries require time-consuming analysis
* 🔍 **Complex Root Cause Analysis** – Linking technical failures to business impact requires expertise

---

## ✨ The Solution

SAP Sentinel converts raw logs into an **intelligent, interactive dashboard**:

* 🧠 **AI Root Cause Analysis (RCA)**
  Interprets SAP error codes into clear technical explanations

* 💼 **Business Impact Mapping**
  Identifies affected domains (Finance, Procurement, Logistics)

* 🔗 **Intelligent Correlation Engine**
  Groups related errors into unified incidents

* 📊 **Risk Distribution Dashboard**
  Visualizes system health across severity levels

* ⚡ **Interactive UI Experience**
  Clickable error cards with deep analysis (Root Cause, Impact, Fix)

---

## 🏗️ System Architecture

A **Hybrid Cloud Architecture** enabling enterprise-grade AI without heavy local hardware:

| Component          | Technology                        | Role                                  |
| ------------------ | --------------------------------- | ------------------------------------- |
| **Frontend**       | React.js, Recharts, Framer Motion | Interactive dashboard & visualization |
| **Backend**        | Flask (Python)                    | REST API & processing logic           |
| **AI Engine**      | Ollama (Mistral-7B)               | Intelligent SAP error analysis        |
| **Infrastructure** | Google Colab                      | Cloud execution (RAM/GPU)             |
| **Gateway**        | Ngrok                             | Secure public API tunnel              |

---

## ⚙️ Setup & Initialization

### 🔹 1. Backend Setup (Google Colab)

1. Open:
   `backend/sap_monitor_backend.ipynb`

2. Install dependencies:

   ```bash
   !pip install flask flask-cors pyngrok ollama
   ```

3. Add your **Ngrok Auth Token**

4. Run all cells

5. Copy generated API URL:

   ```
   https://xxxx-xx.ngrok-free.app
   ```

---

### 🔹 2. Frontend Setup (Local Machine)

1. Navigate to frontend:

   ```bash
   cd frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Update API URL in `src/App.js`:

   ```javascript
   const API_URL = "https://your-ngrok-url.ngrok-free.app";
   ```

4. Start application:

   ```bash
   npm start
   ```

---

## 🎯 Key Features

* ✅ AI-driven SAP log analysis
* ✅ Real-time error monitoring
* ✅ Correlation of related system failures
* ✅ Business impact prioritization
* ✅ Interactive dashboard with charts & insights
* ✅ Modal-based deep error inspection

---

## 🖥️ UI Highlights

* 📊 Severity distribution charts (Pie + Bar)
* 🧾 Error cards with hover & click interactions
* 🔍 Detailed modal with:

  * Root Cause
  * Business Impact
  * Recommended Fix
* 🔗 Correlated error grouping
* 🟢 Live API status indicator
* 🧹 Clear results & re-upload flow

---

## 🛡️ Security & Compliance

Built with enterprise constraints in mind:

* 🔐 **Secure Access** – Uses Ngrok tunneling (no open ports)
* 🧠 **Data Privacy** – Local LLM execution via Ollama
* ⚙️ **Non-Invasive** – Uses standard SAP logs only
* 📋 **Audit Ready** – Clear traceable resolution paths

---

## 📸 Screenshots

> Add your UI screenshots here

```
![Dashboard](./screenshots/dashboard.png)
![Error Analysis](./screenshots/error-modal.png)
![Correlation](./screenshots/correlation.png)
```

---

## 🚀 Future Enhancements

* 🔴 Real-time streaming log monitoring
* 📈 Predictive error detection using ML
* 🔎 Advanced filtering & search
* 🌙 Dark mode enterprise UI
* ☁️ Full cloud deployment (no ngrok dependency)

---

## 👨‍💻 Developed By

**MedBot**
*Intelligent Systems for Enterprise Observability*

---

## ⭐ Final Note

SAP Sentinel is not just a dashboard — it is a step toward **autonomous enterprise monitoring**, where systems don’t just report errors… they **understand and resolve them intelligently**.
