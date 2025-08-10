# Virtual Reality Fitness — Data Engineer Associate (DataCamp)

![Schema](schema.png)

## 📌 Project Overview
This repository contains my solution for the **DataCamp Data Engineer Associate Practical Exam** project: *Virtual Reality Fitness (ActiVR)*.

### Goals
- Perform SQL-based analysis for VR fitness usage data.
- Clean, validate, and prepare data for reporting.
- Generate insights to support a promotional campaign.

### Skills
- SQL
- Data analysis
- Data validation

### Tools
- Python
- Jupyter Notebook (DataCamp Datalab)

---

## 📂 Files
| File | Description |
|------|-------------|
| `notebook.ipynb` | Main analysis and SQL tasks |
| `schema.png` | Database schema diagram |
| `.gitignore` | Ignored files config |
| `README.md` | This file |

---

## 📊 Database Schema
The project database contains 4 tables:
1. **events** – Records of VR game sessions.
2. **games** – Information about games available.
3. **devices** – Hardware details.
4. **users** – Demographics and usage patterns.

![Schema](schema.png)

---

## 🚀 How to Run
1. Open `notebook.ipynb` in Jupyter Notebook or JupyterLab.
2. Run cells in sequential order.
3. Review output tables and plots for insights.

---

## 📝 Results
- *Example insight:* 65% of players prefer cardio-based VR games.
- *Example query:*
```sql
SELECT game_type, COUNT(*) 
FROM events e
JOIN games g ON e.game_id = g.game_id
GROUP BY game_type;
```

---

## 📌 Notes
- Large datasets and temporary files are excluded from this repository.
- The notebook is designed for reproducibility.

