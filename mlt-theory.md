# 🎯 MACHINE LEARNING TECHNIQUES (23CSC02)
## 📚 THE ULTIMATE CENTUM THEORETICAL STUDY GUIDE (100/100)
### Sri Krishna College of Technology | B.E. CSE(AIML) | Semester 4

```
╔════════════════════════════════════════════════════════════════════════╗
║  📋 GUIDE STRUCTURE                                                     ║
║  ─────────────────────────────────────────────────────────────────    ║
║  ✅ Unit 1: Introduction & Mathematical Foundations                    ║
║  ✅ Unit 2: Supervised & Unsupervised Learning                         ║
║  ✅ Unit 3: Probabilistic Methods & Deep Learning                      ║
║                                                                        ║
║  🎯 FEATURES:                                                          ║
║  • 100% THEORETICAL CONTENT — No numericals                            ║
║  • All CIA/Assignment questions integrated as explanatory content     ║
║  • Complete formula reference under respective topics                  ║
║  • ASCII diagrams only where essential for conceptual clarity          ║
║  • Every concept from all provided materials covered                   ║
╚════════════════════════════════════════════════════════════════════════╝
```

---

# 📘 UNIT 1: INTRODUCTION AND MATHEMATICAL FOUNDATIONS

---

## 1.1 WHAT IS MACHINE LEARNING?

### Definition
**Machine Learning (ML)** is a subset of Artificial Intelligence (AI) that enables systems to **learn from data** and **improve from experience** without being explicitly programmed. It discovers the underlying function `f(x)` that maps inputs `X` to outputs `Y`.

```
Mathematical Formulation:
Y = f(X) + ε
where:
- X = Input features (independent variables)
- Y = Target output (dependent variable)  
- f = Unknown function to be learned
- ε = Irreducible error (noise)
```

### The AI Landscape Hierarchy
```
┌─────────────────────────────────────────┐
│  ARTIFICIAL INTELLIGENCE                │
│  (Mimicking Human Intelligence)         │
│  ┌─────────────────────────────────┐    │
│  │  MACHINE LEARNING               │    │
│  │  (Learning from Data/Experience)│   │
│  │  ┌─────────────────────────┐    │    │
│  │  │  DEEP LEARNING          │    │    │
│  │  │  (Neural Networks)      │    │    │
│  │  └─────────────────────────┘    │    │
│  └─────────────────────────────────┘    │
└─────────────────────────────────────────┘
```

### History & Evolution of Machine Learning
| Era | Milestone | Significance |
|-----|-----------|-------------|
| **1950s** | Perceptron (Rosenblatt) | First neuron-inspired algorithm; foundation of neural networks |
| **1970s-80s** | AI Winter | Hype exceeded computational reality; reduced funding |
| **1990s** | SVM & Kernel Methods | Mathematical rigor; strong theoretical foundations |
| **2006-2012** | Deep Learning Revival | Hinton's breakthrough; ImageNet competition; GPU acceleration |
| **2017-Present** | Transformers & LLMs | Attention mechanisms; Generative AI; Foundation models |

### Why Machine Learning Now? (The Need)
```
┌────────────────────────────────────────────────────┐
│  📊 VOLUME                                          │
│  • Petabytes of data generated daily               │
│  • Human analysis impossible at this scale         │
│  • ML processes big data efficiently               │
├────────────────────────────────────────────────────┤
│  🔍 COMPLEXITY                                      │
│  • Non-linear patterns in high-dimensional space   │
│  • Hidden relationships traditional stats miss     │
│  • ML discovers complex feature interactions       │
├────────────────────────────────────────────────────┤
│  ⚡ SPEED                                           │
│  • Millisecond decisions for real-time systems     │
│  • Algorithmic trading, fraud detection, IoT       │
│  • Scalable inference on edge devices              │
└────────────────────────────────────────────────────┘
```

### Applications of Machine Learning

**Healthcare - Disease Prediction**
- ML models analyze patient records, lab results, and imaging data
- Predict disease risk (diabetes, cancer, heart disease) before symptoms appear
- Example: Models predicting ICU admission risk using patient vitals and history

**E-commerce - Recommendation Systems**
- Collaborative filtering suggests products based on similar users' behavior
- Content-based filtering recommends items similar to previously liked products
- ML analyzes large volumes of user behavior data (clicks, purchases, browsing history) to identify patterns and similarities between users, personalizing recommendations dynamically without explicit programming rules

**Email Spam Detection**
- Binary classification problem under Supervised Learning
- Techniques like Naive Bayes or Logistic Regression assign one of two labels — spam or not spam — based on email content features
- Classifying emails as spam or not spam based on content patterns

**Medical Diagnosis**
- Predicting diseases from patient data such as symptoms and test results
- ML models predict disease risk with high accuracy, enabling early diagnosis and better treatment

**Finance - Fraud Detection**
- Fraud detection systems analyze transaction patterns in real-time and flag suspicious activities, protecting users from unauthorized transactions

**Additional High-Impact Applications:**
- 🚗 Autonomous Vehicles: CNNs for object detection, RNNs for trajectory prediction
- 💬 Natural Language Processing: Transformers for translation, sentiment analysis
- 🔐 Cybersecurity: Anomaly detection for intrusion prevention
- 🎵 Entertainment: Personalization using matrix factorization
- 🏠 Real Estate: Predicting house prices using features like size and location via Linear Regression

### Advantages, Disadvantages & Challenges of Machine Learning

| Advantages | Disadvantages | Challenges |
|------------|--------------|------------|
| ✅ Automates repetitive tasks | ❌ Requires large, quality datasets | 🔴 Data bias and fairness issues |
| ✅ Discovers hidden patterns | ❌ Computationally expensive | 🔴 Model interpretability (black box) |
| ✅ Improves with more data | ❌ Risk of overfitting/underfitting | 🔴 Distribution shift (train≠test) |
| ✅ Handles high-dimensional data | ❌ Needs domain expertise for features | 🔴 Adversarial vulnerability |
| ✅ Real-time decision making | ❌ Ethical and privacy concerns | 🔴 Resource-intensive training |

### Why Machine Learning is Considered Data-Dependent
ML algorithms learn patterns directly from training data. Without sufficient, high-quality, and representative data, the model cannot generalize well. The accuracy and reliability of any ML model is entirely governed by the data it is trained on — hence it is data-dependent.

---

## 1.2 TYPES OF MACHINE LEARNING PROBLEMS

### The Four Paradigms
```
MACHINE LEARNING
│
┌─────────┬──────────┼──────────┬─────────┐
│         │          │          │         │
SUPERVISED  UNSUPER-  SEMI-      REINFORCE-
LEARNING    VISED     SUPERVISED MENT
(Teacher)   (Explorer) (Hybrid)  (Agent)
```

### Supervised Learning
**Concept:** Model learns from **labeled dataset** where both input `X` and target `Y` are known.

**Types:**
| Type | Output | Example | Algorithm Examples |
|------|--------|---------|-------------------|
| **Regression** | Continuous value | House price prediction, sales forecasting | Linear Regression, SVR |
| **Classification** | Categorical label | Spam detection, disease diagnosis | Logistic Regression, SVM, Decision Trees, Naive Bayes |

**Regression Task Characteristics:**
- Predicts continuous numerical output (future sales, house prices)
- Based on historical trend data
- Specifically Time Series Forecasting for temporal data
- Linear Regression or Multiple Linear Regression suitable when input features have linear relationship with output

**Classification Task Characteristics:**
- Binary Classification: Two labels (spam/not spam, default/no default)
- Multi-class Classification: Multiple discrete categories
- Assigns class labels based on input feature patterns

### Unsupervised Learning
**Concept:** Model learns from **unlabeled data** to discover hidden structures or patterns.

**Types:**
| Type | Goal | Example | Algorithm |
|------|------|---------|-----------|
| **Clustering** | Group similar items | Customer segmentation, document grouping | K-Means, Hierarchical |
| **Association** | Find rule-based links | Market basket analysis | Apriori, FP-Growth |
| **Dimensionality Reduction** | Reduce features while preserving information | Visualizing high-D data | PCA, t-SNE |

### Semi-Supervised & Reinforcement Learning
**Semi-Supervised Learning:**
- Uses small labeled dataset + large unlabeled dataset
- Cost-effective when labeling is expensive (medical imaging, speech data)
- Example: Self-training where confident predictions become pseudo-labels

**Reinforcement Learning:**
```
Agent → Action → Environment → Reward → Update Policy
↑_______________________↓
```
- Agent learns optimal policy through trial-and-error
- Applications: Game playing (AlphaGo), robotics, autonomous navigation

---

## 1.3 MATHEMATICAL FOUNDATIONS I: LINEAR ALGEBRA & ANALYTICAL GEOMETRY

### Vectors and Matrices in ML
**Vector:** An ordered array of numbers representing features.
```
Example: House features as vector
x = [Area_sqft, Bedrooms, Bathrooms, Age_years]
x = [1500, 3, 2, 10]
```

**Matrix:** A 2D array where rows = samples, columns = features.
```
Dataset X (m samples, n features):
[x₁₁  x₁₂  ...  x₁ₙ]
X = [x₂₁  x₂₂  ...  x₂ₙ]   (m × n matrix)
[ ⋮    ⋮   ⋱    ⋮  ]
[xₘ₁  xₘ₂  ...  xₘₙ]
```

### Matrix Multiplication Perspectives
Given matrices A (m×p) and B (p×n), product C = AB (m×n):

**Dot Product (Row-Column) View:**
```
C[i,j] = Row_i(A) • Column_j(B) = Σₖ A[i,k] × B[k,j]
```

**Column View (Linear Combination):**
```
Each column of C is a linear combination of columns of A
C[:,j] = Σₖ B[k,j] × A[:,k]
```

**Row View:**
```
Each row of C is a linear combination of rows of B
C[i,:] = Σₖ A[i,k] × B[k,:]
```

