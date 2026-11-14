<div align="center">

# 🦁 Confidence vs. Prediction Intervals — Regression Inference Masterclass
### **Lindenwood University — Interactive Data Science & Machine Learning Masterclass**

[![Live Interactive Lab](https://img.shields.io/badge/Launch_Interactive_Lab-Live_Demo-C5B358?style=for-the-badge&logo=googlechrome&logoColor=black)](https://sagarkalauni.github.io/confidence-and-prediction-interval/)
[![Course](https://img.shields.io/badge/Course-MTH_34500-000000?style=for-the-badge&logo=academia&logoColor=C5B358)](#)
[![Author](https://img.shields.io/badge/Faculty-Sagar_Kalauni,_M.S.-1E293B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SagarKalauni)

</div>

---

## 📖 Overview

An interactive statistical visualizer clarifying one of the most critical distinctions in regression analysis: **Confidence Intervals for the Mean Response $E[Y \mid X = x_0]$** versus **Prediction Intervals for a New Individual Observation $Y_0$ at $X = x_0$**.

> 🔗 **Launch the Live Interactive Application:** [**https://sagarkalauni.github.io/confidence-and-prediction-interval/**](https://sagarkalauni.github.io/confidence-and-prediction-interval/)

---

### 📐 Mathematical Formulation

At a target predictor value $x_0$, let $\hat{y}_0 = \hat{\beta}_0 + \hat{\beta}_1 x_0$ be the fitted point estimate and $\hat{\sigma} = \sqrt{MSE}$ be the residual standard error with $n - 2$ degrees of freedom:

1. **$(1 - \alpha)$ Confidence Interval for Mean Response $\mathbb{E}[Y \mid X = x_0]$:**
   $$\hat{y}_0 \pm t_{\alpha/2, \, n-2} \cdot \hat{\sigma} \sqrt{\frac{1}{n} + \frac{(x_0 - \bar{x})^2}{\sum_{i=1}^n (x_i - \bar{x})^2}}$$

2. **$(1 - \alpha)$ Prediction Interval for a Single New Observation $Y_0$:**
   $$\hat{y}_0 \pm t_{\alpha/2, \, n-2} \cdot \hat{\sigma} \sqrt{\mathbf{1} + \frac{1}{n} + \frac{(x_0 - \bar{x})^2}{\sum_{i=1}^n (x_i - \bar{x})^2}}$$

The extra **$1$** inside the radical accounts for the irreducible random error variance $\text{Var}(\varepsilon_0) = \sigma^2$ of an individual future observation.

---

## ✨ Key Interactive Features

- **Dual Band Overlay:** Simultaneously visualize the narrow hyperbolic Confidence Band ($CI$) and the wider Prediction Band ($PI$).
- **Sample Size ($n$) & Confidence Level ($1-\alpha$) Controls:** Observe how increasing $n$ collapses the Confidence Interval toward zero width while the Prediction Interval remains bounded below by $\pm t_{\alpha/2} \sigma$.
- **Extrapolation Penalty Visualization:** Watch the hyperbolic curvature flare outward as $x_0$ moves far away from the sample mean $\bar{x}$.

---

## 🎓 Pedagogical & Course Context

- **Institution:** Lindenwood University (*College of Science, Technology, and Health*)
- **Course Curriculum:** MTH 34500 — Regression Analysis
- **Instructor & Author:** **Sagar Kalauni, M.S.** (*Full-Time Faculty in Data Science*)
- **Tech Stack:** HTML5, Tailwind CSS, **D3.js** (Dynamic Data Visualization), **MathJax** (LaTeX Mathematical Rendering), Vanilla ES6+ JavaScript (Zero-Dependency Client-Side Execution).

---

## 🚀 Running Locally

Because this visualizer is engineered as a self-contained, zero-build client-side application, you can run it immediately in any modern browser:

```bash
# Clone the repository
git clone https://github.com/SagarKalauni/confidence-and-prediction-interval.git

# Navigate into the project directory
cd confidence-and-prediction-interval

# Open index.html directly in your browser or serve locally:
python -m http.server 8000
```

---

## 🔗 Explore the Complete Interactive Masterclass Suite

| Module | Topic | Live Link |
| :--- | :--- | :---: |
| **Linear Regression** | Ordinary Least Squares & Residual Minimization | [Launch](https://sagarkalauni.github.io/linear-regression/) |
| **Logistic Regression** | Sigmoid Probabilities & Binary Cross-Entropy | [Launch](https://sagarkalauni.github.io/logistic-regression/) |
| **Regularization ($L_1 / L_2$)** | Lasso vs. Ridge Constraint Geometry | [Launch](https://sagarkalauni.github.io/Regularization/) |
| **K-Nearest Neighbors** | Instance-Based Learning & Distance Metrics | [Launch](https://sagarkalauni.github.io/knn/) |
| **Support Vector Machine** | Maximum-Margin Hyperplanes & Soft Margin $C$ | [Launch](https://sagarkalauni.github.io/support-vector-machine/) |
| **RBF Kernel SVM** | Non-Linear Kernel Trick & $(\gamma, C)$ Tuning | [Launch](https://sagarkalauni.github.io/rbf-kernel-svm/) |
| **Decision Tree (CART)** | Recursive Splitting, Gini & Entropy | [Launch](https://sagarkalauni.github.io/decision-tree/) |
| **Random Forest** | Bagging & Ensemble Variance Reduction | [Launch](https://sagarkalauni.github.io/random-forest/) |
| **Voting Classifier** | Hard Majority vs. Soft Probability Voting | [Launch](https://sagarkalauni.github.io/voting-classifier/) |
| **K-Means Clustering** | Lloyd's Algorithm, Voronoi & Elbow WCSS | [Launch](https://sagarkalauni.github.io/k-mean-clustering/) |
| **Confusion Matrix** | Precision, Recall, Specificity & $F_1$-Score | [Launch](https://sagarkalauni.github.io/confusion-matrix/) |
| **Confidence vs. Prediction Intervals** | Mean Response vs. Individual Uncertainty | [Launch](https://sagarkalauni.github.io/confidence-and-prediction-interval/) |
| **Bootstrapping** | Non-Parametric Resampling with Replacement | [Launch](https://sagarkalauni.github.io/bootstrap/) |
| **Q-Q Plot** | Gaussian Normality & Tail Diagnostics | [Launch](https://sagarkalauni.github.io/qq-plot/) |
| **Train-Test Split & CV** | Holdout Partitioning & $K$-Fold Cross-Validation | [Launch](https://sagarkalauni.github.io/split/) |
| **One-Hot Encoding** | Categorical Expansion & Dummy Variable Trap | [Launch](https://sagarkalauni.github.io/one-hot-encoding/) |

---

<div align="center">
  <sub>Developed with ❤️ for Data Science students by <a href="https://github.com/SagarKalauni">Sagar Kalauni</a> · <a href="https://sagarkalauni.github.io">Portfolio</a></sub>
</div>
