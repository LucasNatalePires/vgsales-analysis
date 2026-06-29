# 🎮 Video Game Sales Analysis

**Course:** L7 Diploma in Data Analytics and Business — CCT College Dublin  
**Module:** Data Visualization and Communication (CA1)  
**Dataset:** [vgsales.csv](https://www.kaggle.com/datasets/gregorut/videogamesales) — Video Game Sales with Ratings

---

## 📋 Project Overview

This project analyses a video game sales dataset on behalf of a fictional retail company preparing its Autumn sales strategy. The analysis addresses four business questions using Python-based visualizations.

---

## ❓ Questions Answered

| # | Question | Chart Type |
|---|----------|-----------|
| 1 | What are the top 5 games by global sales? | Horizontal Bar Chart |
| 2 | What is the distribution of the top 4 genres? | Bar Chart |
| 3 | Do older games (≤ 2006) have a higher median EU sales? | Box Plot |
| 4 | What are the 3 most common developers? | Bar Chart |

---

## 🔧 Methodology

### Data Cleaning
- Removed duplicate rows
- Dropped rows with <2% null values (`Name`, `Year_of_Release`, `Genre`, `Publisher`)
- Removed columns with >40% missing values (`Critic_Score`, `User_Score`, `Rating`, etc.)
- Replaced null `Developer` values with `'Unknown'` (~39% of rows)

### Feature Engineering
- Created `Developer_Group` column to consolidate studio name variants (e.g., "EA Sports", "EA Games" → "Electronic Arts") — reduced unique entries from 1,681 to 1,441

### Feature Selection
Only features relevant to the four questions were retained for the final analysis.

---

## 📊 Key Findings

- **Wii Sports** leads global sales with 82.5M units, far ahead of any other title
- **Action** is the most common genre, though the classification is broad (e.g., FIFA and GTA both listed as Action)
- **Newer games (post-2006)** have a higher median EU sales than older titles, but also greater variability
- **Electronic Arts** dominates by title count (716), while **Nintendo** achieves comparable revenue with far fewer releases
- All regional markets peaked around 2008–2009 and declined consistently thereafter

---

## 🖼️ Poster

![Poster](poster.png)

---

## 🗂️ Files

| File | Description |
|------|-------------|
| `CA1_Visu_Comu.ipynb` | Jupyter Notebook with full EDA, cleaning, and visualizations |
| `poster.png` | Exported poster image |

---

## 🛠️ Tech Stack

- Python 3
- pandas
- seaborn
- matplotlib
- Jupyter Notebook

---

## 📚 References

Harvard-style references included in the Jupyter Notebook.

Só isso — tabela de arquivos com os dois ficheiros que vão de facto para o repositório.
