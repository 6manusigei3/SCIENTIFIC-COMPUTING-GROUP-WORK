# BIT 2118 — Scientific Computing Group Work

**REG NO: BSCCS/2025/40046**

> **Scientific programming, numerical analysis and computational problem-solving with Python.**

This repository presents the group's coursework for **BIT 2118: Scientific Computing**. It brings together Python implementations, mathematical explanations and illustrative applications of computational methods. The work progresses from numerical data handling and linear algebra to root-finding, differential equations, optimisation and simulation.

## Project at a glance

| Item | Details |
|---|---|
| Course | BIT 2118 — Scientific Computing |
| Coursework | Group Work, Tasks 1–20 |
| Language | Python 3 |
| Numerical computing | NumPy |
| Scientific algorithms | SciPy |
| Visualisation | Matplotlib |
| Automated testing | Pytest (Tasks 9–12 section) |

## Contents

- [Project scope](#project-scope)
- [Task index](#task-index)
- [Methods and concepts](#methods-and-concepts)
- [Repository structure](#repository-structure)
- [Requirements and setup](#requirements-and-setup)
- [Running the programs](#running-the-programs)
- [Testing and numerical verification](#testing-and-numerical-verification)
- [Interpreting results](#interpreting-results)
- [Assumptions and limitations](#assumptions-and-limitations)
- [Learning outcomes](#learning-outcomes)
- [References](#references)

---

## Project scope

The coursework is organised into three sections to make the progression of concepts clear.

| Section | Tasks | Main emphasis |
|---|---:|---|
| [Scientific computing foundations](./TASK%201-8/) | 1–8 | Python, arrays, vectorisation, numerical error, matrices and linear systems |
| [Numerical methods](./numerical-methods-task-9-12/) | 9–12 | Eigenvalue analysis, root-finding and nonlinear equations |
| [Further numerical techniques](./TASK%2013-20/) | 13–20 | Interpolation, curve fitting, calculus, differential equations, optimisation and simulation |

## Task index

### Tasks 1–8 — Scientific computing foundations

| Task | Topic | Main concept |
|---:|---|---|
| 1 | Data Science Essentials with Python | Foundational Python and data-science knowledge. |
| 2 | NumPy Arrays and Numerical Computation | Array creation, descriptive statistics and unit conversion. |
| 3 | Mathematical Functions and Vectorisation | Loop-based versus vectorised computation. |
| 4 | Floating-Point Arithmetic and Numerical Errors | Precision, approximation error and numerical stability. |
| 5 | Matrix Algebra and Matrix Operations | Matrix operations and coordinate transformations. |
| 6 | Systems of Linear Equations | Solving simultaneous equations and checking residuals. |
| 7 | Gaussian Elimination and LU Decomposition | Matrix factorisation for solving linear systems. |
| 8 | Iterative Methods for Linear Systems | Jacobi and Gauss–Seidel iteration. |

**Detailed guide:** [TASK 1-8/readme.md](./TASK%201-8/readme.md)

### Tasks 9–12 — Numerical methods

| Task | Topic | Illustrative application |
|---:|---|---|
| 9 | Eigenvalues and Eigenvectors | Campus network analysis and relative node importance. |
| 10 | Bisection and Fixed-Point Iteration | Greenhouse temperature equilibrium and convergence comparison. |
| 11 | Newton–Raphson and Secant Methods | Internal rate of return for a solar-powered water-pumping scenario. |
| 12 | Nonlinear Equation Solving | Intersections in a reservoir and embankment model. |

**Detailed guide:** [numerical-methods-task-9-12/README.md](./numerical-methods-task-9-12/README.md)

This section contains the task implementations, supporting outputs and an automated test suite.

### Tasks 13–20 — Further numerical techniques

| Task | Topic | Main concept |
|---:|---|---|
| 13 | Interpolation | Estimating values between known data points. |
| 14 | Curve Fitting | Fitting a mathematical model to observations. |
| 15 | Numerical Differentiation | Finite-difference approximations of derivatives. |
| 16 | Numerical Integration | Approximation of definite integrals and accumulated quantities. |
| 17 | Euler's Method | Numerical approximation of ordinary differential equations. |
| 18 | SciPy `solve_ivp()` | Numerical solution of initial-value problems. |
| 19 | SciPy `minimize()` | Numerical optimisation. |
| 20 | Monte Carlo Simulation | Estimation using random sampling. |

**Detailed guide:** [TASK 13-20/readme.md](./TASK%2013-20/readme.md)

---

## Methods and concepts

The exercises demonstrate core scientific-computing practices:

- **Array-based computation:** representing datasets and applying operations efficiently.
- **Vectorisation:** reducing explicit Python loops for numerical operations.
- **Numerical accuracy:** understanding floating-point representation, error, tolerance and stability.
- **Linear algebra:** applying matrix operations, factorisation and linear-system solvers.
- **Iterative methods:** using stopping criteria and comparing convergence.
- **Numerical approximation:** estimating roots, interpolated values, derivatives and integrals.
- **Modelling and simulation:** translating a mathematical problem into a computational procedure and interpreting the result.

## Repository structure

```text
SCIENTIFIC-COMPUTING-GROUP-WORK/
├── README.md
├── TASK 1-8/
│   ├── task folders and Python implementations
│   └── readme.md
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

The tree highlights the main organisation; each section directory contains its own task materials.

## Requirements and setup

### Requirements

- Python 3
- NumPy
- SciPy
- Matplotlib
- Pytest (for Tasks 9–12 tests)

### 1. Clone the repository

```bash
git clone https://github.com/6manusigei3/SCIENTIFIC-COMPUTING-GROUP-WORK.git
cd SCIENTIFIC-COMPUTING-GROUP-WORK
```

### 2. Create a virtual environment

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

### 3. Install dependencies

Install the dependencies specified for Tasks 9–12:

```bash
python -m pip install -r numerical-methods-task-9-12/requirements.txt
```

For scripts in the other sections, ensure the scientific Python libraries are installed:

```bash
python -m pip install numpy scipy matplotlib
python -m pip install pytest
```

## Running the programs

### Tasks 9–12

Run these commands from the repository root. The subshell change ensures Python can locate the section's `tasks` package:

```bash
cd numerical-methods-task-9-12
python -m tasks.task_09_eigenvalues
python -m tasks.task_10_bisection_fixed_point
python -m tasks.task_11_newton_secant
python -m tasks.task_12_nonlinear_equations
```

### Tasks 1–8 and 13–20

Open the relevant section and run the required Python script using its actual filename. General pattern:

```bash
python "path/to/the/task_script.py"
```

Some programs display results in the terminal; others may also display or save plots. Consult the relevant section README for task-specific instructions.

## Testing and numerical verification

The Tasks 9–12 section includes automated tests. From inside `numerical-methods-task-9-12`, run:

```bash
pytest -q
```

Numerical output should also be checked against the mathematical problem. Depending on the task, verification may include:

- Substituting a computed solution into the original equations.
- Examining the residual of a linear system.
- Comparing an approximation with an exact value when one is available.
- Checking convergence against the method's tolerance and stopping condition.
- Comparing numerical methods using the same inputs.

A program running without errors does not, by itself, establish that its numerical result is accurate. Mathematical verification and interpretation remain important.

## Interpreting results

For each exercise, consider the following questions:

1. **Input:** Which data, parameters or initial values are supplied?
2. **Method:** Which numerical technique is used, and why is it appropriate?
3. **Output:** What solution, estimate or visual result is produced?
4. **Verification:** How can the result be checked?
5. **Interpretation:** What does the result mean in the problem's context?
6. **Sensitivity:** How does changing an input, step size, tolerance or iteration limit affect the result?

## Assumptions and limitations

The practical scenarios are mathematical examples used to demonstrate computational methods. Unless a task explicitly identifies measured data, its input values should be understood as illustrative rather than verified field measurements or professional forecasts.

Numerical results can be affected by rounding, floating-point precision, initial guesses, step sizes, convergence tolerances and model assumptions. A method suitable for one set of inputs may not converge or may be unsuitable for another. These factors should be considered when interpreting each result.

## Learning outcomes

Through the coursework, the group gains practical experience in:

- Using Python to represent and process scientific data.
- Applying NumPy and SciPy to numerical problems.
- Comparing computational approaches by efficiency, accuracy and convergence.
- Solving linear and nonlinear equations.
- Understanding numerical error and finite-precision arithmetic.
- Approximating derivatives, integrals and differential-equation solutions.
- Applying interpolation, curve fitting, optimisation and simulation.
- Presenting and interpreting computational results.

## References

The following official documentation supports the tools and libraries used:

- [Python Documentation](https://docs.python.org/3/)
- [NumPy Documentation](https://numpy.org/doc/)
- [SciPy Documentation](https://docs.scipy.org/doc/scipy/)
- [Matplotlib Documentation](https://matplotlib.org/stable/)
- [Pytest Documentation](https://docs.pytest.org/)

---

**BIT 2118 — Scientific Computing | Group Work**