**Outer Product View:**
```
AB = Σₖ (Column_k of A) × (Row_k of B)
Each term is a rank-1 matrix
```

### Norms and Distance Metrics
| Norm | Formula | Name | Use Case |
|------|---------|------|----------|
| **L₁ Norm** | ‖x‖₁ = Σ\|xᵢ\| | Manhattan | Sparse solutions, Lasso |
| **L₂ Norm** | ‖x‖₂ = √(Σxᵢ²) | Euclidean | Least squares, Ridge |
| **L∞ Norm** | ‖x‖∞ = max\|xᵢ\| | Chebyshev | Worst-case analysis |

**Euclidean Distance Formula:**
```
d(x,y) = ‖x - y‖₂ = √Σ(xᵢ - yᵢ)²
```

**Manhattan Distance Formula:**
```
d(x,y) = ‖x - y‖₁ = Σ|xᵢ - yᵢ|
```

### Inner Product and Orthogonality
**Dot Product (Inner Product):**
```
⟨x, y⟩ = xᵀy = Σ xᵢyᵢ = ‖x‖‖y‖cos(θ)
```

**Orthogonality Condition:**
```
Vectors x and y are orthogonal ⟺ ⟨x, y⟩ = 0 ⟺ θ = 90°
```

### Eigenvalues and Eigenvectors (PCA Foundation)
**Definition:** For matrix A, eigenvector v and eigenvalue λ satisfy:
```
Av = λv
```
The eigenvector v doesn't change direction when transformed by A; it only scales by λ.

**Finding Eigenvalues:**
```
1. Solve characteristic equation: det(A - λI) = 0
2. For each λ, solve (A - λI)v = 0 for eigenvector v
```

**Key Properties:**
```
• Trace(A) = Σλᵢ  (sum of diagonal = sum of eigenvalues)
• det(A) = Πλᵢ   (determinant = product of eigenvalues)
• If A is singular → at least one λ = 0
• Symmetric matrices have real eigenvalues & orthogonal eigenvectors
```

### Matrix Centering and Covariance (PCA Preprocessing)
**Mean Vector:** μ = (1/n)Σxᵢ for each feature

**Centered Data:** X' = X - μ (subtract mean from each feature)

**Covariance Matrix:** C = (1/n) X'ᵀX'

Centered data has zero mean per feature — essential for PCA.

---

## 1.4 MATHEMATICAL FOUNDATIONS II: PROBABILITY & STATISTICS

### Descriptive Statistics for ML
| Measure | Formula | ML Application |
|---------|---------|---------------|
| **Mean (μ)** | μ = (1/n)Σxᵢ | Feature centering, normalization |
| **Variance (σ²)** | σ² = (1/n)Σ(xᵢ-μ)² | Feature scaling, outlier detection |
| **Standard Deviation (σ)** | σ = √σ² | Z-score normalization |
| **Covariance** | Cov(X,Y) = E[(X-μₓ)(Y-μᵧ)] | Feature correlation, PCA |

### Bayesian Conditional Probability (Foundation of Naive Bayes)
**Bayes' Theorem:**
```
                P(B|A) × P(A)
P(A|B) = -----------------------
                     P(B)
```

| Term | Name | Interpretation |
|------|------|---------------|
| P(A|B) | **Posterior** | Updated belief about A after observing B |
| P(B|A) | **Likelihood** | Probability of evidence B if hypothesis A is true |
| P(A) | **Prior** | Initial belief about A before seeing evidence |
| P(B) | **Evidence** | Normalizing constant: total probability of B |

### Law of Total Probability (Evidence Calculation)
```
P(B) = P(B|A)×P(A) + P(B|¬A)×P(¬A)
```
This computes the marginal probability of B by summing over all possible causes.

### Asymmetry of Conditional Probability
```
P(A|B) ≠ P(B|A) in general
```
P(A|B) is the probability of A given B, while P(B|A) is the probability of B given A. These are generally not equal. This is the foundation of Bayes' Theorem — which provides a way to relate and compute one from the other.

### Random Variable in Probability and ML
A random variable is a variable whose value is determined by the outcome of a random experiment. In ML, it represents uncertain quantities such as input features or output labels. It can be:
- **Discrete:** Finite outcomes (e.g., class labels)
- **Continuous:** Infinite outcomes (e.g., house prices, temperatures)

---

## 1.5 MATHEMATICAL FOUNDATIONS III: VECTOR CALCULUS & OPTIMIZATION

### Gradient and Optimization
**Gradient (∇):** Vector of partial derivatives pointing in direction of steepest ascent.
```
For f(x₁,x₂,...,xₙ):
∇f = [∂f/∂x₁, ∂f/∂x₂, ..., ∂f/∂xₙ]ᵀ
```

**Gradient Descent Algorithm:**
```
Goal: Minimize loss function L(w)
Initialize: w₀ (random weights)
Repeat until convergence:
  1. Compute gradient: g = ∇L(wₖ)
  2. Update weights: wₖ₊₁ = wₖ - α·g
  3. Check convergence: |L(wₖ₊₁) - L(wₖ)| < ε
where α = learning rate (step size)
```

### ASCII Diagram: Gradient Descent Landscape
```
Loss L(w)
^
|     *  ← Starting point
|    / \
|   /   \      Gradient points ↑ (steepest ascent)
|  /     \     We move ↓ opposite to gradient
| /       \
|/         \___
+------------------> Weights (w)
        ↑
   Global Minimum
```

### Why Square the Error in MSE?
**Three Critical Reasons:**
```
1️⃣ Avoids Cancellation
• Errors can be positive or negative
• Sum of absolute errors: +5 and -5 cancel to 0 (misleading)
• Squared errors: 25 + 25 = 50 (properly penalizes both)

2️⃣ Penalizes Large Errors Heavily
• Error of 2 → penalty = 4
• Error of 4 → penalty = 16 (4× larger, not 2×)
• Forces model to care about outliers

3️⃣ Differentiable Everywhere
• |x| has sharp corner at x=0 → derivative undefined
• x² is smooth → gradient exists everywhere
• Enables gradient-based optimization (essential for training)
```

---

## 1.6 MATHEMATICAL FOUNDATIONS IV: INFORMATION & DECISION THEORY

### Information Theory: Quantifying Uncertainty
**Self-Information:**
```
I(x) = -log₂(P(x))
• Rare event (P small) → high information
• Common event (P large) → low information
```

**Entropy H(X): Average Uncertainty**
```
H(X) = -Σ P(x)·log₂(P(x))
Properties:
• H = 0 → perfectly predictable (one outcome certain)
• H = max → maximum uncertainty (uniform distribution)
• Measured in bits (log base 2)
```

### Information Gain (Decision Tree Splitting Criterion)
**Formula:**
```
IG(S, A) = H(S) - Σᵥ (|Sᵥ|/|S|) · H(Sᵥ)
where:
• S = parent dataset
• A = attribute being tested
• Sᵥ = subset where attribute A = value v
• |·| = number of samples
```

**Interpretation:** Information Gain = Reduction in entropy after splitting on attribute A. Higher IG = better split.

### Decision Theory: Expected Risk & Bayes Decision Rule
**Loss Function L(y, ŷ):** Cost of predicting ŷ when true label is y.

**Expected Risk for action a:**
```
R(a|x) = Σᵧ L(y, a) · P(y|x)
```

**Bayes Decision Rule:** Choose action a* that minimizes expected risk:
```
a* = argminₐ R(a|x)
```

---

## 📝 UNIT 1 SUMMARY CHEAT SHEET
```
┌─────────────────────────────────────────────────────────┐
│  🔑 KEY FORMULAS - UNIT 1                                │
├─────────────────────────────────────────────────────────┤
│  • Euclidean Distance: d = √Σ(xᵢ-yᵢ)²                    │
│  • Dot Product: ⟨x,y⟩ = Σxᵢyᵢ = ‖x‖‖y‖cosθ              │
│  • Bayes: P(A|B) = P(B|A)P(A)/P(B)                      │
│  • Evidence: P(B) = P(B|A)P(A) + P(B|¬A)P(¬A)           │
│  • Entropy: H(X) = -ΣP(x)log₂P(x)                       │
│  • Info Gain: IG = H(parent) - Σ(|Sᵥ|/|S|)H(Sᵥ)         │
│  • Gradient Descent: w ← w - α∇L(w)                     │
│  • Eigenvalue: Av = λv → det(A-λI)=0                    │
│  • Covariance: C = (1/n)X'ᵀX'                           │
├─────────────────────────────────────────────────────────┤
│  🎯 EXAM TIPS                                            │
│  • Always verify eigenvalues: Trace=Σλ, Det=Πλ          │
│  • For Bayes: compute evidence P(B) using total prob    │
│  • Entropy max at uniform distribution (H=1 for binary) │
│  • Gradient points uphill; descend opposite direction   │
│  • Column perspective: Wx = Σxᵢ·(columnᵢ of W)          │
└─────────────────────────────────────────────────────────┘
```

---

# 📘 UNIT 2: SUPERVISED AND UNSUPERVISED LEARNING

---

## 2.1 INTRODUCTION: DISCRIMINATIVE vs GENERATIVE MODELS

### Fundamental Distinction
| Aspect | Discriminative Models | Generative Models |
|--------|---------------------|-------------------|
| **Learns** | P(Y|X) directly | P(X,Y) = P(X|Y)P(Y) |
| **Focus** | Decision boundary | Data distribution |
| **Question** | "Which class is this?" | "What does each class look like?" |
| **Can Generate** | ❌ No | ✅ Yes (synthetic data) |
| **Examples** | Logistic Regression, SVM, Decision Trees, Neural Nets | Naive Bayes, HMM, GMM, GANs |

### When to Use Which?
```
✅ Use Discriminative When:
• Primary goal is accurate classification
• Limited training data
• Features are high-dimensional

✅ Use Generative When:
• Need to generate new samples
• Handling missing data (can marginalize)
• Semi-supervised learning (use unlabeled data)
• Modeling causal relationships
```

