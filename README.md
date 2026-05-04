# 🏥 Healthcare Operations & Assessment Performance Analytics

A Power BI analytics project focused on monitoring operational performance across a healthcare assessment lifecycle — from initial client call through to completion.

> **Note:** This was a freelance engagement. All data used in this project is either anonymised or synthetic. No client-identifiable information is included in this repository.

---

## 📌 Project Objective

The client needed visibility into their assessment operations — inspectors were completing assessments at varying rates, turnaround times were inconsistent, and there was no centralised view of the pipeline. The goal was to build a dashboard system that made performance measurable and drop-offs visible.

**Key business questions:**
- How many assessments are at each stage of the lifecycle?
- Which inspectors are performing well, and where are the bottlenecks?
- What is the conversion rate from initial call → assessment → completion?
- Where in the process are drop-offs happening, and why?

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Power BI | Dashboard design, KPI visualisation |
| DAX | Custom measures and calculated columns |
| Amazon Redshift | Source database for operational data |
| Power Query | ETL — data extraction, transformation, load |
| Data Modelling | Relationships across assessment, inspector, and timeline tables |

---

## 🔍 Approach & Methodology

### 1. Data Integration
- Connected Power BI to Amazon Redshift as the data source
- Built Power Query ETL pipelines to extract and transform raw operational data
- Replaced manual data exports with a scheduled refresh model

### 2. Data Modelling
- Designed a star schema with assessment records as the fact table
- Created dimension tables for inspectors, sites, time periods, and assessment stages

### 3. DAX Measures Built
- **Conversion Rate** — call → assessment → completion at each stage
- **Turnaround Time (TAT)** — average days from referral to completion per inspector
- **Productivity Score** — assessments completed per inspector per week
- **Drop-off Rate** — percentage of cases that stall at each lifecycle stage

### 4. Dashboard Design
- Built a multi-page Power BI report with:
  - Executive summary page (overall KPIs)
  - Inspector performance page (individual breakdown)
  - Assessment lifecycle funnel (stage-by-stage drop-off view)
  - Trend analysis page (weekly/monthly performance over time)

---

## 💡 Key Outcomes

- Identified process drop-offs that contributed to delayed completions — addressing these reduced average TAT by ~5%
- Gave operations managers a real-time view of inspector workloads, enabling better allocation
- Replaced a manual weekly reporting process with an automated, always-on dashboard

---

## 📁 Repository Contents

```
Healthcare-Operations-Analytics/
│
├── screenshots/           # Dashboard screenshots (anonymised)
├── dax_measures.md        # All DAX measures used with explanations
├── data_model.png         # Schema diagram of the data model
└── README.md
```

---

## 🧠 What I Learned

- Designing end-to-end BI solutions from raw database to executive dashboard
- Writing complex DAX measures for funnel and conversion tracking
- Working with Amazon Redshift as a live data source in Power BI
- Structuring a data model for operational (non-transactional) use cases

---

## 👩‍💻 About Me

**Nikhitha Nadella** — Data Analyst with 3+ years of experience in banking and financial services.

🔗 [LinkedIn](https://www.linkedin.com/in/nikhithanadella/) | [GitHub](https://github.com/Nikhitha-Nadella) | nikkinadella@gmail.com
