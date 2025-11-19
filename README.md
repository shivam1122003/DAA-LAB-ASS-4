# DAA-LAB-ASS-4
# Airline Crew Scheduling – Backtracking & Profiling

## 📌 Overview
This project implements a **Backtracking-based Airline Crew Scheduling System**.  
The goal is to assign flights to crew members while satisfying:

- ❌ No overlapping flights  
- 💤 Minimum required rest time  
- 💼 (Optional) Cost or fairness optimization  

The project includes full profiling (time + memory), visualizations, and a final analysis of feasibility.

---

## 🎯 Problem Definition
Given:
- A list of flights (ID, start time, end time)
- A set of crew members

Find a valid assignment such that:
- No crew member is assigned overlapping flights
- Rest time ≥ 1 hour between consecutive flights

This is a **Constraint Satisfaction Problem (CSP)**.

---

## 🔍 Algorithm: Backtracking
A recursive DFS search:
1. Pick the next flight  
2. Try assigning it to each crew member  
3. Check constraints  
4. Backtrack if invalid  

While backtracking is simple and exact, it is **exponential** in complexity:

**Time Complexity**  
- *n* = flights  
- *k* = crew members  

---

## 🧪 Profiling & Visualization
The notebook includes:
- ⏱ `time` profiling  
- 🧠 `memory_profiler` integration  
- 🔁 Recursive call counter  
- 📈 Execution time vs number of flights  
- 📉 Memory usage vs number of flights  
- 📊 Growth of backtracking search tree  

---

## 🔬 Key Insights
### Strengths
- Exact correctness  
- Intuitive recursive approach  
- Easy to extend with extra constraints  

### Limitations
- **Infeasible for real airline datasets**  
- Time and memory explode exponentially  
- Cannot handle multi-day duty periods or cost optimization at scale  

### Practical Relevance
The project illustrates why large airlines use:
- Mixed Integer Programming (MILP)
- Constraint Programming (CP-SAT)
- Metaheuristics (GA, Tabu search)
- Column generation methods  

---

## 🗂 Repository Structure

---

## ⚙️ Setup Instructions
### Install Dependencies

### Run Notebook
Open in Google Colab or Jupyter:

---

## 📚 Citations
- *Airline Crew Scheduling Literature*
  - Gopalakrishnan & Johnson (2005). “Airline Crew Scheduling: Models and Algorithms.”
  - Barnhart et al. (2003). “Column Generation Approaches for Crew Pairing.”
- Google OR-Tools CP-SAT Solver Documentation  
- ICAO Crew Rest and Duty Regulations

---

## 👤 Author
Your Name  
Course / Assignment  
