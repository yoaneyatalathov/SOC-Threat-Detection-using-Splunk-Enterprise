# Splunk Detection Rules

This folder contains the Splunk Search Processing Language (SPL) detection rules developed for this project.

---

## 🔍 Port Scan Detection

**Purpose**

Detects potential port scanning activities by identifying a source IP attempting to connect to multiple destination ports within a short period.

**Log Source**

- Windows Security Log

**Event ID**

- 5157

**Detection Method**

- Signature-Based Detection

**Rule File**

`port-scan-detection.spl`

---

## 💉 SQL Injection Detection

**Purpose**

Detects SQL Injection attempts by identifying common SQL Injection payloads in Apache Access Log requests.

**Log Source**

- Apache Access Log (XAMPP)

**Detection Method**

- Signature-Based Detection

**Rule File**

`sql-injection-detection.spl`

---

## Detection Workflow

```text
Attack
    │
    ▼
Log Collection
    │
    ▼
Splunk Enterprise
    │
    ▼
SPL Detection Rule
    │
    ▼
Dashboard
    │
    ▼
Triggered Alert
```
