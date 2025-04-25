# Hydrostatic Thrust Bearing Optimisation

This project presents a Python-based optimisation framework for hydrostatic thrust bearing systems. By applying metaheuristic algorithms — **Random Search** and **Simulated Annealing** — the system successfully minimised **frictional power loss by 22%**, while ensuring the load-bearing performance remained within physical constraints.

---

## 📌 Project Details

- **Project Title**: Hydrostatic Thrust Bearing Optimisation  
- **Duration**: November 2023  
- **Role**: Sole Developer & Researcher  
- **Keywords**: Mechanical Optimisation, Metaheuristics, Simulated Annealing, Frictional Loss Reduction, Python, Engineering Algorithms

---

## 🎯 Objectives

- Develop a simulation model for hydrostatic thrust bearing behaviour.
- Define a multi-objective cost function incorporating **pressure** and **frictional energy loss**.
- Apply metaheuristic optimisation algorithms to **minimise power losses**.
- Validate results through **statistical testing** and convergence analysis.

---

## 🛠️ Tech Stack

- **Language**: Python  
- **Libraries**: NumPy, Matplotlib, Pandas, Seaborn  
- **Concepts**: Metaheuristic Optimisation, Penalty Functions, Engineering Simulation, Statistical Analysis

---

## 🧠 Technical Details

### ⚙️ Objective Function & Physical Constraints

- Designed a **multi-objective cost function**:
  - Minimise **frictional energy loss (Ef)**
  - Maximise or maintain required **pressure/load capacity**
- Implemented **7 physical constraints**:
  - Load capacity threshold
  - Pressure limits
  - Thermal bounds (temperature increase)
  - Geometric constraints (inner/outer radius, area, thickness)
- Used **penalty-based constraint handling** to discourage invalid designs

### 🔄 Optimisation Algorithms

- **Random Search**:
  - Simple stochastic algorithm
  - Used as a performance baseline
- **Simulated Annealing**:
  - Temperature-based probabilistic algorithm
  - Custom cooling schedule and neighbourhood control
  - Accepted suboptimal moves early on to escape local minima

### 📊 Robustness Testing & Validation

- Performed **21 independent runs** per algorithm 
- Applied **paired t-tests** to assess statistical significance of results
- Generated **visualisations** (convergence plots, scatter plots) to compare performance

---

## 📈 Results

### 🔧 Sample Metric Comparison

| Metric                      | Initial Design | Optimised Design |
|----------------------------|----------------|------------------|
| Frictional Energy Loss (Ef) | 3200 J         | 2504.77 J        |
| Power Loss Reduction        | –              | **22%**          |

### 🧠 Observations

- Simulated Annealing consistently outperformed Random Search, delivering better solutions with lower objective values and more stable convergence.
- The project highlighted how metaheuristics can solve complex engineering problems where analytical solutions are infeasible.
- Built a strong foundation for applying similar optimisation strategies in broader mechanical or data science applications.




