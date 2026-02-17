# Power-BI
Various analysis and visualisation of individual projects using Power BI

# Customer Call Agent Efficiency Analysis

## 📌 Project Overview
This project analyses the performance of customer call agents within a specific team. The primary objective is to measure efficiency, identify performance patterns, and generate actionable insights to improve daily operations, enhance customer experience, and optimise resource allocation.

---

## 📁 Dataset Description
- **Source:** 01 Call-Center-Dataset.xlsx
- **Time Period:** Defined range of call records
- **Granularity:** Individual agent-level data

### Key Fields Included:
| Field | Description |
|-------|-------------|
| Agent ID / Name | Unique identifier for each agent |
| Calls handled per shift | Total calls managed during shift |
| Average call duration | Mean time spent per call |
| Resolution status | Resolved / Escalated / Follow-up required |
| Customer satisfaction score | Post-call rating (where available) |
| Timestamps | Call start and end times |
| Break times | Scheduled and unscheduled breaks |
| Adherence | Schedule compliance tracking |
| Call type | Inquiry, complaint, technical support, etc. |

---

## 🧹 Data Cleaning & Preparation
Raw call log data required structured cleaning before analysis:

### 1. Handling Missing Data
- Identified incomplete records (missing resolution status, agent IDs)
- Applied exclusion or estimation methods where appropriate

### 2. Standardising Time Data
- Converted timestamps into consistent formats
- Calculated derived metrics:
  ```python
  Call duration = End time - Start time
  Idle time = Next call start - Previous call end
  Time of day patterns = Hourly call distribution
