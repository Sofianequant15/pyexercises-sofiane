# Survive the Quarter — Croissant Rocket

## Project overview

**Survive the Quarter** is my final Python project for SKEMA Business School.

The player manages the marketing decisions of **Croissant Rocket**, a fictional drone-delivery company. The objective is to survive **10 days** while protecting two key resources:

- **Budget**
- **Reputation**

Every day, the player receives a new situation and must choose between **A, B, or C**. Each decision changes the budget and reputation.

If the budget or reputation reaches **0 or below**, the player is fired.

---

## 🎮 Graphic version

A browser-based graphic version of the project is available here:

**https://sofianequant15.github.io/pyexercises-sofiane/**

This version runs directly in a web browser and does not require Python to be installed.

---

## 🐍 Python version

The main Python version of the project is:

`survive_the_quarter.py`

To run it from the terminal:

```bash
python3 survive_the_quarter.py
```

The player is asked to:

1. Enter a name.
2. Choose a difficulty.
3. Play through 10 randomly selected scenarios.
4. Choose A, B, or C for each situation.
5. Try to keep both budget and reputation above 0.

---

## Difficulty

The selected extra feature for the project is **Difficulty**.

- **Easy:** starting budget of **15,000 EUR**
- **Hard:** starting budget of **6,000 EUR**

Reputation starts at **50** and cannot go above **100**.

---

## Final score

If the player survives all 10 days, the final score is calculated with:

```text
score = reputation + budget // 200
```

The final title is then assigned according to the score:

- **Below 95:** Eternal Intern
- **95–119:** Growth Hacker
- **120–139:** CMO Material
- **140 or more:** Viral Legend

The game also identifies the player's **best** and **worst** decisions based on reputation change.

---

## Project files

- `survive_the_quarter.py` — main terminal game
- `survive_the_quarter_web.py` — Gradio graphic-interface version
- `scenarios_A.csv` — scenario database
- `results.csv` — saved game results
- `AI_log_Sofiane_DIDI.pdf` — AI assistance and development log
- `github_pages_game/` — static web version used for GitHub Pages

The scenario file contains the original scenarios plus my three additional scenarios (**31, 32, and 33**).

---

## Technical elements used

The Python project uses:

- `csv`
- `random`
- functions
- tuples
- lists
- dictionaries
- loops
- input validation
- file reading
- file writing
- game history tracking

The program is divided into several functions so that each part of the game has a clear responsibility.

---

## Game flow

```text
Start
  ↓
Enter player name
  ↓
Choose difficulty
  ↓
Load scenarios from CSV
  ↓
Shuffle scenarios
  ↓
Play 10 days
  ↓
Choose A / B / C
  ↓
Update budget and reputation
  ↓
Check if player is fired
  ↓
Calculate final score and title
  ↓
Display best and worst move
  ↓
Save result
```

---

## Graphic interface

The graphical version keeps the same main game concept but presents it with a visual interface including:

- budget gauge
- reputation gauge
- day counter
- scenario cards
- interactive A/B/C choices
- decision feedback
- final score and title
- best and worst move

The GitHub Pages version is a static browser adaptation of the game so it can be shared with the teacher using a permanent web link.

---

## Author

**Sofiane DIDI**  
SKEMA Business School
