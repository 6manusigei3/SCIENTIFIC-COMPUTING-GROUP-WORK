# BIT 2118 – Scientific Computing Group Work

A collection of Python-based coursework tasks for **BIT 2118: Scientific Computing**. This repository brings together practical exercises covering scientific programming, numerical computation, linear algebra, numerical methods, differential equations, optimisation and simulation.

The work is organised into three sections covering Tasks 1–8, Tasks 9–12 and Tasks 13–20. Each section contains its own task files and supporting explanations or results.

## Course and Project Overview

- **Course:** BIT 2118 – Scientific Computing
- **Project:** Scientific Computing Group Work
- **Programming language:** Python 3
- **Main libraries:** NumPy, SciPy and Matplotlib
- **Coverage:** Tasks 1–20

## Repository Contents

| Section | Tasks | Focus |
|---|---:|---|
| [TASK 1-8](./TASK%201-8/) | 1–8 | Python and data science foundations, arrays, vectorization, numerical errors, matrix algebra, linear systems and iterative methods |
| [Numerical Methods – Tasks 9-12](./numerical-methods-task-9-12/) | 9–12 | Eigenvalues and eigenvectors, root-finding, nonlinear equations and numerical analysis |
| [TASK 13-20](./TASK%2013-20/) | 13–20 | Interpolation, curve fitting, differentiation, integration, differential equations, optimisation and Monte Carlo simulation |

## Task Guide

### Tasks 1–8: Scientific Computing Foundations

The first section introduces the Python and numerical-computing concepts used throughout the coursework.

| Task | Topic | Description |
|---|---|---|
| 1 | Data Science Essentials with Python | Foundational Python and data-science knowledge used in later exercises. |
| 2 | NumPy Arrays and Numerical Computation | Creates numerical arrays and calculates descriptive statistics and unit conversions. |
| 3 | Mathematical Functions and Vectorization | Compares loop-based calculations with NumPy vectorized operations. |
| 4 | Floating-Point Arithmetic and Numerical Errors | Explores floating-point precision, approximation errors and numerical stability. |
| 5 | Matrix Algebra and Matrix Operations | Applies matrix transformations, including rotation and scaling. |
| 6 | Systems of Linear Equations | Solves simultaneous linear equations and checks the residual. |
| 7 | Gaussian Elimination and LU Decomposition | Uses LU factorization to solve linear systems, including systems with different right-hand sides. |
| 8 | Iterative Methods for Linear Systems | Implements and compares the Jacobi and Gauss-Seidel methods. |

See the [Tasks 1–8 folder](./TASK%201-8/) for the task files and detailed explanations in its README.

### Tasks 9–12: Numerical Methods

This section applies numerical techniques to practical, illustrative problems.

| Task | Topic | Application |
|---|---|---|
| 9 | Eigenvalues and Eigenvectors | Analysing the relative importance of locations in a campus network. |
| 10 | Bisection and Fixed-Point Iteration | Estimating greenhouse temperature equilibrium and comparing convergence. |
| 11 | Newton-Raphson and Secant Methods | Estimating the internal rate of return for a solar-powered water-pumping investment scenario. |
| 12 | Nonlinear Equation Solving | Finding intersections in a reservoir and embankment design model. |

The implementation is in [numerical-methods-task-9-12/tasks](./numerical-methods-task-9-12/tasks/). Supporting plots and execution notes are in [outputs](./numerical-methods-task-9-12/outputs/), and the section-specific guide is in [its README](./numerical-methods-task-9-12/README.md).

### Tasks 13–20: Further Numerical Techniques

The final section explores additional numerical methods and their applications.

| Task | Topic |
|---|---|
| 13 | Interpolation |
| 14 | Curve Fitting |
| 15 | Numerical Differentiation |
| 16 | Numerical Integration |
| 17 | Euler's Method for Ordinary Differential Equations |
| 18 | Solving Ordinary Differential Equations with SciPy `solve_ivp()` |
| 19 | Numerical Optimisation using SciPy `minimize()` |
| 20 | Monte Carlo Simulation |

