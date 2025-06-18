# Visualizing Data
---

## Why Visualize Data?

Data scientists visualize data to better understand patterns, trends, and anomalies. While it's possible to scan raw data or calculate summary statistics like means or medians, **graphs allow us to detect patterns at a glance** — especially in large or complex datasets.

---

## Representing Data Visually

Graphing gives us a **quick, qualitative view** of our data. It helps with:

- Detecting **outlier values**
- Examining **distributions**
- Spotting **relationships** between variables

Sometimes we know what type of graph to use in advance. Other times, we explore different visualizations to see what patterns emerge.

---

## Example: Self-Driving Car Coordinates

Imagine you have data showing the position `(x, y)` of a self-driving car over time. In raw form, this data might look random:

- **Mean location**: around (0.2, 0.3)
- **Range**: from about -2 to 2 on each axis

But if you plot the points, you'll likely see a **clear path or movement pattern**, revealing far more than summary statistics alone.

---

## Introduction to Matplotlib

[Matplotlib](https://matplotlib.org/) is Python’s most widely used data visualization library. It lets you create charts like line plots, histograms, bar graphs, and scatter plots — with a lot of control over formatting.

### 🔹 Why Use Matplotlib?
- Easy to integrate with NumPy and pandas
- Flexible for customizing plots
- Widely supported and beginner-friendly

### 🔹 Common Plot Types
| Plot Type      | Function            | Use Case                        |
|----------------|---------------------|----------------------------------|
| Line Plot      | `plt.plot()`        | Trends over time or index       |
| Histogram      | `plt.hist()`        | Distributions                   |
| Scatter Plot   | `plt.scatter()`     | Relationship between variables  |
| Bar Chart      | `plt.bar()`         | Categorical comparisons         |

---

## Quick Demo in Python

```python
import matplotlib.pyplot as plt

# Example data: replace with your dataset
x = [0.1, 0.5, 1.0, 1.5, 2.0]
y = [0.3, 0.6, 1.1, 1.4, 2.1]

plt.figure(figsize=(6, 4))
plt.scatter(x, y, color='blue', marker='o')
plt.title('Self-Driving Car Path')
plt.xlabel('X Position')
plt.ylabel('Y Position')
plt.grid(True)
plt.show()

```
---
## 📂 Open the Code Notebook

Click below to open this week’s code notebook and follow along with examples and exercises:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1iv0y0Tjz_JegwkqnMoM4uji2_b5uKMZP)
