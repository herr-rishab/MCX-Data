# Aegis-MCX: MCX Market Intelligence Platform
Aegis-MCX is a DevOps demonstration project using an **MCX market-intelligence web app (Flutter Web)** to show how **accessibility testing in CI/CD** can be correlated with **production monitoring alerts** to reduce alert fatigue and highlight real user-impacting issues.

---

## 📌 Overview

In most DevOps pipelines, accessibility tests and monitoring alerts work independently. This leads to many alerts without clarity on user impact.

**Aegis-MCX connects these two stages**, correlating accessibility test failures with runtime alerts to generate **single, meaningful, high-priority alerts**.

---

## 🎯 Objectives

- Integrate accessibility testing into CI/CD  
- Monitor MCX API performance and reliability  
- Correlate accessibility issues with monitoring alerts  
- Reduce alert noise  
- Improve user-focused reliability  

---

## 🧩 Key Components

### MCX Web App (Flutter)
- Daily Margin (Today, Previous, Difference)
- Market Watch with FUTCOM expiry spreads
- Instruments: ALUMINI, COPPER, CRUDEOIL, GOLD, SILVER, etc.
- Responsive, web-ready UI

### Accessibility Testing
- Lighthouse in CI/CD
- Keyboard navigation, contrast, screen-reader checks
- JSON reports with severity levels

### Monitoring & Correlation
- Prometheus (or mocked alerts)
- Node.js alert correlation engine
- Rule-based prioritization

---

## 🔁 Workflow

1. Code push triggers CI/CD  
2. Flutter web build + accessibility tests  
3. Results stored as JSON  
4. App deployed  
5. Monitoring generates alerts  
6. Aegis correlates alerts + accessibility results  
7. One prioritized alert is sent to the team  

---

## 🧮 Margin Calculation Logic

Total = Initial + ELM + Tender + Delivery
        + Add L/S + Spec L/S + Daily Vol + Annual Vol

Difference = Total − Previous Day Total
