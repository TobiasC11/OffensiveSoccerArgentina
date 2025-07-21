# ⚽ What Distinguishes Offensive Soccer Teams in the Argentine League?
## Comparative Analysis of Style and Performance (2021–2024)

---

## 📌 Introduction

This analysis explores the characteristics of offensive teams in Argentina's Professional League between 2021 and 2024. Using a custom-designed Offensive Index, we compare their statistics with non-offensive teams to assess whether their style translates into better overall performance.

---

## ⚙️ Methodology

### What Is an Offensive Team?

For this study, we created an **Offensive Index** based on **min-max normalization** of various offensive metrics. The index places more weight on **chance creation** (xG, touches in the box, big chances) than on finishing (goals), aiming to capture attacking style, not just scoring efficiency.

Teams were classified as *"offensive"* if their index score was above the 65th percentile for their respective season.

---

## 📊 Comparative Analysis

### 🟩 Overall Performance

- **Average points** per season:
  - Offensive: **60**
  - Non-offensive: **49**

- **Average wins/draws/losses**:
  - Offensive: 16 / 12 / 12
  - Non-offensive: 12 / 12 / 16

- **Average goals per season**:
  - Offensive: **51**
  - Non-offensive: **39**

- **Average possession**:
  - Offensive: **52%**
  - Non-offensive: **47.7%**

<img width="790" height="490" alt="Image" src="https://github.com/user-attachments/assets/df9d276b-5806-4dd6-b6d8-ee39da219e3f" />

---

### 🔵 Offensive Style

- **Total shots per season**:
  - Offensive: **266**
  - Non-offensive: **227**

- **Shot accuracy (SoT%)**:
  - Offensive: **31.8%**
  - Non-offensive: **30.5%**

---

### 🔴 Defensive Aspects

- **xG conceded per season**:
  - Offensive: **20**
  - Non-offensive: **14**

- **Clean sheets per season**:
  - Offensive: **6.5**
  - Non-offensive: **7**

- **Interceptions per match**:
  - Both groups average **10**

📌 *Preliminary conclusion*:
> An offensive style does not appear to significantly penalize defensive performance, although offensive teams concede more xG, likely due to taking greater risks.

---

## 🧠 Reflections and Limitations

Data was gathered from various public sources using scraping techniques (FBref, Fotmob, etc.), with notable limitations for South American leagues. This restricted the depth of some parts of the analysis.

**Limitations**:
- Seasonal inconsistencies or missing data
- Lack of play-by-play event data
- No control for factors like home advantage, opponent quality, or tactics

### Next Steps:
We are developing a model to analyze how forward performance varies when transferring from a non-offensive to an offensive team, which is not included in this report.

---

## 📊 Appendix: Offensive Index Weights

Below are the weights assigned to each statistic in building the index:

### 🔹 Finishing and Goals (Total: 30%)
| Metric                                | Weight |
|---------------------------------------|--------|
| Total Goals (`Standard_Gls`)          | 10%    |
| Goals per Shot (`Standard_G/Sh`)      | 10%    |
| Goals per Shot on Target (`Standard_G/SoT`) | 2.5%  |
| Shot Accuracy (`Standard_SoT%`)       | 2.5%   |
| Shots on Target (`Standard_SoT`)      | 2%     |
| Total Shots (`Standard_Sh`)           | 2%     |
| Shots per 90 (`Standard_Sh/90`)       | 1%     |
| Shots on Target per 90 (`Standard_SoT/90`) | 1%   |
| Penalty Goals (`Standard_PK`)         | 1%     |
| Penalty Attempts (`Standard_PKatt`)   | 1%     |

### 🔹 Chance Creation (Total: 70%)
| Metric                                            | Weight |
|---------------------------------------------------|--------|
| Expected Goals Assisted (`expected_goals_team`)   | 25%    |
| Big Chances Created (`big_chance_team`)           | 10%    |
| Dangerous Shots on Target (`ontarget_scoring_att_team`) | 10% |
| Touches in Opponent’s Box (`touches_in_opp_box_team`) | 10% |
| Possession Won in Final Third (`poss_won_att_3rd_team`) | 4%  |
| Penalties Won (`penalty_won_team`)                | 3%     |
| Big Chances Missed (`big_chance_missed_team`)     | 3%     |

---

## ✅ Conclusion

This analysis shows that offensive teams not only generate more attacking play but also achieve **better results in terms of points and goals**, with no clear evidence of being significantly more vulnerable defensively. This suggests that adopting an offensive style may be a **profitable strategy** in Argentina’s top division.

---
