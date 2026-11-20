# Cooling of a Square Plate — The Heat Equation

Companion notebook to our report *Cooling of a Square Plate: The Heat Equation*
for **Numerical Linear Algebra & Partial Differential Equations**
(Bachelor in Applied Mathematics, IE University).

We solve the 2D heat equation on the unit square,

    u_t = κ (u_xx + u_yy),   u = 0 on the boundary,   u(x,y,0) = 16x(1−x)y(1−y),

with κ = 0.1 up to T = 1. The notebook compares an analytical Fourier-series
solution against implicit time stepping with four linear solvers:
Conjugate Gradient (with and without IC(0) preconditioning),
red–black Gauss–Seidel, and sparse LU. It reports accuracy, run time,
and memory use on grids from 10×10 up to 100×100.

## Contents
- `cooling_square_plate_lean.ipynb` – full code, figures and tables
  (outputs are saved, so it can be read directly on GitHub)

## How to run
Requires Python 3.10+ with NumPy, SciPy ≥ 1.12, Matplotlib, pandas, psutil and Jupyter.

    pip install numpy scipy matplotlib pandas psutil jupyter
    jupyter notebook cooling_square_plate_lean.ipynb

Then choose **Kernel → Restart & Run All**. No input files are needed.

## Authors
- Katrín Lilja Árnadóttir
- Filip Dimitrijević
- Lisa Sophie Mostowoj
- Patricia-Magdalena Nistor
- David Vodonenko

Instructors: Ignacio Zubizarreta, Laura Álvaro Gómez
IE University, November 2026
