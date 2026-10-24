### We fit a ridge regression model to the California housing data and use it as a testbed for six optimizers: gradient descent, Newton, BFGS, L-BFGS, SGD and Adam.

The problem is a convex quadratic, so the "right" answer is known in closed form. That lets us measure every method against the exact minimizer and see where the theory from the lectures (linear rate for GD that depends on the condition number, quadratic for Newton, superlinear for quasi-Newton) holds up on real data.

```python
python3 -m venv .venv

source .venv/bin/activate

pip install -r requirements.txt

jupyter notebook ridge_housing.ipynb
```
