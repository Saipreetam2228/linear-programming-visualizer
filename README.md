# 📊 Linear Programming Visualizer

## 🚀 Overview

This project implements and visualizes a **Linear Programming (LP)** problem using Python. It solves the optimization problem using `scipy.optimize.linprog` and also includes a **fallback vertex enumeration method** to ensure the solution works even when SciPy is unavailable.

In addition to solving the LP problem, the project generates a graphical representation of:

* Feasible region
* Constraint boundaries
* Objective function contours
* Optimal solution point

---

## 🧮 Problem Statement

Maximize:

[
z = 3x_1 + 4x_2
]

Subject to:

[
x_1 + 2x_2 \leq 4
]
[
2x_1 + x_2 \leq 4
]
[
x_1 \geq 0,\quad x_2 \geq 0
]

---

## ⚙️ Features

* ✅ Solves Linear Programming problems using **SciPy (`linprog`)**
* ✅ Includes **manual vertex enumeration** as a fallback method
* ✅ Automatically detects optimal solution
* ✅ Visualizes:

  * Feasible region (shaded area)
  * Constraint lines
  * Objective function contour lines
  * Optimal solution point
* ✅ Works even without external optimization libraries

---

## 🛠️ Tech Stack

* **Python**
* **NumPy**
* **Matplotlib**
* **SciPy**

---

## 📂 Project Structure

```
linear-programming-visualizer/
│
├── lp_visualizer.ipynb     # Google Colab / Jupyter Notebook
├── lp_visualizer.py        # Python script version
├── requirements.txt        # Dependencies
├── output/                 # Saved plots (optional)
└── README.md               # Project documentation
```

---

## ▶️ How to Run

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/linear-programming-visualizer.git
cd linear-programming-visualizer
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Program

```bash
python lp_visualizer.py
```

---

## 📊 Output

The script generates a visualization that includes:

* ✔ Feasible region (highlighted area)
* ✔ Constraint boundary lines
* ✔ Objective function contours
* ✔ Optimal solution (marked point)

You can also modify the code to save the output:

```python
plt.savefig("output/sample_plot.png", dpi=300)
```

---

## 🧠 Concepts Covered

* Linear Programming (LP)
* Convex Feasible Regions
* Optimization Techniques
* Graphical Solution Method
* Numerical Optimization using SciPy

---

## 🔄 Fallback Mechanism

If SciPy is not available, the project:

* Computes intersection points of constraints
* Filters feasible vertices
* Evaluates objective function manually
* Selects the optimal vertex

---

## 🔮 Future Improvements

* 🔹 User input for custom LP problems
* 🔹 Interactive visualization (Streamlit / Web app)
* 🔹 Support for 3D LP problems
* 🔹 Step-by-step solution explanation

---

## 📌 Author

Developed as part of practical learning in **Optimization and Mathematical Modeling using Python**.

---

## ⭐ If you found this useful

Give this repo a ⭐ and consider contributing!