---

## 2.2 LINEAR REGRESSION & LEAST SQUARES

### Model Formulation
```
Hypothesis: h_w(x) = w₀ + w₁x₁ + w₂x₂ + ... + wₙxₙ = wᵀx
Vector Form: ŷ = Xw  (X: m×n design matrix, w: n×1 weights)
```

### Cost Function: Mean Squared Error (MSE)
```
J(w) = (1/2m) Σᵢ₌₁ᵐ (h_w(x⁽ⁱ⁾) - y⁽ⁱ⁾)²
     = (1/2m) ‖Xw - y‖²
```

### Normal Equation (Analytical Solution)
```
Optimal weights: w* = (XᵀX)⁻¹Xᵀy

Derivation:
1. Set gradient ∇J(w) = 0
2. ∇J = (1/m)Xᵀ(Xw - y) = 0
3. XᵀXw = Xᵀy
4. w = (XᵀX)⁻¹Xᵀy
```

### Linear Dependence and Normal Equation Limitations
If the dataset is linearly dependent, XᵀX becomes **SINGULAR (non-invertible)**.

**Causes:**
• Perfect multicollinearity: One feature = linear combo of others
• More features than samples: n > m
• Redundant features included

**Consequences:**
• (XᵀX)⁻¹ does not exist → Normal equation fails
• Infinite solutions: Many w give same minimum loss

