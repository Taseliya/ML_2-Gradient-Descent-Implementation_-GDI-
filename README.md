 Gradient Descent Implementation

This is how gradient descent actually works, using linear regression on some noisy, made-up data. The whole point? To tweak the model’s parameters bit by bit until it nails the lowest possible Mean Squared Error (MSE).

Project Overview
-What’s the goal? Build gradient descent from scratch with NumPy to uncover the pattern behind y = 3x + 2 (plus some random noise).
- What did I do?
  - Cooked up some random-but-patterned data.
  - Wrote out the Mean Squared Error cost function.
  - Set up a loop that keeps adjusting the weights (w) and bias (b) using gradients.
  - Watched how the cost dropped each time around the training loop (100 times total).

 Key Results
- Learned Parameters: The model zeroed in on w ≈ 2.98 and b ≈ 1.69—pretty close to the ground truth, even with the noise tossed in.
- Performance: The final MSE hit 0.65, so the model did a solid job finding the original line through the scattered points.

 How it Works
It starts simple, with w=0 and b=0. On every loop through the data, it figures out which way to move by calculating the gradients (dw, db). Then it shuffles the parameters a little (step size is 0.01), always marching toward a lower error.

 Technologies Used
- Language: Python
- Libraries: Just NumPy for the math and Matplotlib for the graphs.

 Visualizations
That “Cost vs. Iterations” plot says it all: at first, the MSE drops fast, but after a while, it cools off and flattens out as the model homes in on the best possible values.
