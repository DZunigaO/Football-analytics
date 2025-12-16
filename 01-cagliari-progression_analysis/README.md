# Understanding Cagliari Calcio's Relegation: A Data-Driven Analysis of Progression Failures

**Final Project** | Data Science for Football Professionals | University of Edinburgh | 2025

---

## Overview

This project investigates why Cagliari Calcio was relegated from Serie A in the 2021/22 season, with a specific focus on the team's attacking struggles. Using event data from the entire season, I identified critical weaknesses in ball progression that help explain the team's poor results and ultimate relegation.

---

## Problem Statement

The analysis aimed to answer:

- What were the underlying causes of Cagliari's poor attacking output?
- Which specific aspects of play most contributed to their struggles?
- How did player roles and tactical choices affect progression and chance creation?

---

## Methodology

### Data Source
- **Competition:** Serie A 2021/22 season
- **Provider:** IMPECT event data


### Analytical Approach

**1. Season-Level Performance Benchmarking**
- Compared Cagliari's attacking and defensive KPIs against all Serie A teams
- Identified progression metrics as the primary area of weakness
- Established correlation between bypassed opponents and expected goals (xG)

**2. Passing Pattern Analysis**
- Analyzed pass types (low vs. chipped passes) across the league
- Examined the relationship between pass type frequency, accuracy, and defensive pressure
- Identified Cagliari's unusual reliance on high-risk chipped passes

**3. Spatial and Network Analysis**
- Evaluated line-breaking receptions by pitch zone
- Constructed passing networks to visualize team structure and player connections
- Mapped successful passes in the final third to identify progression patterns

**4. Player-Level Assessment**
- Identified key players involved in bypassing opponents (as passers and receivers)
- Analyzed midfield involvement in progression
- Examined how player positioning affected overall team structure

---

## Key Findings

### 1. Progression Deficiency
- **Lowest in the league** for bypassed opponents per successful pass (0.50 vs league average ~0.65)
- **Bottom three** for total successful passes
- **Last place** for line-breaking receptions (52.7 per 90 vs league mean 78.3)

### 2. Pass Type Inefficiency
- **Second-highest reliance on chipped passes** in Serie A
- **Negative correlation** between chipped pass frequency and accuracy
- Lower pressure when attempting chipped passes (18.1% vs league average 19.7%), suggesting tactical choice rather than necessity

### 3. Structural Weakness in Midfield
- Central defenders and forwards dominate progression statistics
- Midfielders underrepresented in both giving and receiving progressive passes
- Progression relies heavily on direct play rather than sustained positional circulation

### 4. Match Context Insights
- More balanced passing distribution and advanced positioning correlated with better results
- Higher bypassed opponents per pass in the successful match vs defeats
- Network analysis revealed more compact, connected structure in winning performance

---

## Technical Skills Demonstrated

**Data Analysis**
- Event data manipulation and feature engineering
- Correlation analysis and benchmarking
- Spatial analysis of pitch positioning

**Visualization**
- Multi-panel comparative plots
- Passing network diagrams with spatial context
- Pitch-based event visualizations
- Statistical scatter plots with trend lines

**Football Analytics Concepts**
- Expected goals (xG) framework
- Progressive passing metrics
- Line-breaking receptions
- Pressure quantification
- Bypassed opponents calculation

**Tools & Technologies**
- Python for data processing and analysis
- Data visualization libraries (Matplotlib/similar)
- Event data handling from IMPECT format

---


## Business Impact & Applications

This analysis demonstrates how data-driven insights can:

1. **Identify root causes** of poor performance beyond surface-level metrics
2. **Quantify tactical tendencies** that may be suboptimal
3. **Provide actionable recommendations** for coaching staff:
   - Reduce reliance on direct, low-success chipped passes
   - Develop midfield involvement in progression
   - Focus training on positional combinations and line-breaking passes
4. **Inform recruitment** by highlighting positional weaknesses

---

## Repository Contents

```
01-cagliari-progression-analysis/
├── README.md                              # This file
├── Cagliari_Analysis_Report.pdf          # Full written report
├── Cagliari_Progression_Analysis.ipynb   # Complete analysis notebook
└── figures/                              # All visualizations
    ├── figure1_season_metrics.png
    ├── figure2_progression_xg.png
    ├── figure3_line_breaking.png
    ├── figure4_pass_types.png
    ├── figure5_pressure.png
    ├── figure6_passing_network.png
    └── figure7_final_third_passes.png
```

---

## How to Use This Repository

### View the Analysis
1. **Quick overview:** Read this README
2. **Full narrative:** See `Cagliari_Analysis_Report.pdf`
3. **Technical details:** Explore `Cagliari_Progression_Analysis.ipynb`

### Run the Code
```python
# Install dependencies
pip install -r requirements.txt

# Open Jupyter notebook
jupyter notebook Cagliari_Progression_Analysis.ipynb
```

**Note:** Raw event data is not included due to licensing restrictions. The notebook includes sample data structures and all analytical code.

---

## Key Takeaways

> "Cagliari's relegation wasn't simply about defending poorly—it was about failing to create chances through cohesive possession. The team's over-reliance on direct, low-probability passes and lack of midfield involvement in progression meant they couldn't consistently threaten opponents."

This project demonstrates the value of multi-level analysis (team, player, match) combined with league-wide benchmarking to identify specific, actionable problems rather than generic performance issues.

---

## Contact

**Diego Zúñiga**
- Email: dazunigaol97@gmail.com
- LinkedIn: [linkedin.com/in/diego-zuniga-data-science](https://www.linkedin.com/in/diego-zuniga-data-science/)

Questions about the methodology, interested in collaboration, or want to discuss football analytics? Feel free to reach out!

---

## Acknowledgments

This analysis was completed as the final project for the **Data Science for Football Professionals** course at the University of Edinburgh (2025). Data provided by IMPECT.

---

*Last Updated: January 2025*
