Linear Regression From Scratch

A univariate linear regression model implemented using Python and NumPy, built entirely from scratch without Scikit-learn or pre-built machine learning functions.

Overview

Implemented gradient descent and manual partial differentiation to reduce the Mean Squared Error (MSE) from 1225 to approximately 38, approaching the theoretical minimum of 36.

Mathematics

Model:
y_pred = wx + b

Partial derivatives:

dw = (2/m) * Σ((y_pred - y) * x)

db = (2/m) * Σ(y_pred - y)

Parameter updates:

w = w - α * dw

b = b - α * db

Loss Visualization

Includes a Loss vs. Epochs graph using a logarithmic Y-axis with base 1.001 (plt.yscale('log', base=1.001)) to better visualize loss convergence.

Training Results

Parameter	Value
Learning Rate	0.0006
Initial Loss	1225
Final Loss	~38
Theoretical Minimum Loss	36
Optimization	Gradient Descent
Libraries	NumPy, Matplotlib

The learning rate was selected through experimentation to achieve stable convergence.