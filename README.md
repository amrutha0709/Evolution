
---

## 🚀 Features
- **Genetic Algorithm**:
  - One-point crossover.
  - Rank-based selection.
  - Replacement based on fitness.
- **Hill Climber**:
  - Random mutation applied to evolve genotypes.
  - Replacement of less fit individuals.

---

## 🔧 Parameters
- **Genetic Algorithm**:
  - Population size: 100 demes, 10 genotypes each.
  - Bit length per genotype: 400.
  - Mutation rate: \( \frac{1}{\sqrt{N}} \).
  - Crossover rate: Decreases dynamically as generations progress.
  - Migration rate: 0.0004.

- **Hill Climber**:
  - Random mutations applied at per-bit mutation rate.
  - Adaptive replacement based on fitness.

---

## 📜 Fitness Function
Fitness is calculated based on **Hamming Distance** between genotype blocks and target strings:
- **Target Strings**:
  - \( t_1 = [1010...10] \) (alternating bits).
  - \( t_2 = [1111...11] \) (all ones).
- **Weights**: Block fitness is weighted differently for each target string.

---

## 🖥️ Execution
1. **Genetic Algorithm**:
   - Run the script `ga_crossover.py`.
   - Tracks average fitness per generation.
   - Generates plots for fitness progression.

2. **Hill Climber**:
   - Run the script `hill_climber.py`.
   - Logs average fitness at regular intervals.

---

## 📈 Output
- Plots showing average fitness per generation.
- Logs of fitness progress for hill climber and GA.

---

## 🧑‍💻 Author
[Your Name]