The Python implementations and task explanations are available in [TASK 13-20](./TASK%2013-20/).

## Technologies and Libraries

- **Python 3** – implementation of the numerical methods and computational exercises.
- **NumPy** – arrays, mathematical operations, matrix calculations and numerical data processing.
- **SciPy** – scientific algorithms, including linear algebra, root-finding, integration, differential-equation solving and optimisation.
- **Matplotlib** – plotting numerical results, functions, convergence and other visual outputs.
- **Pytest** – automated testing for the Tasks 9–12 section.

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/6manusigei3/SCIENTIFIC-COMPUTING-GROUP-WORK.git
cd SCIENTIFIC-COMPUTING-GROUP-WORK
```

### 2. Create and activate a virtual environment (recommended)

**Linux / macOS**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

**Windows PowerShell**

```powershell
py -m venv .venv
.venv\Scripts\Activate.ps1
```

### 3. Install the dependencies

For the Tasks 9–12 section, install its listed requirements:

```bash
python -m pip install -r numerical-methods-task-9-12/requirements.txt
```

For the other task scripts, make sure NumPy, SciPy and Matplotlib are available:

```bash
python -m pip install numpy scipy matplotlib
```

To run the automated tests for Tasks 9–12:

```bash
python -m pip install pytest
```

## Running the Programs

Run a Python file from its relevant folder. For example, the Tasks 9–12 modules can be run from the repository root with:

```bash
python -m tasks.task_09_eigenvalues
python -m tasks.task_10_bisection_fixed_point
python -m tasks.task_11_newton_secant
python -m tasks.task_12_nonlinear_equations
```

For scripts in the other sections, open the relevant task folder and run the required `.py` file using Python:

```bash
python path/to/task_file.py
```

Some programs display results in the terminal, while others also generate graphs or other visual outputs. Refer to the README inside each section for task-specific instructions.

## Testing

The Tasks 9–12 section includes automated tests. From the `numerical-methods-task-9-12` directory, run:

```bash
pytest -q
```

## Learning Outcomes

Through these exercises, the group practises how to:

- Represent and process numerical data using Python.
- Apply vectorized operations to improve computational efficiency.
- Recognise floating-point limitations and assess numerical accuracy.
- Use matrices and solve systems of linear equations.
- Apply direct and iterative numerical methods.
- Approximate roots, derivatives, integrals and solutions to differential equations.
- Fit mathematical models to observed data.
- Apply optimisation and simulation techniques to practical problems.
- Interpret numerical output and visualise computational results.

## Repository Structure

```text
SCIENTIFIC-COMPUTING-GROUP-WORK/
│
├── TASK 1-8/
│   ├── Task 2
│   ├── Task 3
│   ├── Task 4
│   ├── Task 5
│   ├── Task 6
│   ├── Task 7
│   ├── Task 8
│   └── readme.md
│
├── numerical-methods-task-9-12/
│   ├── tasks/
│   │   ├── task_09_eigenvalues.py
│   │   ├── task_10_bisection_fixed_point.py
│   │   ├── task_11_newton_secant.py
│   │   └── task_12_nonlinear_equations.py
│   ├── outputs/
│   ├── tests/
│   ├── requirements.txt
│   └── README.md
│
└── TASK 13-20/
    ├── task 13 Interpolation.py
    ├── TASK14 Curve_fitting.py
    ├── Task-15-Numerical-Differentiation.py
    ├── Task-16-Numerical-Integration.py
    ├── task 17 Euler's Method.py
    ├── task 18 solve_ivp().py
    ├── task 19 minimize().py
    ├── TASK -20 -monte_carlo.py
    └── readme.md
```

## References

- [Python Documentation](https://docs.python.org/3/)
- [NumPy Documentation](https://numpy.org/doc/)
- [SciPy Documentation](https://docs.scipy.org/doc/scipy/)
- [Matplotlib Documentation](https://matplotlib.org/stable/)
- [Pytest Documentation](https://docs.pytest.org/)

---

**BIT 2118 – Scientific Computing | Group Work**
