# Sea Level Predictor 🌊

This project analyzes historical sea level data from **1880 to recent years** and predicts future sea level rise using linear regression. Visualizations compare long-term trends with more recent data to project how rising sea levels might continue through **2050**.

---

## 📂 Dataset

The dataset comes from the EPA and contains:
- `Year`: Observation year (from 1880 onward)
- `CSIRO Adjusted Sea Level`: Adjusted global sea level in inches

File: `epa-sea-level.csv`

---

## 🔍 Objectives

### ✅ Scatter Plot with Regression Lines
- Plot raw sea level data from 1880 to present.
- Fit a **linear regression line** over:
  - All data (1880–latest)
  - Recent data (2000–latest)

### 🧮 Linear Regression
Using `scipy.stats.linregress`:
- Compute the **slope and intercept** of each regression line.
- Project both lines through **year 2050** to estimate future sea levels.

---

## 📈 Output Visualization

- **Red line**: Best fit line using all data from 1880–2050
- **Green line**: Best fit line from 2000–2050
- **Title**: Rise in Sea Level
- **X-axis**: Year
- **Y-axis**: Sea Level (inches)

Output saved as:
sea_level_plot.png

yaml
Copy
Edit

---

## 🧪 Sample Usage

```python
from sea_level_predictor import draw_plot

draw_plot()
🛠️ Requirements
Python 3

pandas

matplotlib

scipy

Install dependencies:

bash
Copy
Edit
pip install pandas matplotlib scipy
🧠 Insights
How much has the sea level risen since 1880?

Is the rate of rise increasing in recent decades?

What might sea levels look like in 2050?

This project builds foundational skills in:

Data cleaning

Regression modeling

Predictive visualization
