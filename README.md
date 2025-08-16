# Syracuse Women’s Lacrosse Data Analysis

This project analyzes player statistics and game performance for the Syracuse University Women’s Lacrosse team across the **2024 and 2025 seasons**. It uses structured data to answer important questions about game results, player performance, and fan attendance.

---

## 📁 Datasets:

| Datasets            | Description                                     |
|---------------------|-------------------------------------------------|
| `2024_players.csv`  | Player statistics for the 2024 season           |
| `2025_players.csv`  | Player statistics for the 2025 season           |
| `2024_games.csv`    | Game data for the 2024 season                   |
| `2025_games.csv`    | Game data for the 2025 season                   |

(Not included but can be downloaded from the link: https://cuse.com/sports/2013/1/16/WLAX_0116134638)


## Project Files: 

1. README.md : Documentation and instructions for running the project


## Basic Questions Answered by LLM in Week 1:

1. **How many games did Syracuse Women’s Lacrosse play in 2024 and 2025?**
Answer: 2024: 22 games 2025: 19 games 

2. **Who scored the most goals in the 2024 season?**
Answer: Emma Tyrrell with 70 goals 

3. **Who had the most assists in the 2025 season?**
Answer: Emma Ward with 46 assists 

4. **What was Syracuse’s win-loss record in 2024?**
Answer: 15 wins, 7 losses 

5. **Which 2025 game had the highest attendance?**
Answer: Feb 25 vs #3 Northwestern, with 2,899 attendees 


## Advanced Questions Answered by LLM in Week 2:

1. **Who was the most improved returning player (2024 → 2025) by points per game (PPG = (G+A)/GP)?**
Answer: Olivia Adamson (+1.561 PPG; 2024: 3.773 → 2025: 5.333)

2. **Did SU improve more on offense or defense year-over-year?**
GF/G = goals for per game; GA/G = goals against per game.

2024: GF/G 14.50, GA/G 10.25, Win% 58.3%

2025: GF/G 13.20, GA/G 11.20, Win% 50.0%
Answer: Offense slipped (−1.30 GF/G) while defense allowed more (+0.95 GA/G). Net: both offense and defense regressed in the 2025 rows you provided.

3. **“Clutch” performance—how did SU do in close games (|goal diff| ≤ 2)?**

2024 close games: 0–2 (2 games)

2025 close games: 1–2 (3 games)
Answer: Slightly better clutch results in 2025 (1 win vs 0), but still under .500 in close ones.

4. **Who led 2025 in shooting efficiency (G/Sh), minimum 30 shots?**
Answer: Gracie Britton — 0.488 (41 shots, min threshold = 30).

5. **If the coach wants +2 more wins in 2025, should the focus be offense or defense?**
Simple simulation (apply evenly in every game):

Actual 2025 wins: 5

Add +1 goal to SU in every game: still 5 wins

Prevent 1 goal in every game: still 5 wins
Answer: With a uniform +1 GF or −1 GA, the 2025 outcomes don’t change on these rows; that suggests targeted improvement (specific matchups or close-loss situations) would matter more than a uniform tweak. A good next pass is a targeted swing (e.g., add +1 goal only in losses decided by 1–2) or opponent-specific adjustments.

---

## 🛠️ Dependencies

- Python 3.7+
- Required library: pandas