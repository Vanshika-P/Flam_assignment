# Flam_assignment
Flam Assignment (Vanshika Patil)
1) Objective: Estimate the unknown parameters θ, M, X in the given parametric curve equation using numerical optimization
2) Final estimated parameters: θ (radians) = 0.5163051223, θ (degrees) ≈ 29.582°, M = –0.05, X = 55.0134078
3) Final Parametric Equation:
   Desmos Format- (t*cos(0.5163051223) - exp(-0.05*abs(t))*sin(0.3*t)*sin(0.5163051223) + 55.0134078, 42 + t*sin(0.5163051223) + exp(-0.05*abs(t))*sin(0.3*t)*cos(0.5163051223))
   LaTeX_format- \left(t\cos(0.5163051222957233) - e^{-0.04999999999562039\left|t\right|}\cdot\sin(0.3t)\sin(0.5163051222957233) + 55.01340779732458,42 t\sin(0.5163051222957233) + e^{-0.04999999999562039\left|t\right|}\cdot\sin(0.3t)\cos(0.5163051222957233)\right)
4) Method:
   - Loaded x(t) and y(t) from given CSV file.
   - Defined the parametric model using the given mathematical formula.
   - Used Nonlinear Least Squares (scipy.optimize.least_squares) to minimize the residual error between observed and predicted curve points.
   - Applied the parameter bounds: 0° < θ < 50°, –0.05 < M < 0.05, 0 < X < 100
5) Final error: Total L1 Error- ~38102, Mean L1 Error per point- ~25.40

Desmos link: https://www.desmos.com/calculator/hgvd742qpn
Colab Notebook: https://github.com/Vanshika-P/Flam_assignment/blob/main/Assignment_Flam.ipynb
