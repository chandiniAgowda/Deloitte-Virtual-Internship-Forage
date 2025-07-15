# Deloitte Virtual Internship Forage

This repository contains my submission for the **Deloitte Virtual Job Simulation Program**. In this program, I acted as a Data Analyst intern assisting **Daikibo Industrials**, a global manufacturer of heavy machinery, in solving real-world analytical problems using tools like **Tableau** and **Excel**.

## Task 1: Data Analysis – Telemetry Monitoring

### Client Background
Daikibo Industrials has been collecting telemetry data from 4 factory locations:

- **Meiyo Factory** (Tokyo, Japan)  
- **Seiko Factory** (Osaka, Japan)  
- **Berlin Factory** (Berlin, Germany)  
- **Shenzhen Factory** (Shenzhen, China)  

Each location operates **9 types of machines**, each sending status updates every **10 minutes** throughout **May 2021**.

### Objective
Analyze this telemetry data to answer the following:

1. Which **location** had the **highest machine downtime**?
2. Which **device types** contributed most to that downtime?

### Methodology

- Tool Used: **Tableau**
- Imported data from `daikibo-telemetry-data.json`
- Created a **calculated field** named `Unhealthy` assigning **10 units** to every "unhealthy" status (representing 10 minutes of potential downtime)
- Built:
  - `Down Time per Factory` bar chart
  - `Down Time per Device Type` bar chart
- Combined both into a **Dashboard** with interactivity:
  - Selecting a factory filters device-level breakdown

### Key Deliverable
- An interactive dashboard screenshot identifying:
  - The factory with **most downtime**
  - The machines contributing to it
-  `Result.png`

---

## Task 2: Forensic Technology – Pay Equality Analysis

### Objective
Investigate **gender-based pay equality** across all roles and locations in Daikibo Industrials using data from `Equality Table.xlsx`.

### Dataset Description
The Excel file provided includes:

- `Factory`  
- `Job Role`  
- `Equality Score` (range: -100 to +100; 0 = perfectly fair)

### Solution Approach

Added a **4th column** called `Equality Class` based on rules:

- **Fair** if score is between -10 and +10 (inclusive)
- **Unfair** if score is between -20 to -11 OR 11 to 20
- **Highly Discriminative** if score < -20 OR > 20

### Output
- Updated Excel file with `Equality Class` labels
- `Equality Table Classified.xlsx`

---

## Skills & Tools Applied

- **Tableau**: Data importing, calculated fields, charting, dashboards  
- **Excel**: Data classification, conditional logic  
- **Analytical Thinking**: Problem-solving using real-world datasets  
- **Communication**: Translating technical insights into understandable formats  
