# Aegis

**Aegis** is an integrated DevOps system that combines **accessibility testing in CI/CD pipelines** with **alert correlation** to reduce alert fatigue and improve user-focused application reliability.

---

## 📌 Project Overview

In many DevOps teams, testing and monitoring happen in isolation. Accessibility checks run during CI/CD, and monitoring tools raise alerts in production, but these signals are rarely connected. As a result, teams receive many alerts without clear insight into how real users are affected, which can delay response to important issues.

Aegis connects these two stages by linking accessibility test results with monitoring alerts, helping teams focus on alerts that actually matter and respond faster to problems that impact users.

---

## 🎯 Objectives

- Integrate accessibility testing into the CI/CD pipeline  
- Correlate accessibility issues with monitoring alerts  
- Reduce alert noise using correlation techniques  
- Improve overall software quality and user experience  
- Demonstrate core DevOps automation principles  

---

## 🧩 System Components

### 1. Accessibility Testing Module
- Runs automated accessibility tests during CI/CD
- Uses tools such as Lighthouse or axe-core
- Generates structured test reports (pass/fail, severity)
- Stores results in JSON format

### 2. Alert Correlation Engine
- Ingests alerts from monitoring tools or mocked data
- Groups related alerts
- Suppresses duplicate alerts
- Assigns priority based on correlation rules

### 3. Integration Layer
- Links accessibility test results with monitoring alerts
- Applies rule-based logic
- Generates a single meaningful alert

---

## 🔁 Workflow

1. Developer pushes code to the repository  
2. CI/CD pipeline is triggered  
3. Accessibility tests are executed  
4. Test results are stored  
5. Application is deployed  
6. Monitoring alerts are generated  
7. Alert correlation engine analyzes alerts and test results  
8. A prioritized alert is sent to the DevOps team  

---

## ⚙️ Tech Stack

- **CI/CD:** GitHub Actions / Jenkins  
- **Accessibility Testing:** Lighthouse
- **Monitoring:** Prometheus
- **Backend:** Node.js  
- **Alerting:** Console / Slack / Email  
- **Storage:** JSON

---

## ⚡ DevOps Concepts Used

- Continuous Integration (CI)  
- Continuous Testing  
- Monitoring and Alerting  
- Alert Correlation  
- Automation  
- Feedback Loops  

---

## Team Members

- **Ayan Dafadar**  
	- Accessibility testing integration  
	- CI/CD pipeline configuration  
	- Accessibility severity classification  

- **Rishab Aggarwal**  
	- Alert ingestion  
	- Alert correlation logic  
	- Alert prioritization  

---

## Example Scenario

- Accessibility test fails for keyboard navigation on login
- Monitoring tool reports high latency for authentication service

**Aegis Output:**
> Login service issue detected with accessibility impact – High Priority

---

## Future Enhancements

- Alert visualization dashboard  
- Support for multiple monitoring tools  
- Advanced alert scoring  
- Historical alert analysis  

---

## Conclusion

Aegis demonstrates how accessibility testing and monitoring can be integrated in a DevOps pipeline to provide meaningful alerts, reduce noise, and improve user-focused reliability.

---

This project is developed for academic purposes as part of a DevOps course.