**Solutions:**
1️⃣ Remove redundant features (feature selection)
2️⃣ Use Regularization: Ridge adds λI to make XᵀX+λI invertible
3️⃣ Use Gradient Descent (doesn't require matrix inverse)
4️⃣ Apply PCA to reduce to independent components

---

## 2.3 UNDERFITTING, OVERFITTING & REGULARIZATION

### The Bias-Variance Tradeoff
```
Total Error = Bias² + Variance + Irreducible Error

┌─────────────────────────────────────────┐
│  Underfitting (High Bias)               │
│  • Model is too simple to capture underlying patterns │
│  • Both training and test errors are high │
│  • Model fails to capture trend         │
│  • Fix: More complex model, more features│
├─────────────────────────────────────────┤
│  Overfitting (High Variance)            │
│  • Model learns training data too well including noise │
│  • Training accuracy very high, test accuracy poor │
│  • Large gap between train and test performance │
│  • Fix: Regularization, more data, pruning│
└─────────────────────────────────────────┘
```

### ASCII Diagram: Bias-Variance Tradeoff
```
Error
^
|                    Test Error
|                   /
|                  /
|                 / ← Optimal Point
|                /\
|               /  \
|              /    \
|    Train Error    \
|   .................\..........
+--------------------------------> Model Complexity
   Simple          Complex
  (Underfit)      (Overfit)
```

### Regularization: Lasso (L1) vs Ridge (L2)
| Type | Penalty Term | Effect | Use Case |
|------|-------------|--------|----------|
| **Ridge (L2)** | λΣwⱼ² | Shrinks coefficients toward 0 | Many small effects, multicollinearity |
| **Lasso (L1)** | λΣ|wⱼ| | Sets some coefficients EXACTLY to 0 | Feature selection, sparse models, high-dimensional data |

### Lasso Regression for Feature Selection
With many features where many are irrelevant, standard regression assigns small non-zero weights to all features, creating noise. Lasso shrinks irrelevant feature weights exactly to zero, effectively performing automatic feature selection.

**Geometric Intuition:** Lasso's constraint region is a diamond shape in weight space. The loss function's ellipse touches the diamond at a corner — a corner means one or more weights equal zero. This is unlike Ridge (L2) whose circular constraint rarely touches axes.

**Advantages of Lasso Over Ridge:**
• Feature selection (sparse solution) vs all features retained
• Weights go to exactly zero vs weights only shrink toward zero
• Better for high-dimensional sparse problems vs when all features are relevant

### Solutions Summary for Underfitting/Overfitting
| Problem | Solution |
|---------|----------|
| Underfitting | Add more features, increase model complexity, reduce regularization, use polynomial features |
| Overfitting | Regularization (L1/L2), more training data, cross-validation, dropout (neural networks), early stopping, reduce model complexity |

---

## 2.4 CROSS-VALIDATION

### Definition and Importance
Cross-validation is a model evaluation technique where the dataset is split into multiple folds. The model is trained on some folds and tested on the remaining fold, repeated across all folds.

**Importance:**
• Reduces overfitting during evaluation
• Gives a reliable estimate of model performance on unseen data
• Makes efficient use of limited data
• Provides robust performance estimate through averaging

### K-Fold Cross-Validation Procedure
```
Algorithm:
1. Shuffle dataset randomly
2. Split into K equal folds (typically K=5 or 10)
3. For each fold i = 1 to K:
   a. Use fold i as validation set
   b. Train on remaining K-1 folds
   c. Evaluate on fold i → record metric
4. Final score = average of K validation scores
```

### ASCII Diagram: 5-Fold CV
```
Dataset: [1][2][3][4][5]  (5 folds)

Iter 1: [TEST][Train][Train][Train][Train] → Acc₁
Iter 2: [Train][TEST][Train][Train][Train] → Acc₂
Iter 3: [Train][Train][TEST][Train][Train] → Acc₃
Iter 4: [Train][Train][Train][TEST][Train] → Acc₄
Iter 5: [Train][Train][Train][Train][TEST] → Acc₅

Final Accuracy = (Acc₁+Acc₂+Acc₃+Acc₄+Acc₅) / 5
```

### Interpreting Cross-Validation Results
Slightly different errors across folds is **normal and expected**. This indicates variance in the model's performance across different subsets of data. Slightly different errors show that the model is sensitive to the specific training/test split. The average of all fold errors gives a robust performance estimate.

**If errors differ GREATLY:**
• Possible data leakage in some folds
• Class imbalance not stratified
• Small dataset → high sampling variance

**Best Practice:** Use Stratified K-Fold for classification to maintain class distribution in each fold.

### Types of Cross-Validation
1. **K-Fold** — data split into K equal folds (most common)
2. **Stratified K-Fold** — maintains class distribution in each fold
3. **Leave-One-Out (LOO)** — K = N (one sample as test each time)
4. **Time Series Split** — respects temporal order for sequential data

### Role in Hyperparameter Tuning
Cross-validation is used in Grid Search to select the best hyperparameters:
• Try different values of learning rate, depth, regularization
• Select combination with lowest average CV error
• Prevents selection bias from a single train-test split

---

## 2.5 LOGISTIC REGRESSION & CLASSIFICATION

### From Linear to Logistic: The Sigmoid Transformation
**Problem with Linear Regression for Classification:**
- Outputs unbounded values (-∞ to +∞)
- Not interpretable as probabilities

**Solution: Sigmoid Function**
```
σ(z) = 1 / (1 + e⁻ᶻ)

Properties:
• Maps any real z to (0, 1) → interpretable as probability
• Differentiable everywhere → enables gradient descent
• S-shaped curve: smooth transition between classes
```

### Decision Boundary & Threshold
```
Prediction Rule:
IF σ(wᵀx) ≥ 0.5 → Class 1
ELSE → Class 0

Note: Threshold 0.5 is adjustable based on cost of FP vs FN
```

### Loss Function: Log Loss (Cross-Entropy)
```
For single sample:
L = -[y·log(ŷ) + (1-y)·log(1-ŷ)]

For m samples:
J(w) = -(1/m) Σᵢ [y⁽ⁱ⁾log(ŷ⁽ⁱ⁾) + (1-y⁽ⁱ⁾)log(1-ŷ⁽ⁱ⁾)]

Why Log Loss?
• Heavily penalizes confident wrong predictions
• Convex → guaranteed global minimum with gradient descent
• Derived from Maximum Likelihood Estimation
```

### Logistic Regression for Bank Loan Default Prediction
**Model Application:**
Logistic Regression is a supervised classification algorithm that models the probability of a binary outcome (Default = Yes/No). Unlike Linear Regression which predicts continuous values, Logistic Regression maps predictions to probabilities between 0 and 1 using the Sigmoid function.

**Features (inputs):**
• Credit Score, Monthly Income, Loan Amount, Employment Status (0/1), Debt-to-Income Ratio

**Training:** The model learns weights and bias by minimizing Binary Cross-Entropy Loss using gradient descent.

**Probability Output and Decision Threshold:**
After training, for a new customer with feature vector X:
P(Default) = σ(wᵀX + b)

**Decision Threshold (τ):**
• Default: τ = 0.5 → If P ≥ 0.5, classify as Default (1), else No Default (0)
• Banks can adjust τ based on risk tolerance:
  - Lower τ (e.g., 0.3) → More conservative, catches more defaults but may reject good customers
  - Higher τ (e.g., 0.7) → More lenient, approves more customers but higher default risk

**Model Evaluation Metrics:**
| Metric | Purpose |
|--------|---------|
| Accuracy | Overall correct predictions |
| Precision | Of predicted defaults, how many actually defaulted |
| Recall | Of actual defaults, how many were caught |
| AUC-ROC | Measures performance across all thresholds |

**Advantages for Banks:**
1. Interpretable — each weight explains feature importance
2. Outputs probability (not just class label)
3. Computationally efficient
4. Threshold can be tuned to business risk

---

## 2.6 SUPPORT VECTOR MACHINES (SVM)

### Maximum Margin Classifier
**Core Idea:** Find hyperplane that separates classes with MAXIMUM margin.
```
Decision Boundary: wᵀx + b = 0
Margin = 2 / ‖w‖  (distance between support vectors)

Optimization Problem:
Minimize: (1/2)‖w‖²
Subject to: yᵢ(wᵀxᵢ + b) ≥ 1 for all i

Why maximize margin? Better generalization (Structural Risk Minimization)
```

### ASCII Diagram: SVM Margin
```
Class +1          Class -1
  +                 -
  +   [SV+]    [SV-]   -
  +      |<--margin-->|   -
  +      |     |     |   -
  +      |  wᵀx+b=0 |   -   ← Optimal Hyperplane
  +      |_________|   -
  +                 -

SV+ and SV- = Support Vectors (define the margin)
Points not on margin don't affect the solution!
```

### Role of Support Vectors
Support vectors are the data points closest to the hyperplane. They alone define the margin — removing other points doesn't change the hyperplane. They support the margin boundary.

### Soft Margin SVM (for non-separable data)
When data is not perfectly linearly separable, we allow some misclassifications using slack variables (ξᵢ ≥ 0):
```
Minimize: (1/2)‖w‖² + C·Σ(ξᵢ)
```

**C is the regularization parameter:**
• High C = less margin, fewer errors allowed (risk of overfitting)
• Low C = wider margin, more errors allowed (risk of underfitting)

### Kernel Trick: Handling Non-Linear Data
**Problem:** Data not linearly separable in original space.

**Solution:** Map to higher dimension where separation is possible.

**Kernel Function:** K(x,z) = φ(x)ᵀφ(z)
• Computes dot product in high-D space WITHOUT explicit mapping φ
• Computational shortcut: "Kernel Trick"

### Types of Kernels
| Kernel | Formula | Use Case |
|--------|---------|----------|
| **Linear** | K(x,z) = xᵀz | Linearly separable data |
| **Polynomial** | K(x,z) = (xᵀz + c)ᵈ | Non-linear, degree d |
| **RBF/Gaussian** | K(x,z) = exp(-‖x-z‖²/2σ²) | Most popular, any shape |
| **Sigmoid** | K(x,z) = tanh(αxᵀz + c) | Neural net similarity |

### Why RBF Kernel is Most Widely Used
The RBF (Radial Basis Function/Gaussian) kernel is most widely used because:
• It can model ANY smooth decision boundary
• Works well in practice across diverse problems
• Has only one hyperparameter (sigma) to tune
• Maps to infinite-dimensional space implicitly

---

## 2.7 INSTANCE-BASED METHODS: K-NEAREST NEIGHBORS (KNN)

### Definition and Characteristics
KNN is a non-parametric, lazy supervised learning algorithm. For a new query point, it finds the K training points closest to it and predicts the class by majority voting (classification) or average value (regression).

**Key Properties:**
• No explicit training phase — memorizes entire training dataset
• Prediction made by comparing query point to stored examples at test time
• Non-parametric: No assumptions about data distribution

### Algorithm — Step by Step
```
1. Choose the value of K (number of neighbours)
2. Compute the distance from the query point to ALL training points
3. Sort distances in ascending order
4. Select the K nearest training points
5. For classification → majority vote; For regression → mean value
6. Return prediction
```

### Distance Metrics
| Metric | Formula | Properties |
|--------|---------|------------|
| **Euclidean** | d = √Σ(xᵢ-yᵢ)² | Most common; sensitive to scale |
| **Manhattan** | d = Σ|xᵢ-yᵢ| | Robust to outliers; grid-like paths |
| **Minkowski** | d = (Σ|xᵢ-yᵢ|ᵖ)¹/ᵖ | Generalizes both (p=1: Manhattan, p=2: Euclidean) |

### ASCII Diagram — KNN Voting
```
Training Data: Query Point: Q=(3, 3), K= 3

(1,1)-> Class A    Distances:
(2,2)-> Class A    d(Q,(1,1))= sqrt(8) = 2.83
(4,3)-> Class A    d(Q,(2,2))= sqrt(2) = 1.41 *
(5,4)-> Class B    d(Q,(4,3))= sqrt(1) = 1.00 *
(6,5)-> Class B    d(Q,(5,4))= sqrt(5) = 2.24 *
                   d(Q,(6,5))= sqrt(13)= 3.61

3 nearest: (2,2)A, (4,3)A, (5,4)B  → Majority: A (2 votes)
Prediction: Q belongs to Class A
```

### Effect of K Value
| K Value | Behaviour | Risk |
|---------|-----------|------|
| **K = 1** | Very sensitive to noise, complex boundary | Overfitting (high variance) |
| **K = optimal** | Smooth boundary, good generalization | Cross-validate to find best K |
| **K = N (all data)** | Always predicts majority class | Underfitting (high bias) |

### Why Feature Scaling is Important in KNN
KNN relies on distance. Features with larger ranges dominate the distance computation. Example: Feature A (0-1), Feature B (0-1000). B dominates. Solution: normalize all features to same scale (e.g., min-max scaling to [0,1]).

### Similarity vs Dissimilarity Measures
**Similarity measure:** Higher value = more similar (e.g., cosine similarity 0 to 1).

**Dissimilarity measure:** Higher value = more different (e.g., Euclidean distance ≥ 0).

KNN typically uses dissimilarity (distance) — closer points have smaller distance.

### Distinguishing Decision Tree and KNN Classification
| Decision Tree | KNN |
|--------------|-----|
| Builds a tree using feature splits | Stores all training points |
| Classifies by traversing tree rules | Classifies by majority vote of K nearest neighbors |
| Fast prediction after training | Slow prediction (computes distances) |
| Interpretable | Less interpretable |

---

## 2.8 TREE-BASED METHODS: DECISION TREES

### Definition and Structure
A Decision Tree is a supervised learning algorithm that models decisions using a tree-like structure. It recursively partitions the feature space into regions using a 'Divide and Conquer' strategy. Each internal node tests a feature, each branch is the outcome, and each leaf node gives the prediction.

### ASCII Tree Diagram
```
         [ROOT NODE]
         Feature: Outlook
         /      |      \
     Sunny  Overcast  Rainy
       |       |        |
 [Internal] [LEAF] [Internal]
 Humidity=?  Play   Wind=?
    / \      Yes    /   \
 High  Normal   Strong  Weak
   |       |      |       |
 [LEAF] [LEAF] [LEAF] [LEAF]
  No    Yes    No    Yes
```

### ID3 Algorithm — Using Entropy and Information Gain
**Entropy — Measures impurity/disorder of a dataset:**
```
H(S) = -Σ p(x)·log₂(p(x))
where p(x) = proportion of class x in set S
H = 0 → perfectly pure (all same class)
H = 1 → maximum impurity (50-50 split for binary)
```

**Information Gain — Measures how much an attribute reduces entropy:**
```
IG(S, A) = H(S) - Σᵥ[(|Sᵥ|/|S|)·H(Sᵥ)]
S = entire dataset, A = attribute, Sᵥ = subset where A = value v
```

ID3 selects the attribute with the **HIGHEST Information Gain**.

### CART Algorithm — Using Gini Index
**Gini Index — Measures probability of misclassification:**
```
Gini(S) = 1 - Σ pᵢ²
pᵢ = proportion of class i
Gini = 0 → pure node (all same class)
Gini = 0.5 → maximum impurity (binary, 50-50)
```

**Gini Gain (split quality):**
```
Gini_split = (|S_L|/|S|)·Gini(S_L) + (|S_R|/|S|)·Gini(S_R)
```
Select feature and threshold that **MINIMIZES Gini_split**.

### ID3 vs CART Comparison
| Property | ID3 | CART |
|----------|-----|------|
| Split Criterion | Information Gain (Entropy) | Gini Index |
| Tree type | Multi-way splits | Binary splits only |
| Task | Classification only | Classification & Regression |
| Data handling | Handles only categorical data | Handles both categorical and numerical |
| Missing values | Not handled | Handled |
| Pruning | No pruning | Supports pruning |

### What is Information Gain and How is it Used in ID3?
IG measures the reduction in entropy of dataset S after splitting on attribute A. IG(S,A) = H(S) - Σᵥ[(|Sᵥ|/|S|)·H(Sᵥ)]. ID3 selects the attribute with the HIGHEST information gain at each node, building the tree top-down recursively until all leaves are pure or data runs out.

### Comparing Entropy and Gini Index
**Entropy:** H = -Σ[p·log₂(p)] → range [0, 1] for binary, computationally expensive due to logarithm.

**Gini:** G = 1-Σ[p²] → range [0, 0.5] for binary, computationally cheaper (no logarithm).

Both measure impurity. Gini is preferred in CART for efficiency. Both reach 0 for pure nodes, maximum at equal class distribution.

### What is Pruning in Decision Trees? Why is it Needed?
Pruning removes branches of the tree that provide little predictive power.

**Needed to prevent overfitting** — a fully grown tree memorizes training data.

**Pre-pruning:** Stop growing early (min samples, max depth).

**Post-pruning:** Grow full tree, then remove weak branches (cost-complexity pruning).

---

## 2.9 ENSEMBLE METHODS

### Concept
Ensemble methods combine multiple base learners (weak or strong) to produce a model with better predictive performance than any single model. The core idea is: multiple diverse models that make different errors, when combined, reduce overall error.

### Bagging (Bootstrap Aggregating)
Bagging trains multiple base learners on DIFFERENT random subsets of training data (bootstrap samples = sampling with replacement). Final prediction is made by majority voting (classification) or averaging (regression).

```
Full Dataset D (N samples)
│
Bootstrap Sampling (with replacement):
D1 = random sample of N from D -> Train Model 1 -> pred_1
D2 = random sample of N from D -> Train Model 2 -> pred_2
D3 = random sample of N from D -> Train Model 3 -> pred_3

Final = majority_vote(pred_1, pred_2, pred_3)
```

**KEY:** Reduces VARIANCE (overfitting) without increasing bias

### Boosting
Boosting trains models sequentially. Each new model focuses on the ERRORS made by the previous model. Misclassified examples get higher weight. Final prediction is a weighted sum of all model predictions.

```
Iteration 1: Train Model_1 on D (uniform weights)
            Identify misclassified points -> INCREASE their weight

Iteration 2: Train Model_2 on D (updated weights)
            Identify misclassified points -> INCREASE their weight

...

Final = w1·Model_1 + w2·Model_2 + ... + wT·Model_T
(w_i = confidence/accuracy of model i)
```

**KEY:** Reduces BIAS (underfitting). Examples: AdaBoost, Gradient Boost

### Random Forest
Random Forest is an ensemble of Decision Trees using Bagging + Feature Randomness. Each tree is trained on a bootstrap sample and uses a RANDOM subset of features at each split. This decorrelates the trees and reduces variance.

### Why Random Forest Performs Better Than a Single Decision Tree
1. **Multiple diverse trees:** each trained on different bootstrap samples of data
2. **Feature randomness:** at each split, only a RANDOM subset of features is considered — this decorrelates trees so they don't all make the same errors
3. **Majority voting:** errors of individual trees cancel out
4. **Result:** lower variance (less overfitting), better generalization

### Distinguishing Between Bagging and Boosting
| Bagging | Boosting |
|---------|----------|
| Parallel training | Sequential training |
| Random bootstrap subsets | Weighted data (focus on errors) |
| Reduces VARIANCE | Reduces BIAS |
| All models have equal weight | Models have unequal weights based on accuracy |
| Example: Random Forest | Example: AdaBoost, XGBoost |

### Comparison Table — Ensemble Methods
| Method | Training | Data Used | Reduces | Example |
|--------|----------|-----------|---------|---------|
| Bagging | Parallel | Bootstrap | Variance | Random Forest |
| Boosting | Sequential | Weighted | Bias | AdaBoost, XGBoost |
| Stacking | Sequential | Cross-val | Both | Meta-learner |

---

## 2.10 EVALUATION OF CLASSIFICATION MODELS

### Confusion Matrix Fundamentals
```
                    PREDICTED
              Positive      Negative
ACTUAL  Positive    TP         FN
        Negative    FP         TN

Definitions:
• TP: True Positive  (correctly predicted positive)
• TN: True Negative  (correctly predicted negative)
• FP: False Positive (Type I error: false alarm)
• FN: False Negative (Type II error: missed detection)
```

### Performance Metrics: Formulas & Use Cases
| Metric | Formula | When to Prioritize |
|--------|---------|-------------------|
| **Accuracy** | (TP+TN)/(TP+TN+FP+FN) | Balanced classes, equal cost of errors |
| **Precision** | TP/(TP+FP) | Cost of FP high (spam filter, fraud alert) |
| **Recall (Sensitivity)** | TP/(TP+FN) | Cost of FN high (cancer screening, security) |
| **F1-Score** | 2·(Prec·Rec)/(Prec+Rec) | Imbalanced classes, need balance |
| **Specificity** | TN/(TN+FP) | When true negatives matter (healthy diagnosis) |

### When to Use Which Metric? Decision Framework
```
┌─────────────────────────────────────────┐
│  Scenario: Imbalanced Dataset (1% fraud)│
│  → Accuracy misleading: 99% by always predicting "not fraud" │
│  → Use: Precision, Recall, F1, AUC-ROC  │
├─────────────────────────────────────────┤
│  Scenario: Medical Diagnosis            │
│  → Missing disease (FN) is catastrophic │
│  → Prioritize: HIGH RECALL              │
│  → Accept lower precision (more tests)  │
├─────────────────────────────────────────┤
│  Scenario: Spam Filtering               │
│  → False alarm (FP) annoys users        │
│  → Prioritize: HIGH PRECISION           │
│  → Accept missing some spam (lower recall)│
├─────────────────────────────────────────┤
│  Scenario: Model Selection              │
│  → Need single metric to compare models │
│  → Use: F1-Score or AUC-ROC             │
└─────────────────────────────────────────┘
```

---

## 2.11 CLUSTERING ALGORITHMS

### Definition
Clustering is an unsupervised learning method that groups similar data points together into clusters without using labelled data. The goal is to maximize intra-cluster similarity and minimize inter-cluster similarity.

### K-Means Algorithm
**Objective Function (Within-Cluster Sum of Squares):**
```
J = Σₖ Σ_{x∈Cₖ} ‖x - μₖ‖²
• μₖ = centroid of cluster k
• Cₖ = set of points assigned to cluster k
• Goal: Minimize total squared distance to centroids
```

**Algorithm Steps:**
```
1. Choose K (number of clusters)
2. Initialize K centroids randomly (or use K-Means++)
3. REPEAT until convergence:
   a. ASSIGNMENT: Assign each point to nearest centroid
      c⁽ⁱ⁾ = argminₖ ‖x⁽ⁱ⁾ - μₖ‖²
   b. UPDATE: Recompute centroids as mean of assigned points
      μₖ = (1/|Cₖ|) Σ_{i∈Cₖ} x⁽ⁱ⁾
4. Return cluster assignments and centroids
```

### ASCII Diagram — K-Means Iterations
```
Initial (K=2, random centroids*):
  ..*..          Centroid 1=*  Centroid 2=*
  .....
  ..... 
  .*...

Iteration 1 — ASSIGN (assign each point to nearest centroid):
  A A C A A      A=Cluster1, B=Cluster2
  B B B B B      C=equidistant, goes to one
  A A A A A
  B C B B B

Iteration 1 — UPDATE (recompute centroids):
  * moves to mean of A points
  * moves to mean of B points

Continue until centroids stop moving (convergence)
```

### How Changing K Affects K-Means Cluster Formation
• **Small K:** Fewer, larger clusters — may group unrelated points together (underfitting)
• **Large K:** Many small clusters — may split naturally grouped points (overfitting)
• **Optimal K:** Balances within-cluster cohesion and between-cluster separation. Found using the Elbow Method

### Disadvantages of K-Means
1. Must specify K in advance — unknown in practice
2. Sensitive to initialization (different random seeds may give different results)
3. Assumes spherical, equal-sized clusters — fails on complex shapes
4. Sensitive to outliers (outliers distort centroids)
5. May converge to local minimum (use K-Means++ for better initialization)

### Hierarchical Clustering
Hierarchical clustering builds a tree of clusters called a dendrogram. It does NOT require pre-specifying K.

| Type | Agglomerative (Bottom-Up) | Divisive (Top-Down) |
|------|---------------------------|---------------------|
| Start | Each point = own cluster | All points in one cluster |
| Process | Merge nearest clusters step by step | Split cluster into smaller ones |
| End | One big cluster (all points) | Each point = own cluster |
| Common? | YES — more popular | Less common |

### Linkage Methods in Hierarchical Clustering
- **Single Linkage:** min distance between any two points from different clusters — tends to create long chains
- **Complete Linkage:** max distance — creates compact clusters
- **Average Linkage:** average distance — compromise between single and complete
- **Ward Linkage:** minimize total within-cluster variance — most commonly used

### Cluster Validity — Elbow Method & Silhouette Score
**Elbow Method:** Plot inertia (J) vs K. The 'elbow point' where J stops decreasing rapidly is the optimal K.

**Silhouette Score:** Measures how well each point fits in its cluster vs others:
```
s(i) = (b(i) - a(i)) / max(a(i), b(i))
a(i) = avg distance to points in SAME cluster
b(i) = avg distance to points in NEAREST other cluster
```
s(i) ranges from -1 to 1: 1 = well clustered, 0 = on boundary, -1 = wrong cluster

---

## 2.12 DIMENSIONALITY REDUCTION: PRINCIPAL COMPONENT ANALYSIS (PCA)

### Definition and Purpose
Principal Component Analysis (PCA) is an unsupervised technique that reduces the number of features (dimensions) while preserving the maximum variance in the data. It transforms data into a new coordinate system where axes (principal components) are ordered by the amount of variance they explain.

### Why Reduce Dimensions?
```
✅ Benefits:
• Remove redundant/correlated features
• Combat the Curse of Dimensionality
• Reduce computational cost
• Easier visualization (project to 2D or 3D)
• Reduce noise in data
```

### PCA Algorithm — Step by Step
```
1. MEAN CENTER the data — subtract mean from each feature: X' = X - mean(X)
2. Compute COVARIANCE MATRIX: C = (1/n)·X'ᵀ·X'
3. Compute EIGENVALUES (λ) and EIGENVECTORS (v) of C: C·v = λ·v
4. Sort eigenvectors by eigenvalues in DESCENDING order
5. Select top k eigenvectors (principal components) that explain desired variance
6. PROJECT data onto k principal components: Z = X'·Vₖ
```

### Key Concepts
**Eigenvalue (λ):** Represents the AMOUNT OF VARIANCE explained by each principal component. Larger eigenvalue = more important component.

**Eigenvector:** Represents the DIRECTION of the principal component in the original feature space.

**Explained Variance Ratio:**
```
EVRᵢ = λᵢ / Σ(λⱼ)
```
Cumulative EVR tells you how much variance is retained by keeping k components.

### What Do Eigenvalues Represent in PCA?
Eigenvalues represent the amount of variance explained by each principal component. A large eigenvalue means the corresponding eigenvector (principal component direction) captures a large spread/variance in the data. By keeping only eigenvectors with large eigenvalues, we retain most information while reducing dimensions.

### What is the Curse of Dimensionality and How Does PCA Help?
As dimensions increase: data becomes sparse, distance metrics lose meaning, and models require exponentially more data. PCA projects data to lower dimensions while preserving maximum variance, reducing sparsity and computational cost.

---

## 2.13 RECOMMENDATION SYSTEMS

### Types of Recommendation Approaches
| Approach | How It Works | Pros | Cons |
|----------|-------------|------|------|
| **Content-Based Filtering** | Recommends items similar to items the user liked before. Based on item features (genre, keywords, etc.) | No cold-start for new items; interpretable | Limited to user's existing preferences; needs feature engineering |
| **Collaborative Filtering** | Recommends items liked by similar users. Based on user-item interaction matrix (ratings, views) | Discovers unexpected preferences; no item features needed | Cold-start for new users/items; sparsity issues |
| **Hybrid** | Combines both approaches | Best of both worlds | More complex implementation |

### Role of User Similarity in Recommendations
User similarity measures how alike two users are based on their preferences or behavior (e.g., using cosine similarity or Pearson correlation). In collaborative filtering, if two users are highly similar, items liked by one are recommended to the other. It enables personalized recommendations without needing item content details.

### Cosine Similarity for Movie Recommendations
```
cos(θ) = (U₁·U₂) / (‖U₁‖ × ‖U₂‖)

Interpretation:
• Cosine similarity ∈ [-1, 1]; 1 = identical direction
• High similarity (e.g., 0.93) indicates highly similar preferences
• Items that one user rated highly and the other hasn't seen are the best recommendations
```

### ASCII Diagram — Collaborative Filtering
```
User-Item Rating Matrix (? = unknown ratings to predict):

          Item1  Item2  Item3  Item4  Item5
User A:    5      4      ?      1      ?
User B:    4      ?      4      1      2
User C:    ?      3      5      ?      3
User D:    1      1      ?      5      4

Find users similar to User A (by rating overlap)
User B is similar (both rated Item1=4-5, Item4=1)
Predict User A's rating for Item3 based on User B's rating
```

---

## 2.14 EM ALGORITHM (EXPECTATION-MAXIMIZATION)

### Definition
EM is an iterative optimization algorithm used to find maximum likelihood estimates in models with latent (hidden) variables. It alternates between two steps:

### Two Steps (Iterate until convergence)
**E-Step (Expectation):**
Given current parameters, compute the EXPECTED value of the log-likelihood given current parameters. Compute the expected value of the latent variables (i.e., soft assignments — probability each point belongs to each cluster).

**M-Step (Maximization):**
Maximize the expected log-likelihood to update parameters. Given expected latent variables, find parameters that MAXIMIZE the likelihood. Update means, variances, and mixing coefficients.

### EM for Gaussian Mixture Model
```
Init: Random μ₁, μ₂, σ₁, σ₂, π₁, π₂

E-Step: For each point xᵢ, compute:
rᵢₖ = P(cluster k | xᵢ) = [πₖ·𝒩(xᵢ|μₖ,σₖ)] / Σⱼ[πⱼ·𝒩(xᵢ|μⱼ,σⱼ)]
(soft assignment: rᵢₖ = probability xᵢ belongs to cluster k)

M-Step: Update parameters using rᵢₖ (soft assignments):
Nₖ = Σᵢ rᵢₖ
μₖ = (1/Nₖ)·Σᵢ(rᵢₖ·xᵢ)
σₖ = sqrt((1/Nₖ)·Σᵢ rᵢₖ·(xᵢ-μₖ)²)
πₖ = Nₖ / N

Repeat until convergence.
```

**Convergence:** Log-likelihood never decreases; stops when change < ε

### Applications
Used in Gaussian Mixture Models, Hidden Markov Models, clustering with probabilistic assignments.

---

## 📝 UNIT 2 SUMMARY CHEAT SHEET
```
┌─────────────────────────────────────────────────────────┐
│  🔑 KEY FORMULAS - UNIT 2                                │
├─────────────────────────────────────────────────────────┤
│  • Logistic: ŷ = σ(wᵀx) = 1/(1+e⁻ʷᵀˣ)                   │
│  • Log Loss: L = -[y·log(ŷ)+(1-y)·log(1-ŷ)]             │
│  • SVM Margin: 2/‖w‖; Constraint: yᵢ(wᵀxᵢ+b)≥1         │
│  • Entropy: H = -ΣP·log₂P; IG = H(parent)-Σw·H(child)  │
│  • Gini: G = 1-ΣP²                                       │
│  • KNN: c⁽ⁱ⁾ = argminₖ ‖x⁽ⁱ⁾-μₖ‖²                       │
│  • K-Means Objective: J = ΣₖΣ‖x-μₖ‖²                    │
│  • PCA: C = (1/n)X'ᵀX'; C·v = λ·v; EVR = λᵢ/Σλ         │
│  • Cosine Sim: (u·v)/(‖u‖‖v‖)                           │
│  • Precision = TP/(TP+FP); Recall = TP/(TP+FN)          │
│  • F1 = 2·(P·R)/(P+R)                                   │
│  • EM: rᵢₖ = P(k|xᵢ); μₖ = Σrᵢₖxᵢ/Σrᵢₖ                │
├─────────────────────────────────────────────────────────┤
│  🎯 EXAM TIPS                                            │
│  • For Bayes spam: always compute evidence P(B) first   │
│  • K-Means: show at least one full iteration in exams   │
│  • PCA: eigenvalues = variance; sort descending         │
│  • SVM: support vectors define margin; others irrelevant│
│  • Ensemble: Bagging→variance↓; Boosting→bias↓         │
│  • Metrics: choose based on cost of FP vs FN            │
└─────────────────────────────────────────────────────────┘
```

---

# 📘 UNIT 3: PROBABILISTIC METHODS, NEURAL NETWORKS & DEEP LEARNING

---

## 3.1 NAÏVE BAYES ALGORITHM

### Bayes Theorem Foundation
```
                P(B|A) × P(A)
P(A|B) = -----------------------
                     P(B)
```

| Term | Name | Meaning |
|------|------|---------|
| P(A|B) | Posterior | Prob of A given we observe B |
| P(B|A) | Likelihood | Prob of observing B if A is true |
| P(A) | Prior | Initial probability of A |
| P(B) | Evidence | Prob of observing B (normalizer) |

### The "Naive" Assumption
Naive Bayes assumes all features are **CONDITIONALLY INDEPENDENT** given the class label. This is the 'naive' part.
```
P(x₁, x₂, ..., xₙ | C) = P(x₁|C) × P(x₂|C) × ... × P(xₙ|C)
```

### Classification Rule
Predict class C* that maximizes posterior:
```
C* = argmax_C [ P(C) × Πᵢ P(xᵢ | C) ]
```

### Types of Naive Bayes
| Type | Feature Distribution | Use Case |
|------|---------------------|----------|
| **Gaussian** | P(xᵢ|C) ~ 𝒩(μᶜᵢ, σᶜᵢ²) | Continuous features (sensor data) |
| **Multinomial** | P(xᵢ|C) = count-based | Text classification (word frequencies) |
| **Bernoulli** | P(xᵢ|C) = binary (present/absent) | Text with binary features |

### Zero-Frequency Problem and Laplace Smoothing
**Problem:** If a feature value never appears with a class in training data, P(xᵢ|C) = 0, causing the whole probability to be zero.

**Solution: Laplace Smoothing** — adding 1 to all counts:
```
P(xᵢ|C) = (count(xᵢ,C) + 1) / (count(C) + vocabulary_size)
```

### Why is the Assumption Called "Naive"?
It assumes all features are CONDITIONALLY INDEPENDENT given the class. In reality, features often correlate (e.g., words in a sentence are related). This is rarely true, hence the assumption is 'naive'. Despite this, NB works surprisingly well in practice for text classification due to robustness of the voting-like aggregation.

### Naive Bayes for Spam Classification
**Setup:** Given an email with words, compute posterior probabilities for Spam and Not Spam classes.

**Naive Bayes Assumption:** Words are conditionally independent given the class:
```
P(Spam | words) ∝ P(Spam) × P(offer|Spam) × P(free|Spam) × P(money|Spam)
```

**Log-Space Computation (Practical Implementation):**
To avoid numerical underflow with many features:
```
log P(Spam|email) = log P(Spam) + Σ log P(wᵢ|Spam)
```

---

## 3.2 MAXIMUM LIKELIHOOD (MLE) vs MAXIMUM A POSTERIORI (MAP)

### MLE — Maximum Likelihood Estimation
MLE finds the parameters that make the observed data MOST LIKELY. It asks: 'What parameter values would most probably produce the data we observed?'
```
θ_MLE = argmax_θ P(Data | θ)
```
In practice, we maximize log-likelihood (simpler and avoids underflow):
```
θ_MLE = argmax_θ log P(Data | θ)
```

### MAP — Maximum A Posteriori
MAP incorporates PRIOR KNOWLEDGE about parameters. It maximizes the posterior probability of parameters given data:
```
θ_MAP = argmax_θ P(θ | Data) = argmax_θ [P(Data | θ) × P(θ)]
```
MAP = MLE + Prior. When prior is uniform (flat), MAP reduces to MLE.

### Comparison — MLE vs MAP
| Property | MLE | MAP |
|----------|-----|-----|
| Prior | Ignored | Included |
| Overfitting | More prone | Less prone (regularized) |
| Formula | argmax P(D|θ) | argmax P(D|θ)·P(θ) |
| Bayesian? | Frequentist | Bayesian (point estimate) |
| Small data | Can overfit | More robust with prior |

### Key Insight
As data size N → ∞, the influence of the Prior fades, and MAP converges to MLE.

---

## 3.3 BAYESIAN BELIEF NETWORKS (BBN)

### Definition
A Bayesian Belief Network (BBN) is a probabilistic graphical model represented as a Directed Acyclic Graph (DAG). Each node represents a random variable, each edge represents a conditional dependency, and each node has a Conditional Probability Table (CPT).

### Structure — ASCII Diagram
```
Example: Student exam performance network

[Rain] [Traffic]
   \      /
    \    /
     \  /
[Late_to_exam]
      |
      v
[Exam_Performance]

Each node has a CPT:
P(Late | Rain=T, Traffic=T) = 0.9
P(Late | Rain=T, Traffic=F) = 0.7
P(Late | Rain=F, Traffic=T) = 0.6
P(Late | Rain=F, Traffic=F) = 0.1

Joint probability = PRODUCT of all CPTs:
P(A,B,C,D) = P(A)·P(B)·P(C|A,B)·P(D|C)
```

### Properties
- **DAG:** No cycles — ensures consistent probability distributions
- **Markov condition:** Each node is conditionally independent of its non-descendants given its parents
- **Factorization:** Joint distribution factorizes as product of conditional distributions
- **Applications:** Used for diagnosis, prediction, and anomaly detection

### Inference Types in BBNs
1. **Predictive:** Cause → Effect (e.g., Rain → Traffic)
2. **Diagnostic:** Effect → Cause (e.g., Traffic → Rain?)
3. **Intercausal:** Multiple causes affecting one outcome (Explaining Away)

---

## 3.4 PROBABILITY DENSITY ESTIMATION (PDE)

### Purpose
Used for continuous data to show where values are most likely to concentrate.

### Parametric vs Non-Parametric
**Parametric:** Assumes a distribution family (e.g., Gaussian). Task: Estimate μ and σ².

**Non-Parametric:** No assumptions. Kernel Density Estimation (KDE) sums kernels (Gaussian curves) at each point. Controlled by the Bandwidth parameter:
- Too narrow = jagged estimate
- Too wide = oversmoothed estimate

---

## 3.5 SEQUENCE MODELS: MARKOV & HIDDEN MARKOV MODELS

### Markov Property
The future state depends ONLY on the current state, not on the history of past states:
```
P(Xₜ₊₁ | Xₜ, Xₜ₋₁, ..., X₁) = P(Xₜ₊₁ | Xₜ)
```
This is the Markov Assumption — the process is memoryless.

### Standard Markov Model
States are fully observable (e.g., Weather).

### Hidden Markov Models (HMM)
Extends Markov models to systems where underlying states are Hidden (latent). We only see Observations (emissions).

### Components of HMM
1. **Hidden States:** Q = {q₁, q₂, ..., q_N} — not directly observable
2. **Observations:** O = {o₁, o₂, ..., o_T} — what we can see
3. **Initial Distribution:** π = P(q₁) — starting probability for each state
4. **Transition Matrix A:** A[i][j] = P(state j | state i) — probability of moving between hidden states
5. **Emission Matrix B:** B[i][k] = P(observation k | state i) — probability of a hidden state producing an observation

### ASCII Diagram — HMM Unrolled
```
Hidden States:  q₁  →  q₂  →  q₃  →  q₄
                 |      |      |      |
                 ↓      ↓      ↓      ↓
Observations:    o₁     o₂     o₃     o₄

q₁→q₂: Transition probability A[1][2]
q₁→o₁: Emission probability B[1][o₁]
```

### Three Core Problems of HMM
| Problem | Question | Algorithm |
|---------|----------|-----------|
| **Evaluation** | P(Observations | Model) = ? | Forward Algorithm |
| **Decoding** | Best hidden state sequence? | Viterbi Algorithm |
| **Learning** | Best model parameters? | Baum-Welch (EM) |

### Identifying Most Probable State Sequence Using HMM
The **Viterbi Algorithm** is used. Given a sequence of observations, it computes the most probable hidden state sequence by dynamic programming — tracking the maximum probability path through all states at each time step.

### Applications
Speech recognition, NLP POS tagging, DNA sequence analysis, weather prediction.

---

## 3.6 NEURAL NETWORKS: FOUNDATIONS

### Biological Motivation
ANNs are inspired by biological neurons in the human brain. A biological neuron receives inputs through dendrites, processes them in the cell body, and fires an output through the axon if the input exceeds a threshold.

### The Perceptron — Simplest Neural Network
The perceptron is the building block of neural networks. It computes a weighted sum of inputs and passes it through an activation function:
```
y = f(Wᵀ·X + b) = f(w₁·x₁ + w₂·x₂ + ... + wₙ·xₙ + b)
```

### ASCII Diagram — Perceptron
```
Inputs    Weights    Summation    Activation    Output
 x₁ ───► w₁ ──┐
 x₂ ───► w₂ ──┼──► [ Σ wᵢxᵢ + b ] ──► [ f(·) ] ──► y
  ⋮       ⋮   │
 xₙ ───► wₙ ──┘
                ▲
                │
               b (bias)
```

### Role of Bias in a Perceptron
Bias is an additional learnable parameter added to the weighted sum: z = Σ(wᵢxᵢ) + b. It shifts the activation function left or right, allowing the model to fit data that does not pass through the origin. Without bias, the decision boundary is forced through the origin, reducing the model's flexibility.

### Limitation of Perceptron
Can only solve Linearly Separable problems (cannot solve XOR).

### Multi-Layer Perceptron (MLP) / Feed-Forward Network
An MLP has three layers: Input layer, one or more Hidden layers, and Output layer. Each layer is fully connected to the next. Information flows in one direction (no cycles) — hence 'feed-forward'.

### Components of a Feedforward Neural Network
1. **Input Layer** — receives raw features
2. **Hidden Layer(s)** — performs non-linear transformations
3. **Weights and Biases** — learnable parameters
4. **Activation Functions** — introduce non-linearity (ReLU, Sigmoid, etc.)
5. **Output Layer** — produces final prediction
6. **Loss Function** — measures prediction error

### Backpropagation
Backpropagation is the algorithm used to train neural networks. It computes gradients of the loss function with respect to all weights using the CHAIN RULE of calculus, then updates weights using Gradient Descent.

**FORWARD PASS:**
```
Input X → Layer 1 → Layer 2 → ... → Output ŷ
Compute Loss: L = loss_function(ŷ, y_true)
```

**BACKWARD PASS:**
```
Compute dL/dŷ (gradient of loss w.r.t. output)
Propagate BACKWARDS through each layer using Chain Rule:
dL/dWₖ = dL/d(outputₖ) · d(outputₖ)/dWₖ
```

**WEIGHT UPDATE (Gradient Descent):**
```
Wₖ = Wₖ - learning_rate · dL/dWₖ
```
Repeat for all batches, all epochs until convergence.

### What is Vanishing Gradient Problem?
During backpropagation, gradients are multiplied across layers. Sigmoid and Tanh have derivatives < 1. In deep networks, repeated multiplication makes gradients approach 0 — weights in early layers barely update, training stalls.

**Solution:** Use ReLU (derivative is 1 for z > 0), batch normalization, residual connections.

---

## 3.7 ACTIVATION AND LOSS FUNCTIONS

### Activation Functions Comparison
| Function | Formula | Range | Pros | Cons | Best For |
|----------|---------|-------|------|------|----------|
| **Sigmoid** | 1/(1+e⁻ᶻ) | (0,1) | Probabilistic output | Vanishing gradient; not zero-centered | Output layer (binary) |
| **Tanh** | (eᶻ-e⁻ᶻ)/(eᶻ+e⁻ᶻ) | (-1,1) | Zero-centered; stronger gradient | Still vanishes for large |z| | Hidden layers (legacy) |
| **ReLU** | max(0,z) | [0,∞) | No vanishing gradient; sparse; fast | Dying ReLU (z<0 → gradient=0) | Hidden layers (default) |
| **Leaky ReLU** | max(αz, z), α≈0.01 | (-∞,∞) | Fixes dying ReLU | Slightly more complex | Hidden layers (when ReLU fails) |
| **Softmax** | eᶻⁱ/Σⱼeᶻʲ | (0,1), Σ=1 | Multi-class probabilities | Requires careful numerical implementation | Output layer (multi-class) |

### Loss Functions
| Loss | Formula | Use Case |
|------|---------|----------|
| **Mean Squared Error** | (1/n)Σ(y-ŷ)² | Regression problems |
| **Cross-Entropy (Log Loss)** | -[y·log(ŷ)+(1-y)·log(1-ŷ)] | Binary classification |
| **Categorical Cross-Entropy** | -Σ yᵢ·log(ŷᵢ) | Multi-class classification |

### Why is ReLU Preferred Over Sigmoid in Hidden Layers?
1. **No vanishing gradient:** derivative is 1 for positive inputs
2. **Computationally simple:** max(0,z)
3. **Sparse activation:** negative inputs give 0 output (introduces sparsity)
4. **Faster convergence in practice**

**Disadvantage:** Dying ReLU (neurons that always output 0) — fixed by Leaky ReLU.

---

## 3.8 LIMITATIONS OF MACHINE LEARNING

### Critical Challenges
| Limitation | Explanation | Mitigation Strategies |
|------------|-------------|----------------------|
| **Data Dependency** | ML needs large, high-quality, labelled data. Garbage in = garbage out. | Data augmentation, transfer learning, active learning |
| **Manual Feature Engineering** | Traditional ML requires domain experts to manually design and select features, which is time-consuming and may miss important patterns | Deep learning learns features automatically |
| **Poor Performance on High-Dimensional Data** | Traditional ML struggles with unstructured, high-dimensional data like images and audio | Deep learning with CNNs handles this |
| **Overfitting** | Model memorizes training data, fails on new data | Regularization, dropout, cross-validation, early stopping |
| **Underfitting** | Model too simple to capture patterns | More complex model, more features, longer training |
| **Bias & Fairness** | Biased training data leads to biased, unfair predictions | Fairness-aware algorithms, diverse data, bias audits |
| **Interpretability** | Deep models are black boxes — hard to explain predictions | LIME, SHAP, attention visualization, simpler models when possible |
| **Computational Cost** | Deep learning requires expensive GPUs and long training times | Model compression, distillation, efficient architectures |
| **Distribution Shift** | Model trained on one distribution fails when test data distribution differs | Domain adaptation, online learning, robust training |

### Dataset Suffers from Overfitting — Deep Learning or Traditional ML?
Traditional ML would be more suitable in this case. With small datasets prone to overfitting, simpler models with regularization (like SVM or Logistic Regression) generalize better. Deep learning has millions of parameters and requires large datasets — it would overfit even more severely on a small dataset.

---

## 3.9 DEEP LEARNING ARCHITECTURES

### Why Deep Learning is Needed
- Traditional ML requires hand-crafted features — domain expertise needed
- Deep learning learns features automatically from raw data
- Extremely powerful for unstructured data: images, text, audio, video
- With enough data and compute, deep models outperform all traditional ML

### Traditional ML vs Deep Learning Comparison
| Aspect | Traditional ML | Deep Learning |
|--------|---------------|---------------|
| **Features** | Hand-crafted | Learned automatically |
| **Data needed** | Less | Large amounts |
| **Interpretability** | More interpretable | Black box |
| **Compute** | CPU sufficient | GPU/TPU needed |
| **Best for** | Tabular data, small datasets | Images, text, speech |

---

## 3.10 CONVOLUTIONAL NEURAL NETWORKS (CNN)

### Definition
CNNs are deep learning models specialized for grid-structured data like images. They use convolutional layers to automatically learn spatial hierarchies of features (edges → textures → shapes → objects).

### Why CNNs for Images?
```
Key Insights:

1️⃣ Local Connectivity: Pixels near each other are more related
• Neuron connects to small local region (receptive field)
• Not fully connected → fewer parameters

2️⃣ Weight Sharing: Same filter detects feature anywhere in image
• Translation invariance: pattern same whether top-left or bottom-right
• Dramatically reduces parameters vs fully connected

3️⃣ Hierarchical Features:
Layer 1: Edges, corners → Layer 2: Textures → Layer 3: Parts → Layer 4: Objects
```

### CNN Architecture Components
```
1. CONVOLUTIONAL LAYER:
• Apply learnable filters (kernels) across input
• Each filter detects specific pattern (edge, blob, etc.)
• Output: Feature maps (activation maps)

2. ACTIVATION (ReLU):
• Apply element-wise: f(x) = max(0, x)
• Introduces non-linearity; enables complex function learning

3. POOLING LAYER:
• Downsample feature maps (reduce spatial dimensions)
• Max Pooling: Take max in window → preserves strongest features
• Benefits: Reduces computation; provides translation invariance

4. FULLY CONNECTED LAYERS:
• After flattening feature maps, standard dense layers
• Final classification/regression

5. SOFTMAX (for classification):
• Convert final outputs to class probabilities
```

### Output Size Formula
```
Output_Size = (Input_Size - Filter_Size + 2×Padding) / Stride + 1
```

### Role of Pooling Layer in CNN
Pooling reduces the spatial dimensions (height and width) of feature maps.

**Benefits:**
1. Reduces number of parameters and computation
2. Controls overfitting
3. Provides translation invariance (small shifts in input don't change output drastically)

**Max Pooling:** keeps maximum value in region (preserves strongest feature)
**Average Pooling:** keeps average value in region

### How CNN Differs from Regular (Fully Connected) Neural Network
1. **CNN uses LOCAL connectivity** — each neuron connects to small local region. MLP uses GLOBAL connectivity — each neuron connects to all previous neurons.
2. **CNN uses WEIGHT SHARING** — same filter applied across entire image. MLP has unique weights per connection.
3. **CNN exploits spatial structure.** MLP ignores spatial structure.

**Result:** CNN has far fewer parameters, less overfitting, works better on images.

---

## 3.11 RECURRENT NEURAL NETWORKS (RNN)

### Definition
RNNs are neural networks designed for sequential data (text, speech, time series). Unlike feedforward networks, RNNs have connections that loop back, giving them MEMORY of previous inputs.

### RNN Hidden State Equation
```
hₜ = f(W·xₜ + U·hₜ₋₁ + b)

where:
• hₜ = hidden state at time t (memory at time t)
• xₜ = current input
• hₜ₋₁ = previous hidden state (memory from past)
• W, U = learned weight matrices (shared across all time steps)
• f = activation function (usually tanh)

This equation encodes current input + past memory into a new state.
```

### ASCII Diagram — RNN Unrolled
```
Folded RNN:          Unrolled RNN (through time):

   xₜ → [ RNN ] → yₜ            x₁ → [h₁] → y₁
        ↑  │                          ↑   │
        └──┘                          │   │
        hₜ                           x₂ → [h₂] → y₂
                                      ↑   │
                                      │   │
                                    x₃ → [h₃] → y₃
```

### Limitations of Basic RNN
- **Vanishing Gradient:** Gradients diminish exponentially during backpropagation through time (BPTT), making it hard to learn long-range dependencies
- **Exploding Gradient:** Gradients can grow exponentially — fixed by gradient clipping
- **Short memory:** Basic RNN forgets information from many steps ago

### LSTM and GRU — Solutions
**Long Short-Term Memory (LSTM)** uses gating mechanisms (input gate, forget gate, output gate) to selectively remember and forget information. This solves the vanishing gradient problem for long sequences.

**Gated Recurrent Unit (GRU)** is a simplified version of LSTM with fewer gates (reset gate, update gate) — faster to train, similar performance.

### Distinguishing CNN and RNN
| CNN | RNN |
|-----|-----|
| Designed for spatial data (images) | Designed for sequential data (text, speech) |
| Uses convolutional filters | Uses recurrent connections with memory |
| Captures local spatial patterns | Captures temporal dependencies |
| Fixed input size | Variable length sequences |

### Difference Between RNN and Feedforward Network
**Feedforward:** No memory. Each input processed independently. No temporal connections.

**RNN:** Has recurrent connections. Hidden state hₜ carries information from previous time steps. Processes sequences by maintaining state over time.

RNN is like a feedforward network with shared weights unrolled through time.

---

## 🎯 FINAL EXAM MASTER CHEAT SHEET
```
┌─────────────────────────────────────────────────────────┐
│  📊 ALL UNITS: KEY FORMULAS AT A GLANCE                 │
├─────────────────────────────────────────────────────────┤
│  UNIT 1: Foundations                                    │
│  • Bayes: P(A|B) = P(B|A)P(A)/P(B)                     │
│  • Evidence: P(B) = P(B|A)P(A) + P(B|¬A)P(¬A)          │
│  • Entropy: H = -ΣP·log₂P; IG = H(parent)-Σw·H(child) │
│  • Gradient Descent: w ← w - α∇L(w)                    │
│  • Eigenvalue: Av = λv; det(A-λI)=0                    │
│  • Euclidean: d = √Σ(xᵢ-yᵢ)²                           │
├─────────────────────────────────────────────────────────┤
│  UNIT 2: Supervised/Unsupervised                        │
│  • Logistic: ŷ = σ(wᵀx); Log Loss = -[y·logŷ+...]     │
│  • SVM: Min (1/2)‖w‖² s.t. yᵢ(wᵀxᵢ+b)≥1; Margin=2/‖w‖│
│  • KNN: c⁽ⁱ⁾ = argminₖ ‖x⁽ⁱ⁾-μₖ‖²                      │
│  • K-Means: J = ΣₖΣ‖x-μₖ‖²; μₖ = mean(Cₖ)             │
│  • PCA: C = (1/n)X'ᵀX'; EVR = λᵢ/Σλ                    │
│  • Metrics: Prec=TP/(TP+FP); Rec=TP/(TP+FN); F1=2PR/(P+R)│
├─────────────────────────────────────────────────────────┤
│  UNIT 3: Probabilistic & Deep Learning                  │
│  • Naive Bayes: C* = argmax [log P(C) + Σlog P(xᵢ|C)] │
│  • MLE: θ* = argmax Σlog P(x|θ); MAP adds log P(θ)    │
│  • HMM: αₜ₊₁(j) = [Σᵢαₜ(i)Aᵢⱼ]·Bⱼ(oₜ₊₁)              │
│  • Perceptron: z = wᵀx+b; y = f(z)                     │
│  • CNN Output: (W-F+2P)/S + 1                          │
│  • RNN: hₜ = f(Wxₜ + Uhₜ₋₁ + b)                        │
│  • ReLU: f(z) = max(0,z); Sigmoid: σ(z)=1/(1+e⁻ᶻ)     │
├─────────────────────────────────────────────────────────┤
│  🎯 100/100 EXAM STRATEGY                               │
│  1️⃣ Part A (2-mark): Direct definitions, formulas      │
│     → memorize cheat sheet                              │
│  2️⃣ Part B (16-mark): Use framework:                   │
│     • Define → Explain → Example → Diagram → Limitation│
│  3️⃣ Diagrams: Draw ASCII only when asked or critical   │
│  4️⃣ Time Mgmt: Part A: 30 min; Part B: 60 min         │
│  5️⃣ Verify: Check eigenvalues (Trace=Σλ), Bayes denom │
└─────────────────────────────────────────────────────────┘
```

---

## 🏆 FINAL TIPS FOR 100/100

```
✅ BEFORE EXAM:
• Memorize the Cheat Sheet formulas (1 page per unit)
• Review all theoretical concepts with their definitions
• Practice explaining algorithms step-by-step without calculations

✅ DURING EXAM:
• Part A: Answer in 2-3 lines; include formula if applicable
• Part B: Use framework: Definition → Explanation → Example → Diagram → Limitation
• Show conceptual understanding → partial credit → centum secured!
• Time: Spend max 3 min on Part A questions; 15 min on Part B

✅ COMMON PITFALLS TO AVOID:
• Forgetting to compute P(B) in Bayes problems
• Confusing precision/recall formulas
• Not checking eigenvalue properties (Trace, Det)
• Mixing up generative vs discriminative model characteristics

✅ LAST-MINUTE REVISION (1 hour before):
1. Bayes theorem components and evidence calculation
2. Entropy/Information Gain conceptual meaning
3. K-Means algorithm steps and objective
4. PCA eigenvalue interpretation
5. Backpropagation chain rule intuition
6. CNN vs RNN architectural differences
7. RNN vanishing gradient + LSTM solution

🎯 YOU'VE GOT THIS!
This guide covers 100% theoretical content from all provided materials.
Focus on understanding frameworks and conceptual relationships.
Show your understanding → centum secured! ✨
```

---

*End of Machine Learning Techniques (23CSC02) Ultimate Theoretical Centum Study Guide*
*Total Content: Comprehensive coverage of all concepts from provided materials*
*Target: 100/100 | Pure Theoretical Focus | Last Updated: April 2026*
*Sri Krishna College of Technology | B.E. CSE(AIML) | Semester 4*

> "Understanding the why behind the how is the key to mastering Machine Learning." 🤖📚✨
