# Power-BI
Various analysis and visualisation of individual projects using Power BI

# Customer Call Agent Efficiency Analysis

## 📌 Project Overview
This project analyses
the performance of customer call agents within a specific team. The primary objective is to measure efficiency, identify performance patterns, and generate actionable insights to improve daily operations, enhance customer experience, and optimise resource allocation.

 <img width="700" height="200" alt="Agent Sttatistics" src="https://github.com/user-attachments/assets/e2318f61-1897-4632-a4ac-271544826bee" />

<img width="190" height="380" alt="Average speed of answer " src="https://github.com/user-attachments/assets/25e5bdad-c23a-49e5-a86b-198e7eba1baf" />
<img width="700" height="181" alt="resolved   answered calls" src="https://github.com/user-attachments/assets/6e2ceaa3-7e44-47be-8905-ad98ad7355ff" />

---

## 📁 Dataset Description
- **Source:** [01 Call-Center-Dataset.xlsx](https://github.com/ezemeju-lgtm/Power-BI/blob/main/01%20Call-Center-Dataset.xlsx)
- **Time Period:** Defined range of call records
- **Granularity:** Individual agent-level data
- Interact with the live project here [View Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMjdhZmQyYTUtNmJlYS00MWZkLWE1MmYtZjRiYmY1OGNlZTcyIiwidCI6IjNlYTdjMTI4LWM2MDEtNDQ3OS1hMDAzLWUxNGQwMGMwYjVjYiJ9)


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
