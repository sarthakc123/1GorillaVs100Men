# 🦍 Gorilla vs 100 Men: A Monte Carlo Simulation

Can a single powerful gorilla defeat 100 men?  
This project models and simulates that scenario using Monte Carlo methods and visual analytics.

---

## 🧠 Concept

Inspired by internet debates, this simulation explores whether a high-speed, high-damage gorilla can outlast and defeat 100 men, each with randomized health, accuracy, and attack strength. The simulation is repeated thousands of times to estimate probable outcomes and draw insights.

---

## 🔬 Simulation Details

- **Environment**: Randomized grid (20x20 to 50x50)
- **Combatants**:
  - Gorilla:
    - HP: 400–600
    - Speed: 10
    - Accuracy: 90%
    - Damage per hit: 40
  - Men (100 total):
    - HP: 10–20
    - Speed: 1
    - Accuracy: 60%
    - Damage per hit: 5–10

- **Rules**:
  - Gorilla moves toward the nearest man or jumps if stuck.
  - Men move toward the gorilla.
  - Attacks occur if within 1-tile distance.
  - Timeout condition after 300 idle steps or max 5000 steps.

---

## 📊 Visualizations

- Outcome distribution (win rate)
- Number of steps to victory
- Grid size vs outcome
- Gorilla HP vs win probability
- Correlation heatmaps between input parameters and simulation result
- Animated battle sequences

![Outcome Sample](assets/outcome_bar_chart.png)
![Step Distribution](assets/step_distribution.png)
![Correlation](assets/correlation_heatmap.png)

---

## 📈 Statistical Convergence

We ran simulations with increasing iterations (1000 to 5000) and observed convergence in the win rates and step distributions, verifying the reliability of our Monte Carlo estimate.

---

## 📂 Files

- `gorilla_simulation.ipynb`: Main simulation and analysis
- `simulation_output.csv`: Logged results from 5000 simulations
- `assets/`: Contains output graphs and animations

---

## 🛠️ Technologies Used

- Python (NumPy, Pandas, Matplotlib, Seaborn)
- Jupyter Notebook
- Monte Carlo Simulation

---

## 📌 Future Ideas

- Add fatigue timers or dodge cooldowns
- Simulate with men in squads or weapons
- Multiplayer AI agents using reinforcement learning

---

## 🤖 Author

Sarthak Chandarana  
[LinkedIn](https://www.linkedin.com/in/sarthak-chandarana) | [GitHub](https://github.com/sarthakchandarana)
