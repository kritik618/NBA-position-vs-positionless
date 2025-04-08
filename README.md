# NBA Player Role Evolution: Position-Based vs. Positionless Play

## 🏀 Overview

This project analyzes the evolution of NBA player roles over time to explore the question: **Is the NBA becoming positionless?** Using player statistics from multiple seasons and K-means clustering, we investigate whether traditional position-based roles (PG, SG, SF, PF, C) are still valid or if playing styles are converging into a more fluid model.

---

## 📅 Seasons Analyzed
- 2004, 2005, 2006, 2008, 2010, 2014, 2018, 2020, and 2024

---

## 🧪 Methodology

- 📊 **Data Source**: Public datasets from Kaggle containing season-by-season NBA player stats
- ⚙️ **Clustering Algorithm**: K-Means
- 🧼 **Preprocessing**:
  - Column filtering for relevant metrics
  - Imputation of missing values using placeholder -1
  - Standardization for scaling
- 🔍 **Analysis**:
  - Created one clustering model per position per year
  - Visualized player stat distributions within each cluster
  - Compared how stat importance shifted across years

---

## 📊 Features Used

| Feature | Description |
|--------|-------------|
| `PTS` | Total points scored |
| `3P`, `3P%` | 3-point shots and accuracy |
| `AST` | Assists (playmaking ability) |
| `STL` | Steals (defensive disruption) |
| `BLK` | Blocks (rim protection) |
| `ORB`, `TRB` | Offensive & total rebounds |
| `GS` | Games started |
| `FG%`, `eFG%` | Shooting efficiency |

Each stat's priority varies based on the player's position.

---

## 🔍 Position-Based Trait Priorities

This project breaks down trait importance by role (PG, SG, SF, PF, C). For example:

- **Point Guards (PG)**: High emphasis on `AST`, `STL`, and `3P%`
- **Shooting Guards (SG)**: Prioritize `PTS`, `3P`, and `FG%`
- **Centers (C)**: Focused on `TRB`, `BLK`, `FG%`, and `ORB`

These priorities are compared across years to track shifting roles.

---

## 📈 Key Insight

As you move from **2004 to 2024**, visual and clustering results indicate a shift toward **role convergence**, suggesting the NBA is increasingly adopting **positionless basketball** — where skillsets are more balanced and less defined by traditional positions.

---

## 📁 Files
notebooks/ ├── nba_clustering_analysis.ipynb # Full analysis and code


---

## 📦 Requirements

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

