# Linear Regression from Scratch (Visualization with Tricks)

This project demonstrates a basic implementation of **linear regression** using Python, `numpy`, and `matplotlib`.  
It visualizes how different update rules ("tricks") adjust the parameters of a regression line to fit a dataset.

---

## 📊 Dataset
We use a small dataset of housing prices based on the number of rooms:

- **Features (X):** `[1, 2, 3, 5, 6, 7]`  
- **Labels (y):** `[155, 197, 244, 356, 407, 448]`

---

## ⚙️ Functions

### Plotting
- `draw_line(slope, y_intercept, ...)` → Draws a line with given slope and intercept.  
- `plot_points(features, labels)` → Plots the dataset points.

### Tricks (Update Rules)
- **Simple Trick:** Small random adjustments based on prediction error.  
- **Absolute Trick:** Updates proportional to the sign of the error.  
- **Square Trick:** Gradient descent style update proportional to error magnitude.

### Linear Regression Loop
- Starts with random weights (`base_price`, `price_per_room`).  
- Iteratively applies one of the tricks to minimize error.  
- Plots the line evolution across epochs.

---

## ▶️ Running the Algorithm

```python
linear_regression(features, labels, learning_rate=0.01, epochs=1000)
