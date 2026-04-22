# 🎯 MACHINE LEARNING TECHNIQUES (23CSC02)
## 📚 THE ULTIMATE CENTUM STUDY GUIDE (100/100)
### Sri Krishna College of Technology | B.E. CSE(AIML) | Semester 4

---

```
╔════════════════════════════════════════════════════════════════════════╗
║  📋 GUIDE STRUCTURE                                                     ║
║  ─────────────────────────────────────────────────────────────────    ║
║  ✅ Module 1: Introduction & Mathematical Foundations (Pages 1-18)     ║
║  ✅ Module 2: Supervised & Unsupervised Learning (Pages 19-40)         ║
║  ✅ Module 3: Probabilistic Methods & Deep Learning (Pages 41-60+)     ║
║                                                                        ║
║  🎯 FEATURES:                                                          ║
║  • All CIA1 + CIA2 + Assignment questions integrated as examples       ║
║  • Step-by-step numerical solutions with working                       ║
║  • ASCII diagrams for visual concepts (only where essential)           ║
║  • Formula sheets, cheat codes, and exam tips                          ║
║  • RBT levels & CO mappings for targeted preparation                   ║
╚════════════════════════════════════════════════════════════════════════╝
```

---

# 📘 MODULE 1: INTRODUCTION AND MATHEMATICAL FOUNDATIONS
## (Pages 1-18)

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

### Applications of Machine Learning (CIA1-QP Q1)

**Q: List two real-world applications of Machine Learning.**

**Answer:**

1. **Healthcare - Disease Prediction**
   - ML models analyze patient records, lab results, and imaging data
   - Predict disease risk (diabetes, cancer, heart disease) before symptoms appear
   - Example: Random Forest classifier using 100+ patient features for ICU admission risk prediction

2. **E-commerce - Recommendation Systems**
   - Collaborative filtering suggests products based on similar users' behavior
   - Content-based filtering recommends items similar to previously liked products
   - Example: Amazon's "Customers who bought this also bought..." increases sales by 35%

**Additional High-Impact Applications:**
- 🚗 Autonomous Vehicles: CNNs for object detection, RNNs for trajectory prediction
- 💬 Natural Language Processing: Transformers for translation, sentiment analysis
- 🔐 Cybersecurity: Anomaly detection for intrusion prevention
- 🎵 Entertainment: Netflix/Spotify personalization using matrix factorization

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
| **Regression** | Continuous value | House price prediction | Linear Regression, SVR |
| **Classification** | Categorical label | Spam detection | Logistic Regression, SVM, Decision Trees |

**CIA1-QP Integration:**
> **Q: A company predicts sales based on past data trends. Which ML task is being performed?**
> 
> **Answer:** This is a **Regression** task under Supervised Learning because:
> - Sales is a continuous numerical value (not discrete categories)
> - Historical data with actual sales figures serves as labeled training data
> - The model learns the function: Sales = f(Marketing Spend, Season, Economic Indicators...)

### Unsupervised Learning

**Concept:** Model learns from **unlabeled data** to discover hidden structures or patterns.

**Types:**

| Type | Goal | Example | Algorithm |
|------|------|---------|-----------|
| **Clustering** | Group similar items | Customer segmentation | K-Means, Hierarchical |
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

### Matrix Multiplication: Four Perspectives (Critical for Exams!)

Given matrices A (m×p) and B (p×n), product C = AB (m×n):

**1. Dot Product (Row-Column) View:**
```
C[i,j] = Row_i(A) • Column_j(B) = Σₖ A[i,k] × B[k,j]
```

**2. Column View (Linear Combination):**
```
Each column of C is a linear combination of columns of A
C[:,j] = Σₖ B[k,j] × A[:,k]
```

**3. Row View:**
```
Each row of C is a linear combination of rows of B
C[i,:] = Σₖ A[i,k] × B[k,:]
```

**4. Outer Product View:**
```
AB = Σₖ (Column_k of A) × (Row_k of B)
Each term is a rank-1 matrix
```

### Worked Example: Column Perspective Multiplication (CIA2 Assignment)

> **Q: A neuron receives weights W and input x. Compute Wx using column perspective.**
> ```
>         [ 0.5  -0.3 ]
>     W = [ 0.2   0.8 ]    ,    x = [ 2 ]
>         [-0.1   0.4 ]                    [-1 ]
> ```

**Step-by-Step Solution (Column Method):**

```
Step 1: Identify columns of W
    Col₁ = [ 0.5 ]    Col₂ = [-0.3 ]
           [ 0.2 ]             [ 0.8 ]
           [-0.1 ]             [ 0.4 ]

Step 2: Multiply each input element by corresponding column
    Wx = x₁ × Col₁ + x₂ × Col₂
       = 2 × [ 0.5 ]  +  (-1) × [-0.3 ]
             [ 0.2 ]            [ 0.8 ]
             [-0.1 ]            [ 0.4 ]

Step 3: Compute scalar-vector products
       = [ 1.0 ]  +  [ 0.3 ]
         [ 0.4 ]     [-0.8 ]
         [-0.2 ]     [-0.4 ]

Step 4: Add vectors component-wise
       = [ 1.0 + 0.3 ]   = [ 1.3 ]
         [ 0.4 - 0.8 ]     [-0.4 ]
         [-0.2 - 0.4 ]     [-0.6 ]

✅ Final Answer: Wx = [1.3, -0.4, -0.6]ᵀ
```

**Geometric Interpretation:** The output is a linear combination of weight column vectors, scaled by input values. This is the fundamental operation in neural network layers.

### Norms and Distance Metrics

| Norm | Formula | Name | Use Case |
|------|---------|------|----------|
| **L₁ Norm** | ‖x‖₁ = Σ\|xᵢ\| | Manhattan | Sparse solutions, Lasso |
| **L₂ Norm** | ‖x‖₂ = √(Σxᵢ²) | Euclidean | Least squares, Ridge |
| **L∞ Norm** | ‖x‖∞ = max\|xᵢ\| | Chebyshev | Worst-case analysis |

**Distance Between Vectors:**
```
Euclidean: d(x,y) = ‖x - y‖₂ = √Σ(xᵢ - yᵢ)²
Manhattan: d(x,y) = ‖x - y‖₁ = Σ|xᵢ - yᵢ|
```

### CIA1-QP Numerical: Euclidean Distance

> **Q: Compute the Euclidean distance between two data points A(2,3) and B(5,7).**

**Solution:**
```
Given: A = (2, 3), B = (5, 7)

Formula: d(A,B) = √[(x₂-x₁)² + (y₂-y₁)²]

Step 1: Compute differences
    Δx = 5 - 2 = 3
    Δy = 7 - 3 = 4

Step 2: Square and sum
    (Δx)² + (Δy)² = 3² + 4² = 9 + 16 = 25

Step 3: Take square root
    d = √25 = 5

✅ Answer: Euclidean distance = 5 units
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

**CIA1-MLT Worked Example:**
> **Q: Given vectors x=(2,-1,3) and y=(1,4,-2): (a) Find dot product. (b) Are they orthogonal?**

**Solution:**
```
(a) Dot Product:
    ⟨x,y⟩ = (2)(1) + (-1)(4) + (3)(-2)
          = 2 - 4 - 6 = -8

(b) Orthogonality Check:
    Since ⟨x,y⟩ = -8 ≠ 0, vectors are NOT orthogonal.
    Angle θ = cos⁻¹(⟨x,y⟩/(‖x‖‖y‖)) = cos⁻¹(-8/(√14·√21)) ≈ 126.9°
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

**Key Properties (Exam Gold!):**
```
• Trace(A) = Σλᵢ  (sum of diagonal = sum of eigenvalues)
• det(A) = Πλᵢ   (determinant = product of eigenvalues)
• If A is singular → at least one λ = 0
• Symmetric matrices have real eigenvalues & orthogonal eigenvectors
```

### Worked Example: 2×2 Eigenvalues (CIA1-MLT)

> **Q: Find eigenvalues and eigenvectors of A = [[2,1],[1,2]]**

**Solution:**
```
Step 1: Characteristic Equation
    det(A - λI) = det([2-λ,  1  ], [ 1,  2-λ]) = 0
                = (2-λ)(2-λ) - (1)(1) = 0
                = λ² - 4λ + 3 = 0
                = (λ-3)(λ-1) = 0
    
    Eigenvalues: λ₁ = 3, λ₂ = 1

Step 2: Verify with Properties
    Trace(A) = 2+2 = 4; Σλ = 3+1 = 4 ✓
    det(A) = 4-1 = 3; Πλ = 3×1 = 3 ✓

Step 3: Find Eigenvectors
    For λ₁ = 3:
        (A - 3I)v = 0 → [[-1,1],[1,-1]]v = 0
        → -v₁ + v₂ = 0 → v₁ = v₂
        Eigenvector: v₁ = [1, 1]ᵀ (or any scalar multiple)
    
    For λ₂ = 1:
        (A - 1I)v = 0 → [[1,1],[1,1]]v = 0
        → v₁ + v₂ = 0 → v₁ = -v₂
        Eigenvector: v₂ = [1, -1]ᵀ

✅ Answer: 
    λ₁=3 with v₁=[1,1]ᵀ; λ₂=1 with v₂=[1,-1]ᵀ
```

### Matrix Centering and Covariance (PCA Preprocessing)

**CIA1-MLT Worked Example:**
> **Q: Given data matrix X = [[1,2],[2,3],[3,4]]: (a) Find mean vector. (b) Center the data.**

**Solution:**
```
(a) Mean Vector:
    μ₁ = (1+2+3)/3 = 2  (mean of column 1)
    μ₂ = (2+3+4)/3 = 3  (mean of column 2)
    μ = [2, 3]

(b) Centered Matrix (X' = X - μ):
    Row 1: [1-2, 2-3] = [-1, -1]
    Row 2: [2-2, 3-3] = [ 0,  0]
    Row 3: [3-2, 4-3] = [ 1,  1]
    
    X' = [[-1, -1],
          [ 0,  0],
          [ 1,  1]]

Note: Centered data has zero mean per feature — essential for PCA.
```

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
| P(A\|B) | **Posterior** | Updated belief about A after observing B |
| P(B\|A) | **Likelihood** | Probability of evidence B if hypothesis A is true |
| P(A) | **Prior** | Initial belief about A before seeing evidence |
| P(B) | **Evidence** | Normalizing constant: total probability of B |

### CIA1-QP: Bayes' Theorem Statement & Application

> **Q: State Bayes' theorem.**
> **Q: In a dataset, 40% of emails are spam. If an email contains a keyword with 70% probability in spam and 10% in non-spam, calculate P(Spam|Keyword).**

**Complete Solution:**
```
Given:
    P(Spam) = 0.40          (Prior)
    P(NotSpam) = 0.60
    P(Keyword|Spam) = 0.70  (Likelihood)
    P(Keyword|NotSpam) = 0.10

Step 1: Compute Evidence P(Keyword) using Law of Total Probability
    P(Keyword) = P(Keyword|Spam)×P(Spam) + P(Keyword|NotSpam)×P(NotSpam)
               = (0.70)(0.40) + (0.10)(0.60)
               = 0.28 + 0.06 = 0.34

Step 2: Apply Bayes' Theorem
                    P(Keyword|Spam) × P(Spam)
    P(Spam|Keyword) = -------------------------
                           P(Keyword)
                    
                    = (0.70 × 0.40) / 0.34
                    = 0.28 / 0.34 = 0.8235

✅ Answer: P(Spam|Keyword) ≈ 82.35%
```

**Interpretation:** Even though only 40% of emails are spam initially, observing the keyword increases the probability to 82% — demonstrating how evidence updates beliefs.

### CIA2-QP: Medical Test Bayes Problem

> **Q: A medical test predicts a disease with 99% sensitivity but 5% false positive rate. Using Bayes theorem, explain how to calculate the probability that a patient has the disease given a positive test.**

**Framework Solution (General Case):**
```
Define Events:
    D = Patient has disease
    + = Test is positive

Given (Typical Values):
    P(D) = prevalence (e.g., 0.01 for rare disease)
    Sensitivity = P(+|D) = 0.99
    False Positive Rate = P(+|¬D) = 0.05

Bayes Calculation:
                    P(+|D) × P(D)
    P(D|+) = ---------------------------------
             P(+|D)×P(D) + P(+|¬D)×P(¬D)

Example with P(D)=0.01:
    Numerator = 0.99 × 0.01 = 0.0099
    Denominator = (0.99×0.01) + (0.05×0.99) = 0.0099 + 0.0495 = 0.0594
    P(D|+) = 0.0099 / 0.0594 ≈ 0.1667 = 16.67%

⚠️ Key Insight: Even with 99% accurate test, low prevalence means 
   most positive results are FALSE POSITIVES (Base Rate Fallacy).
```

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

**ASCII Diagram: Gradient Descent Landscape**
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

### CIA1-MLT: Gradient Descent Step Calculation

> **Q: Loss L(w) = (w-3)². Find gradient. Do 1 step with α=0.1 starting from w=0.**

**Solution:**
```
Step 1: Compute Gradient
    L(w) = (w-3)²
    ∇L = dL/dw = 2(w-3)  [Chain rule]

Step 2: Evaluate at w=0
    ∇L|w=0 = 2(0-3) = -6

Step 3: Apply Update Rule
    w_new = w_old - α·∇L
          = 0 - (0.1)(-6)
          = 0 + 0.6 = 0.6

Step 4: Verify Loss Reduction
    L(0) = (0-3)² = 9
    L(0.6) = (0.6-3)² = (-2.4)² = 5.76 < 9 ✓

✅ Answer: After 1 step, w = 0.6; loss decreased from 9 to 5.76
```

### Why Square the Error in MSE? (Exam Favorite!)

**Q: Why do we use squared error instead of absolute error in Linear Regression?**

**Three Critical Reasons:**

```
1️⃣ Avoids Cancellation
   • Errors can be positive or negative
   • Sum of absolute errors: +5 and -5 cancel to 0 (misleading)
   • Squared errors: 25 + 25 = 50 (properly penalizes both)

2️⃣ Penalizes Large Errors Heavily
   • Error of 2 → penalty = 4
   • Error of 4 → penalty = 16 (4× larger, not 2×)
   • Forces model to care about outliers (useful or problematic)

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
Example: "Solar eclipse tomorrow" carries more info than "Sun rises tomorrow"
```

**Entropy H(X): Average Uncertainty**
```
H(X) = -Σ P(x)·log₂(P(x))

Properties:
• H = 0 → perfectly predictable (one outcome certain)
• H = max → maximum uncertainty (uniform distribution)
• Measured in bits (log base 2)
```

### Worked Example: Entropy Calculation (CIA2 Assignment)

> **Q: Calculate entropy for dataset with classes: Yes=9, No=5 (total=14)**

**Solution:**
```
Step 1: Compute probabilities
    P(Yes) = 9/14 ≈ 0.6429
    P(No)  = 5/14 ≈ 0.3571

Step 2: Apply entropy formula
    H = -[P(Yes)·log₂(P(Yes)) + P(No)·log₂(P(No))]
    
    log₂(0.6429) ≈ -0.637
    log₂(0.3571) ≈ -1.485
    
    H = -[(0.6429)(-0.637) + (0.3571)(-1.485)]
      = -[-0.409 - 0.530]
      = 0.939 bits

✅ Answer: Entropy ≈ 0.94 bits (high uncertainty, good for splitting)
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

### CIA2 Assignment: Decision Tree Root Selection

> **Q: Calculate, based on information gain, which feature is chosen as root node for classifying the following data:**
> ```
> Weather | Temp | Humidity | Wind | Play?
> Sunny   | Hot  | High     | Weak | No
> Cloudy  | Hot  | High     | Weak | Yes
> Sunny   | Mild | Normal   | Strong| Yes
> ... (10 instances total)
> ```

**Step-by-Step Solution Framework:**
```
Step 1: Compute Parent Entropy H(S)
    Count Play=Yes: 6, Play=No: 4 (example)
    H(S) = -[(6/10)log₂(6/10) + (4/10)log₂(4/10)] = 0.971 bits

Step 2: For EACH attribute, compute weighted child entropy:

    Example for "Wind" (values: Weak, Strong):
    
    Wind=Weak (6 instances): Yes=4, No=2
        H(Weak) = -[(4/6)log₂(4/6) + (2/6)log₂(2/6)] = 0.918
    
    Wind=Strong (4 instances): Yes=2, No=2  
        H(Strong) = -[(2/4)log₂(2/4) + (2/4)log₂(2/4)] = 1.000
    
    Weighted Avg = (6/10)(0.918) + (4/10)(1.000) = 0.951

Step 3: Compute Information Gain for Wind
    IG(Wind) = H(S) - WeightedAvg = 0.971 - 0.951 = 0.020

Step 4: Repeat for Weather, Temp, Humidity
    Suppose results:
        IG(Weather) = 0.247 ← HIGHEST
        IG(Temp) = 0.029
        IG(Humidity) = 0.152
        IG(Wind) = 0.020

✅ Answer: "Weather" chosen as root node (maximum information gain)
```

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

### CIA1-MLT: Risk Calculation Example

> **Q: Loss matrix: Accept(Pos:0, Neg:5), Reject(Pos:10, Neg:0). P(Pos)=0.6. Find optimal decision.**

**Solution:**
```
Given:
    P(Pos) = 0.6, P(Neg) = 0.4
    Loss(Accept, Pos) = 0, Loss(Accept, Neg) = 5
    Loss(Reject, Pos) = 10, Loss(Reject, Neg) = 0

Expected Risk(Accept):
    = Loss(Accept,Pos)×P(Pos) + Loss(Accept,Neg)×P(Neg)
    = (0)(0.6) + (5)(0.4) = 0 + 2 = 2.0

Expected Risk(Reject):
    = Loss(Reject,Pos)×P(Pos) + Loss(Reject,Neg)×P(Neg)
    = (10)(0.6) + (0)(0.4) = 6 + 0 = 6.0

Decision: Since 2.0 < 6.0, choose ACCEPT.

✅ Answer: Optimal decision = Accept (minimizes expected loss)
```

---

## 📝 MODULE 1 SUMMARY CHEAT SHEET

```
┌─────────────────────────────────────────────────────────┐
│  🔑 KEY FORMULAS - MODULE 1                              │
├─────────────────────────────────────────────────────────┤
│  • Euclidean Distance: d = √Σ(xᵢ-yᵢ)²                    │
│  • Dot Product: ⟨x,y⟩ = Σxᵢyᵢ = ‖x‖‖y‖cosθ              │
│  • Bayes: P(A|B) = P(B|A)P(A)/P(B)                      │
│  • Entropy: H(X) = -ΣP(x)log₂P(x)                       │
│  • Info Gain: IG = H(parent) - Σ(|Sᵥ|/|S|)H(Sᵥ)         │
│  • Gradient Descent: w ← w - α∇L(w)                     │
│  • Eigenvalue: Av = λv → det(A-λI)=0                    │
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

# 📘 MODULE 2: SUPERVISED AND UNSUPERVISED LEARNING
## (Pages 19-40)

---

## 2.1 DISCRIMINATIVE vs GENERATIVE MODELS

### Fundamental Distinction

| Aspect | Discriminative Models | Generative Models |
|--------|---------------------|-------------------|
| **Learns** | P(Y\|X) directly | P(X,Y) = P(X\|Y)P(Y) |
| **Focus** | Decision boundary | Data distribution |
| **Question** | "Which class is this?" | "What does each class look like?" |
| **Can Generate** | ❌ No | ✅ Yes (synthetic data) |
| **Examples** | Logistic Regression, SVM, Decision Trees, Neural Nets | Naive Bayes, HMM, GANs, LLMs |

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

Why 1/2? Simplifies derivative: d/dw (1/2)z² = z
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

### CIA1-QP: Normal Equation Limitations

> **Q: If the dataset is linearly dependent, explain its effect on solving for weights using the normal equation.**

**Answer:**
```
Linear Dependence → XᵀX is SINGULAR (non-invertible)

Causes:
• Perfect multicollinearity: One feature = linear combo of others
• More features than samples: n > m
• Redundant features: "Size_sqft" and "Size_sqm" both included

Consequences:
• (XᵀX)⁻¹ does not exist → Normal equation fails
• Infinite solutions: Many w give same minimum loss

Solutions:
1️⃣ Remove redundant features (feature selection)
2️⃣ Use Regularization: Ridge adds λI to make XᵀX+λI invertible
3️⃣ Use Gradient Descent (doesn't require matrix inverse)
4️⃣ Apply PCA to reduce to independent components
```

### Worked Example: Simple Linear Regression (CIA1-QP)

> **Q: Fit a simple linear regression model to predict house price given size. Data: Size(sqft): [1200,1500,1700,2000,2200], Price(lakh): [30,34,38,44,48]. Predict price for 1800 sqft.**

**Solution:**
```
Step 1: Prepare Data
    x = [1200, 1500, 1700, 2000, 2200]
    y = [30, 34, 38, 44, 48]
    n = 5

Step 2: Compute Means
    x̄ = (1200+1500+1700+2000+2200)/5 = 8600/5 = 1720
    ȳ = (30+34+38+44+48)/5 = 194/5 = 38.8

Step 3: Compute Slope w₁
    w₁ = Σ(xᵢ-x̄)(yᵢ-ȳ) / Σ(xᵢ-x̄)²
    
    Numerator:
      (1200-1720)(30-38.8) = (-520)(-8.8) = 4576
      (1500-1720)(34-38.8) = (-220)(-4.8) = 1056
      (1700-1720)(38-38.8) = (-20)(-0.8) = 16
      (2000-1720)(44-38.8) = (280)(5.2) = 1456
      (2200-1720)(48-38.8) = (480)(9.2) = 4416
      Σ = 4576+1056+16+1456+4416 = 11520
    
    Denominator:
      (-520)² + (-220)² + (-20)² + (280)² + (480)²
      = 270400 + 48400 + 400 + 78400 + 230400 = 628000
    
    w₁ = 11520 / 628000 ≈ 0.01834

Step 4: Compute Intercept w₀
    w₀ = ȳ - w₁x̄ = 38.8 - (0.01834)(1720) = 38.8 - 31.55 = 7.25

Step 5: Final Model
    Price = 7.25 + 0.01834 × Size

Step 6: Predict for 1800 sqft
    Price = 7.25 + 0.01834(1800) = 7.25 + 33.01 = 40.26 lakh

✅ Answer: Predicted price for 1800 sqft ≈ ₹40.26 lakh
```

---

## 2.3 UNDERFITTING, OVERFITTING & REGULARIZATION

### The Bias-Variance Tradeoff

```
Total Error = Bias² + Variance + Irreducible Error

┌─────────────────────────────────────────┐
│  Underfitting (High Bias)               │
│  • Model too simple                     │
│  • Misses patterns in data              │
│  • Poor train AND test performance      │
│  • Fix: More complex model, more features│
├─────────────────────────────────────────┤
│  Overfitting (High Variance)            │
│  • Model too complex                    │
│  • Memorizes training noise             │
│  • Great train, poor test performance   │
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
| **Lasso (L1)** | λΣ\|wⱼ\| | Sets some coefficients EXACTLY to 0 | Feature selection, sparse models |

**CIA1-QP: Lasso Application**
> **Q: A health analytics company wants to predict disease risk using 100 patient features, but many features are irrelevant. Explain how Lasso Regression can be applied.**

**Answer:**
```
Why Lasso is Ideal:
1️⃣ Automatic Feature Selection
   • L1 penalty forces irrelevant feature weights to exactly 0
   • Model becomes sparse: only important features retained
   • Example: From 100 features, Lasso might keep only 15 non-zero weights

2️⃣ Handles Multicollinearity
   • When features correlate (e.g., BMI and weight), Lasso picks one
   • Avoids unstable coefficient estimates

3️⃣ Improves Interpretability
   • Clinicians can focus on selected features
   • Easier to validate medically

Implementation Steps:
1. Standardize features (Lasso sensitive to scale)
2. Choose λ via cross-validation (larger λ = more features zeroed)
3. Train: minimize MSE + λΣ|wⱼ|
4. Extract non-zero coefficients as selected features

⚠️ Caution: If features highly correlated, Lasso arbitrarily picks one.
   Consider Elastic Net (L1+L2) for grouped selection.
```

---

## 2.4 CROSS-VALIDATION

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

### CIA1-QP: Cross-Validation Interpretation

> **Q: Given a dataset, you perform 5-fold cross-validation and get slightly different errors in each fold. What does this indicate?**

**Answer:**
```
Slightly different errors across folds is EXPECTED and HEALTHY:

✅ What it indicates:
• Data has natural variability (not all samples identical)
• Model performance is stable (small variance across folds)
• No severe overfitting to specific data subsets

📊 Interpreting Fold Variance:
• Low variance (e.g., 0.82, 0.84, 0.83, 0.85, 0.83): Model robust
• High variance (e.g., 0.95, 0.70, 0.88, 0.65, 0.92): Model unstable

⚠️ If errors differ GREATLY:
• Possible data leakage in some folds
• Class imbalance not stratified
• Small dataset → high sampling variance

🔧 Best Practice: Use Stratified K-Fold for classification
   to maintain class distribution in each fold.
```

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

### CIA1-QP: Logistic Regression for Loan Default

> **Q: A bank wants to predict whether a customer will default on a loan. How can Logistic Regression be applied? Explain with probability outputs and decision thresholds.**

**Complete Framework:**
```
Step 1: Feature Engineering
    X = [Credit_Score, Income, Loan_Amount, Employment_Years, ...]
    y = 1 if default, 0 otherwise

Step 2: Model Training
    • Standardize features (logistic regression sensitive to scale)
    • Train: minimize log loss using gradient descent
    • Output: weights w and bias b

Step 3: Probability Prediction
    For new customer x_new:
        z = wᵀx_new + b
        P(default) = σ(z) = 1/(1+e⁻ᶻ)
    
    Example: If σ(z) = 0.73 → 73% probability of default

Step 4: Decision Threshold Selection
    Default threshold = 0.5, but bank can adjust:
    
    Conservative (low risk tolerance):
        Threshold = 0.3 → Flag if P(default) ≥ 30%
        ↑ Recall (catch more defaults), ↓ Precision (more false alarms)
    
    Aggressive (high approval rate goal):
        Threshold = 0.8 → Flag only if P(default) ≥ 80%  
        ↑ Precision (fewer false rejections), ↓ Recall (miss some defaults)

Step 5: Business Integration
    • High-risk customers: Require collateral, higher interest
    • Medium-risk: Manual review
    • Low-risk: Auto-approve

✅ Key Advantage: Probabilistic output enables risk-based decisions,
   not just binary approve/reject.
```

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

### Kernel Trick: Handling Non-Linear Data

**Problem:** Data not linearly separable in original space.

**Solution:** Map to higher dimension where separation is possible.

```
Original Space (2D)          High-D Space (3D)
      o  x                          o
   x     o   ← Not separable    x     o  ← Separable by plane
      o  x                          x

Kernel Function K(x,z) = φ(x)ᵀφ(z)
• Computes dot product in high-D space WITHOUT explicit mapping φ
• Computational shortcut: "Kernel Trick"
```

### Common Kernels

| Kernel | Formula | When to Use |
|--------|---------|-------------|
| **Linear** | K(x,z) = xᵀz | Linearly separable data |
| **Polynomial** | K(x,z) = (xᵀz + c)ᵈ | Feature interactions matter |
| **RBF (Gaussian)** | K(x,z) = exp(-γ‖x-z‖²) | Most versatile; default choice |
| **Sigmoid** | K(x,z) = tanh(αxᵀz + c) | Neural network similarity |

### CIA2-QP: SVM by Hand (1D Example)

> **Q: Given 2 points in 1D: x=1 (class +1), x=-1 (class -1). Find decision boundary and margin.**

**Solution:**
```
Given:
    Point A: x=1, y=+1
    Point B: x=-1, y=-1

Decision boundary: w·x + b = 0

Constraints (for support vectors):
    For A: w(1) + b = +1  →  w + b = 1   ...(1)
    For B: w(-1) + b = -1 → -w + b = -1  ...(2)

Solve system:
    Add (1) and (2): (w+b) + (-w+b) = 1 + (-1)
                     2b = 0 → b = 0
    Substitute b=0 in (1): w + 0 = 1 → w = 1

Decision Boundary:
    1·x + 0 = 0 → x = 0 (hyperplane at origin)

Margin Calculation:
    Margin = 2 / ‖w‖ = 2 / |1| = 2

Support Vectors: Both points (x=1 and x=-1) lie exactly on margin boundaries.

✅ Answer: 
    • Boundary: x = 0
    • Margin: 2 units
    • Support Vectors: x=1 and x=-1
```

---

## 2.7 INSTANCE-BASED LEARNING: K-NEAREST NEIGHBORS (KNN)

### Algorithm Overview

```
KNN is LAZY LEARNING: No explicit training phase!

Prediction for query point q:
1. Compute distance from q to ALL training points
2. Select K nearest neighbors
3. Classification: Majority vote of neighbors' labels
4. Regression: Average of neighbors' values
```

### Distance Metrics

| Metric | Formula | Properties |
|--------|---------|------------|
| **Euclidean** | d = √Σ(xᵢ-yᵢ)² | Most common; sensitive to scale |
| **Manhattan** | d = Σ\|xᵢ-yᵢ\| | Robust to outliers; grid-like paths |
| **Minkowski** | d = (Σ\|xᵢ-yᵢ\|ᵖ)¹/ᵖ | Generalizes both (p=1: Manhattan, p=2: Euclidean) |

### CIA1-QP: Cosine Similarity for Recommendations

> **Q: A recommendation system represents two users' movie preferences as vectors: U₁=[3,0,5,2], U₂=[4,1,5,0]. Calculate cosine similarity. Analyze whether users have similar preferences.**

**Solution:**
```
Cosine Similarity Formula:
    sim(U₁,U₂) = (U₁·U₂) / (‖U₁‖ ‖U₂‖)

Step 1: Compute Dot Product
    U₁·U₂ = (3)(4) + (0)(1) + (5)(5) + (2)(0)
          = 12 + 0 + 25 + 0 = 37

Step 2: Compute Norms
    ‖U₁‖ = √(3² + 0² + 5² + 2²) = √(9+0+25+4) = √38 ≈ 6.164
    ‖U₂‖ = √(4² + 1² + 5² + 0²) = √(16+1+25+0) = √42 ≈ 6.481

Step 3: Compute Similarity
    sim = 37 / (6.164 × 6.481) = 37 / 39.95 ≈ 0.926

Interpretation:
    • Cosine similarity ∈ [-1, 1]; 1 = identical direction
    • 0.926 = VERY HIGH similarity
    • Users likely have similar movie taste

✅ Answer: Cosine similarity ≈ 0.926 → Users have highly similar preferences.
```

### Worked Example: KNN Classification (CIA2-MLT)

> **Q: Training data (2D, binary class): P1(1,2)=A, P2(2,3)=A, P3(5,5)=B, P4(6,4)=B. Query Q=(3,3), K=2. Predict class.**

**Solution:**
```
Step 1: Compute Euclidean Distances from Q(3,3)
    d(Q,P1) = √[(3-1)² + (3-2)²] = √(4+1) = √5 ≈ 2.24
    d(Q,P2) = √[(3-2)² + (3-3)²] = √(1+0) = 1.00 ← Nearest
    d(Q,P3) = √[(3-5)² + (3-5)²] = √(4+4) = √8 ≈ 2.83
    d(Q,P4) = √[(3-6)² + (3-4)²] = √(9+1) = √10 ≈ 3.16

Step 2: Select K=2 Nearest
    1st: P2 (distance 1.00, Class A)
    2nd: P1 (distance 2.24, Class A)

Step 3: Majority Vote
    Class A: 2 votes, Class B: 0 votes
    → Prediction: Class A

✅ Answer: Query point Q=(3,3) classified as Class A.
```

### Effect of K Value

```
┌─────────────────────────────────────────┐
│  K = 1                                  │
│  • Very sensitive to noise/outliers     │
│  • Complex, jagged decision boundary    │
│  • High variance → Overfitting risk     │
├─────────────────────────────────────────┤
│  K = Optimal (found via CV)             │
│  • Smooth boundary, good generalization │
│  • Balance bias-variance tradeoff       │
├─────────────────────────────────────────┤
│  K = N (all training points)            │
│  • Always predicts majority class       │
│  • High bias → Underfitting             │
└─────────────────────────────────────────┘
```

---

## 2.8 TREE-BASED METHODS: DECISION TREES

### ID3 Algorithm: Entropy & Information Gain

**Entropy (Impurity Measure):**
```
H(S) = -Σ P(c)·log₂P(c)
• H=0: Pure node (all same class)
• H=1: Maximum impurity (binary, 50-50 split)
```

**Information Gain (Split Quality):**
```
IG(S, A) = H(S) - Σᵥ (|Sᵥ|/|S|)·H(Sᵥ)

ID3 selects attribute with MAXIMUM IG as splitting criterion.
```

### CART Algorithm: Gini Index

**Gini Impurity:**
```
Gini(S) = 1 - Σ P(c)²
• Gini=0: Pure node
• Gini=0.5: Maximum impurity (binary, 50-50)
```

**Gini Gain for Split:**
```
Gini_split = (|S_L|/|S|)·Gini(S_L) + (|S_R|/|S|)·Gini(S_R)

CART selects split that MINIMIZES Gini_split.
```

### ID3 vs CART Comparison

| Feature | ID3 | CART |
|---------|-----|------|
| **Split Criterion** | Information Gain (Entropy) | Gini Index |
| **Tree Structure** | Multi-way splits | Binary splits only |
| **Task Support** | Classification only | Classification + Regression |
| **Missing Values** | Not handled natively | Handled via surrogate splits |
| **Pruning** | No built-in pruning | Cost-complexity pruning |

### CIA2 Assignment: Entropy & IG Calculation

> **Q: Calculate entropy for dataset with Yes=9, No=5. Then compute IG for "Wind" attribute: Weak(6: Yes=4,No=2), Strong(4: Yes=2,No=2).**

**Complete Solution:**
```
Step 1: Parent Entropy H(S)
    P(Yes)=9/14≈0.643, P(No)=5/14≈0.357
    H(S) = -[0.643·log₂(0.643) + 0.357·log₂(0.357)]
         = -[0.643·(-0.637) + 0.357·(-1.485)]
         = 0.409 + 0.530 = 0.939 bits

Step 2: Child Entropies for "Wind"
    Wind=Weak (6 samples: 4Y,2N):
        H(Weak) = -[(4/6)log₂(4/6) + (2/6)log₂(2/6)]
                = -[0.667·(-0.585) + 0.333·(-1.585)]
                = 0.390 + 0.528 = 0.918 bits
    
    Wind=Strong (4 samples: 2Y,2N):
        H(Strong) = -[(2/4)log₂(2/4) + (2/4)log₂(2/4)]
                  = -[0.5·(-1) + 0.5·(-1)] = 1.000 bits

Step 3: Weighted Average Child Entropy
    Weighted_H = (6/14)·0.918 + (4/14)·1.000
               = 0.393 + 0.286 = 0.679 bits

Step 4: Information Gain
    IG(Wind) = H(S) - Weighted_H = 0.939 - 0.679 = 0.260 bits

✅ Answer: IG(Wind) = 0.260 bits
```

### ASCII Diagram: Decision Tree Structure

```
[ROOT: Outlook?]
       /     |     \
   Sunny  Overcast  Rainy
     |       |        |
[Humidity?] [Play=Yes] [Wind?]
   /   \              /    \
High  Normal      Strong  Weak
 |       |          |       |
[No]  [Yes]      [No]    [Yes]
```

---

## 2.9 ENSEMBLE METHODS

### Bagging vs Boosting: Core Distinction

```
┌─────────────────────────────────────────┐
│  BAGGING (Bootstrap Aggregating)        │
│  • Parallel training of base learners   │
│  • Each trained on random bootstrap sample │
│  • Final prediction: majority vote/average │
│  • REDUCES VARIANCE (overfitting)       │
│  • Example: Random Forest               │
├─────────────────────────────────────────┤
│  BOOSTING                               │
│  • Sequential training                  │
│  • Each model focuses on previous errors │
│  • Misclassified samples get higher weight │
│  • Final prediction: weighted sum       │
│  • REDUCES BIAS (underfitting)          │
│  • Examples: AdaBoost, Gradient Boost, XGBoost │
└─────────────────────────────────────────┘
```

### Random Forest: Why Better Than Single Tree?

```
Random Forest = Bagging + Feature Randomness

Key Innovations:
1️⃣ Bootstrap Sampling
   • Each tree trained on different random subset (with replacement)
   • Creates diversity among trees

2️⃣ Feature Randomness at Each Split
   • Instead of considering all features, randomly select √m features
   • Decorrelates trees (prevents all trees making same errors)

3️⃣ Majority Voting
   • Individual tree errors cancel out
   • Robust to noise and outliers

Result: Lower variance, better generalization, less overfitting
```

### CIA2-MLT: Ensemble Methods Exam Question

> **Q: Why does Random Forest perform better than a single Decision Tree?**

**Model Answer (16-mark framework):**
```
1. VARIANCE REDUCTION THROUGH AVERAGING
   • Single tree: High variance (small data change → different tree)
   • Random Forest: Average predictions of many trees
   • Law of Large Numbers: Variance of average = σ²/n
   • Result: More stable predictions, less overfitting

2. DECORRELATION VIA FEATURE RANDOMNESS
   • Problem: If one strong feature exists, all trees split on it first
   • Solution: At each node, consider only random subset of features
   • Effect: Trees explore different feature combinations
   • Trees become diverse → errors uncorrelated → cancel out

3. ROBUSTNESS TO NOISE AND OUTLIERS
   • Single tree: Outliers can create deep, specific branches
   • Random Forest: Outliers affect only trees that sampled them
   • Bootstrap sampling: ~37% of data not in each sample (out-of-bag)
   • OOB error provides unbiased performance estimate

4. HANDLING HIGH-DIMENSIONAL DATA
   • Feature randomness acts as implicit feature selection
   • Reduces curse of dimensionality impact
   • Works well when p >> n (many features, few samples)

5. PRACTICAL ADVANTAGES
   • Little hyperparameter tuning needed
   • Provides feature importance scores
   • Handles missing values and mixed data types
   • Less prone to overfitting than individual trees

⚠️ Trade-offs:
   • Less interpretable than single tree
   • Slower prediction (must evaluate all trees)
   • Requires more memory

✅ Conclusion: Random Forest achieves better bias-variance tradeoff
   through ensemble diversity, making it consistently superior to
   single decision trees in practice.
```

---

## 2.10 EVALUATION OF CLASSIFICATION MODELS

### Confusion Matrix Fundamentals

```
                    PREDICTED
                 Positive   Negative
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
| **Recall** | TP/(TP+FN) | Cost of FN high (cancer screening, security) |
| **F1-Score** | 2·(Prec·Rec)/(Prec+Rec) | Imbalanced classes, need balance |
| **Specificity** | TN/(TN+FP) | When true negatives matter (healthy diagnosis) |

### CIA2-MLT: Metrics Calculation Example

> **Q: Confusion matrix for spam detection: TP=50, FN=10, FP=5, TN=85. Calculate all metrics.**

**Solution:**
```
Given:
    TP=50, FN=10, FP=5, TN=85
    Total = 50+10+5+85 = 150

1. Accuracy:
   = (TP+TN)/Total = (50+85)/150 = 135/150 = 0.90 = 90%

2. Precision:
   = TP/(TP+FP) = 50/(50+5) = 50/55 ≈ 0.909 = 90.9%
   Interpretation: When model says "spam", 90.9% chance it's correct

3. Recall (Sensitivity):
   = TP/(TP+FN) = 50/(50+10) = 50/60 ≈ 0.833 = 83.3%
   Interpretation: Model catches 83.3% of actual spam emails

4. F1-Score:
   = 2·(Precision·Recall)/(Precision+Recall)
   = 2·(0.909·0.833)/(0.909+0.833)
   = 2·(0.757)/(1.742) = 1.514/1.742 ≈ 0.869 = 86.9%

5. Specificity:
   = TN/(TN+FP) = 85/(85+5) = 85/90 ≈ 0.944 = 94.4%
   Interpretation: 94.4% of non-spam correctly identified

✅ Summary: High precision (few false alarms), moderate recall (misses some spam).
   For spam filtering, high precision is often preferred (users hate false alarms).
```

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

### K-Means: Algorithm & Objective

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

### CIA2 Assignment: K-Means by Hand

> **Q: Perform K-means clustering on dataset. Use first and last datapoints as initial centers (K=2). Data: [0,1,5,4,9,17], [1,0,2,5,10,20], [5,2,0,12,20,34], [4,5,12,0,1,5], [9,10,20,1,0,2], [17,20,34,5,2,0]**

**Note:** This appears to be a distance matrix. Let's reinterpret as 6 points in some space, with given pairwise distances. For K-means, we need coordinates. Assuming the matrix represents 6 points with indices 1-6, and we're given distances.

*Since the data format is ambiguous, here's the general K-means workflow for exam:*

```
Given: Points with coordinates, K=2, initial centroids = point 1 and point 6

Step 1: Initialization
    μ₁⁽⁰⁾ = point 1 coordinates
    μ₂⁽⁰⁾ = point 6 coordinates

Step 2: Iteration 1 - Assignment
    For each point i:
        d₁ = distance(point i, μ₁⁽⁰⁾)
        d₂ = distance(point i, μ₂⁽⁰⁾)
        Assign to cluster with smaller distance

Step 3: Iteration 1 - Update
    μ₁⁽¹⁾ = mean of points assigned to cluster 1
    μ₂⁽¹⁾ = mean of points assigned to cluster 2

Step 4: Check Convergence
    If centroids changed significantly, repeat Steps 2-3
    Else, stop and return clusters

✅ Exam Tip: Show at least one full iteration with distance calculations.
```

### Hierarchical Clustering: Agglomerative Approach

```
Bottom-Up Process:
1. Start: Each point is its own cluster (N clusters)
2. Repeat until one cluster remains:
   a. Find two closest clusters (using linkage criterion)
   b. Merge them into one cluster
3. Result: Dendrogram (tree of merges)

Linkage Criteria:
• Single: min distance between any two points in clusters
• Complete: max distance between any two points  
• Average: average distance between all point pairs
• Ward: minimize increase in within-cluster variance (most popular)
```

### Cluster Validity: Elbow Method & Silhouette

**Elbow Method:**
```
1. Run K-means for K = 1, 2, 3, ..., K_max
2. Plot inertia J(K) vs K
3. Look for "elbow" point where J stops decreasing rapidly
4. That K is optimal

ASCII Diagram:
Inertia J
  ^
  |*
  | *
  |  *
  |   * ← ELBOW (optimal K)
  |    * * * *
  +----------------> K
```

**Silhouette Score:**
```
For each point i:
    a(i) = avg distance to points in SAME cluster
    b(i) = avg distance to points in NEAREST other cluster
    s(i) = (b(i) - a(i)) / max(a(i), b(i))

Interpretation:
• s(i) ≈ 1: Well-clustered
• s(i) ≈ 0: On cluster boundary  
• s(i) ≈ -1: Probably in wrong cluster

Overall silhouette = mean of all s(i)
```

---

## 2.12 DIMENSIONALITY REDUCTION: PRINCIPAL COMPONENT ANALYSIS (PCA)

### Why Reduce Dimensions?

```
✅ Benefits:
• Combat curse of dimensionality (data becomes sparse in high-D)
• Reduce computational cost and storage
• Remove noise and redundant features
• Enable visualization (project to 2D/3D)
• Improve model performance (less overfitting)

⚠️ Trade-off: Some information loss (irreducible)
```

### PCA Algorithm: Step-by-Step

```
1. MEAN CENTER: X' = X - mean(X)  [per feature]
2. COVARIANCE MATRIX: C = (1/n) X'ᵀX'
3. EIGENDECOMPOSITION: Find eigenvalues λ and eigenvectors v of C
   Solve: C·v = λ·v
4. SORT: Order eigenvectors by eigenvalues (descending)
5. SELECT: Choose top k eigenvectors (principal components)
6. PROJECT: Z = X' · Vₖ  [k-dimensional representation]
```

### Key Insight: Eigenvalues = Variance Explained

```
Explained Variance Ratio for PC i:
    EVRᵢ = λᵢ / Σⱼ λⱼ

Cumulative EVR: Σᵢ₌₁ᵏ EVRᵢ = fraction of total variance retained

Rule of Thumb: Choose k such that cumulative EVR ≥ 95%
```

### CIA1-MLT: PCA Worked Example (2D→1D)

> **Q: Data: x1=[2,3,4,5,6], x2=[1,4,3,6,5]. Perform PCA to reduce to 1D.**

**Solution:**
```
Step 1: Mean Center
    μ₁ = (2+3+4+5+6)/5 = 4
    μ₂ = (1+4+3+6+5)/5 = 3.8
    
    x1' = [-2, -1, 0, 1, 2]
    x2' = [-2.8, 0.2, -0.8, 2.2, 1.2]

Step 2: Covariance Matrix
    Var(x1') = [(-2)²+(-1)²+0²+1²+2²]/5 = 10/5 = 2.0
    Var(x2') = [(-2.8)²+0.2²+(-0.8)²+2.2²+1.2²]/5 = 16/5 = 3.2
    Cov(x1',x2') = [(-2)(-2.8)+(-1)(0.2)+0+1(2.2)+2(1.2)]/5 = 10/5 = 2.0
    
    C = [[2.0, 2.0],
         [2.0, 3.2]]

Step 3: Eigenvalues
    det(C - λI) = (2-λ)(3.2-λ) - 4 = λ² - 5.2λ + 2.4 = 0
    λ = [5.2 ± √(27.04-9.6)]/2 = [5.2 ± √17.44]/2
    λ₁ ≈ 4.67, λ₂ ≈ 0.51

Step 4: Explained Variance
    Total variance = 4.67 + 0.51 = 5.18
    EVR₁ = 4.67/5.18 ≈ 90.1%
    EVR₂ = 0.51/5.18 ≈ 9.9%

Step 5: Decision
    PC1 alone explains 90.1% of variance → sufficient for 1D projection

✅ Answer: First principal component captures 90.1% of information.
   Project data onto eigenvector corresponding to λ₁=4.67.
```

---

## 2.13 RECOMMENDATION SYSTEMS

### Two Main Approaches

| Approach | How It Works | Pros | Cons |
|----------|-------------|------|------|
| **Content-Based** | Recommend items similar to what user liked (based on item features) | No cold-start for new items; interpretable | Limited to user's existing preferences; needs feature engineering |
| **Collaborative Filtering** | Recommend items liked by similar users (based on user-item interactions) | Discovers unexpected preferences; no item features needed | Cold-start for new users/items; sparsity issues |

### Collaborative Filtering: User-User Similarity

```
User-Item Rating Matrix:
        Item1  Item2  Item3  Item4
UserA:    5      4      ?      1
UserB:    4      ?      4      1  
UserC:    ?      3      5      ?

Step 1: Find users similar to UserA
    • Compute similarity (cosine/Pearson) using overlapping ratings
    • UserB similar to A: both rated Item1=4-5, Item4=1

Step 2: Predict UserA's rating for Item3
    • Use UserB's rating for Item3 (which is 4)
    • Weighted average if multiple similar users

Step 3: Recommend top-N unrated items with highest predicted ratings
```

### EM Algorithm for Clustering (Gaussian Mixture Models)

**Why EM?** K-Means does hard assignments; EM does SOFT assignments (probabilistic).

**Two Steps (Iterate until convergence):**

```
E-Step (Expectation):
    Given current parameters (μₖ, σₖ, πₖ), compute responsibility:
    rᵢₖ = P(cluster k | xᵢ) = [πₖ·𝒩(xᵢ|μₖ,σₖ)] / Σⱼ[πⱼ·𝒩(xᵢ|μⱼ,σⱼ)]
    • rᵢₖ = probability that point i belongs to cluster k

M-Step (Maximization):
    Given responsibilities rᵢₖ, update parameters:
    Nₖ = Σᵢ rᵢₖ  (effective number of points in cluster k)
    μₖ = (1/Nₖ) Σᵢ rᵢₖ·xᵢ  (weighted mean)
    σₖ² = (1/Nₖ) Σᵢ rᵢₖ·‖xᵢ-μₖ‖²  (weighted variance)
    πₖ = Nₖ / N  (mixing coefficient)

Convergence: Log-likelihood never decreases; stops when change < ε
```

---

## 📝 MODULE 2 SUMMARY CHEAT SHEET

```
┌─────────────────────────────────────────────────────────┐
│  🔑 KEY FORMULAS - MODULE 2                              │
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

# 📘 MODULE 3: PROBABILISTIC METHODS, NEURAL NETWORKS & DEEP LEARNING
## (Pages 41-60+)

---

## 3.1 NAIVE BAYES CLASSIFIER

### Bayes Theorem Refresher
```
                    P(B|A) × P(A)
    P(A|B) = -----------------------
                      P(B)
```

### The "Naive" Assumption
```
P(x₁,x₂,...,xₙ | C) = P(x₁|C) × P(x₂|C) × ... × P(xₙ|C)

• Assumes features are CONDITIONALLY INDEPENDENT given class C
• Rarely true in reality (words in text correlate, etc.)
• Yet works surprisingly well → "Naive Bayes Paradox"
```

### Classification Rule
```
Predict class C* that maximizes posterior:
    C* = argmax_C [ P(C) × Πᵢ P(xᵢ | C) ]

In practice, use log to avoid underflow:
    C* = argmax_C [ log P(C) + Σᵢ log P(xᵢ | C) ]
```

### Types of Naive Bayes

| Type | Feature Distribution | Use Case |
|------|---------------------|----------|
| **Gaussian** | P(xᵢ|C) ~ 𝒩(μᶜᵢ, σᶜᵢ²) | Continuous features (sensor data) |
| **Multinomial** | P(xᵢ|C) = count-based | Text classification (word counts) |
| **Bernoulli** | P(xᵢ|C) = binary (present/absent) | Text with binary features |

### Zero-Frequency Problem & Laplace Smoothing

**Problem:** If feature value never appears with class in training → P(xᵢ|C)=0 → entire product zero.

**Solution: Laplace (Add-1) Smoothing**
```
P(xᵢ|C) = (count(xᵢ,C) + 1) / (count(C) + V)

where V = vocabulary size (number of possible feature values)
```

### CIA2-QP: Naive Bayes Spam Detection

> **Q: In spam detection, 20% of emails are spam. Word "offer" appears in 70% of spam and 10% of non-spam. Calculate P(Spam|"offer").**

**Solution:**
```
Given:
    P(Spam) = 0.20          (Prior)
    P(Ham) = 0.80
    P("offer"|Spam) = 0.70  (Likelihood)
    P("offer"|Ham) = 0.10

Step 1: Compute Evidence P("offer")
    P("offer") = P("offer"|Spam)P(Spam) + P("offer"|Ham)P(Ham)
               = (0.70)(0.20) + (0.10)(0.80)
               = 0.14 + 0.08 = 0.22

Step 2: Apply Bayes Theorem
                    P("offer"|Spam) × P(Spam)
    P(Spam|"offer") = -------------------------
                           P("offer")
                    
                    = (0.70 × 0.20) / 0.22
                    = 0.14 / 0.22 ≈ 0.6364

✅ Answer: P(Spam|"offer") ≈ 63.64%

Interpretation: Observing "offer" increases spam probability from 20% to 64%.
```

---

## 3.2 MAXIMUM LIKELIHOOD (MLE) vs MAXIMUM A POSTERIORI (MAP)

### MLE: Frequentist Approach
```
Goal: Find parameters θ that make observed data MOST LIKELY

θ_MLE = argmax_θ P(Data | θ)

In practice, maximize log-likelihood (numerically stable):
θ_MLE = argmax_θ log P(Data | θ)

Example (Coin Flip):
    Data: 7 heads, 3 tails
    Likelihood: L(p) = p⁷(1-p)³
    Log-L: log L = 7 log p + 3 log(1-p)
    Derivative: 7/p - 3/(1-p) = 0 → p = 0.7
    θ_MLE = 0.7 (matches observed frequency)
```

### MAP: Bayesian Approach with Prior
```
Goal: Find parameters θ that maximize POSTERIOR probability

θ_MAP = argmax_θ P(θ | Data) 
      = argmax_θ [P(Data | θ) × P(θ)]   (Bayes rule, ignore P(Data))

Key Difference: Includes PRIOR P(θ) encoding prior beliefs

Example (Coin Flip with Prior):
    Prior: P(p) ~ Beta(2,2) (believes coin is fair)
    Likelihood: p⁷(1-p)³
    Posterior ∝ p⁷(1-p)³ × p¹(1-p)¹ = p⁸(1-p)⁴
    Mode of Beta(9,5): p = (9-1)/(9+5-2) = 8/12 = 0.667
    θ_MAP = 0.667 (shrunk toward prior mean 0.5)
```

### MLE vs MAP Comparison

| Aspect | MLE | MAP |
|--------|-----|-----|
| **Philosophy** | Frequentist | Bayesian |
| **Uses Prior** | ❌ No | ✅ Yes |
| **Overfitting** | More prone (no regularization) | Less prone (prior acts as regularizer) |
| **Formula** | argmax P(D\|θ) | argmax P(D\|θ)P(θ) |
| **When Data Scarce** | Unreliable estimates | Prior stabilizes estimates |
| **Special Case** | - | Uniform prior → MAP = MLE |

### CIA2-QP: MLE vs MAP Comparison

> **Q: Compare Maximum Likelihood Estimation with Maximum A Posteriori estimation in terms of prior knowledge usage.**

**Model Answer:**
```
1. PRIOR KNOWLEDGE INTEGRATION
   • MLE: Ignores prior knowledge; relies solely on observed data
   • MAP: Explicitly incorporates prior belief P(θ) via Bayes theorem
   • Example: Medical diagnosis with rare disease → MAP uses prevalence as prior

2. MATHEMATICAL FORMULATION
   • MLE: θ* = argmax_θ ∏ᵢ P(x⁽ⁱ⁾|θ) = argmax_θ Σᵢ log P(x⁽ⁱ⁾|θ)
   • MAP: θ* = argmax_θ [∏ᵢ P(x⁽ⁱ⁾|θ)] × P(θ) 
                = argmax_θ [Σᵢ log P(x⁽ⁱ⁾|θ) + log P(θ)]
   • Note: log P(θ) acts as REGULARIZATION TERM

3. BEHAVIOR WITH LIMITED DATA
   • MLE: Estimates can be extreme/unreliable (e.g., p=1.0 if all heads)
   • MAP: Prior pulls estimate toward reasonable values
   • Example: 1 head in 1 flip → MLE: p=1.0; MAP with Beta(2,2): p≈0.6

4. EQUIVALENCE TO REGULARIZATION
   • Gaussian prior P(θ) ~ 𝒩(0,σ²) → MAP ≡ L2 Regularization (Ridge)
   • Laplace prior P(θ) ~ Laplace(0,b) → MAP ≡ L1 Regularization (Lasso)
   • Thus MAP provides Bayesian justification for regularization

5. COMPUTATIONAL ASPECTS
   • MLE: Often has closed-form solution (e.g., linear regression)
   • MAP: May require numerical optimization if prior is complex
   • Both use same optimization machinery (gradient descent, etc.)

✅ Conclusion: MAP extends MLE by incorporating prior knowledge, 
   providing more robust estimates especially with limited data, 
   and offering Bayesian interpretation of regularization.
```

---

## 3.3 BAYESIAN BELIEF NETWORKS (BBN)

### Structure: Directed Acyclic Graph (DAG)

```
Example: Student Performance Network

    [Difficulty]     [Intelligence]
          \             /
           \           /
            \         /
          [Grade] ← [Study_Hours]
                \
                 \
               [Job_Offer]

• Nodes = Random variables
• Edges = Direct causal/conditional dependencies
• No cycles (DAG property ensures consistent probabilities)
```

### Conditional Probability Tables (CPTs)

**Each node has a CPT specifying P(Node | Parents)**

```
Example CPT for Grade (parents: Difficulty, Intelligence):

Difficulty  Intelligence  P(Grade=A)  P(Grade=B)  P(Grade=C)
Easy        High          0.90        0.08        0.02
Easy        Low           0.50        0.30        0.20
Hard        High          0.40        0.40        0.20
Hard        Low           0.10        0.30        0.60

Joint Probability Factorization:
P(D,I,G,S,J) = P(D)·P(I)·P(G|D,I)·P(S|I)·P(J|G)
```

### Inference in BBNs

**Goal:** Compute posterior P(Query | Evidence)

**Methods:**
```
1. Exact Inference:
   • Variable Elimination: Sum out non-query, non-evidence variables
   • Complexity: Exponential in treewidth of graph

2. Approximate Inference:
   • Monte Carlo Sampling (MCMC, Gibbs)
   • Variational Inference: Optimize simpler distribution

3. Special Cases:
   • Naive Bayes: Simple closed-form posterior
   • Hidden Markov Models: Forward-Backward algorithm
```

---

## 3.4 SEQUENCE MODELS: MARKOV & HIDDEN MARKOV MODELS

### Markov Property
```
P(Xₜ₊₁ | Xₜ, Xₜ₋₁, ..., X₁) = P(Xₜ₊₁ | Xₜ)

"The future depends only on the present, not the past"
• Memoryless property
• Foundation for Markov Chains, HMMs, MDPs
```

### Hidden Markov Model (HMM) Components

```
1. Hidden States: Q = {q₁, q₂, ..., q_N} (not directly observable)
2. Observations: O = {o₁, o₂, ..., o_T} (what we see)
3. Initial Distribution: πᵢ = P(q₁ = i)
4. Transition Matrix: A[i][j] = P(qₜ₊₁=j | qₜ=i)
5. Emission Matrix: B[i][k] = P(oₜ=k | qₜ=i)
```

### ASCII Diagram: HMM Unrolled

```
Hidden States:  q₁  →  q₂  →  q₃  →  ...  →  qₜ
                 |      |      |           |
                 ↓      ↓      ↓           ↓
Observations:   o₁     o₂     o₃    ...    oₜ

• Horizontal arrows: Transition probabilities A
• Vertical arrows: Emission probabilities B
```

### Three Fundamental HMM Problems

| Problem | Question | Algorithm |
|---------|----------|-----------|
| **Evaluation** | P(Observations \| Model) = ? | Forward Algorithm |
| **Decoding** | Most likely state sequence given observations? | Viterbi Algorithm |
| **Learning** | Best model parameters given observations? | Baum-Welch (EM) |

### CIA2 Assignment: HMM Probability Calculation

> **Q: What is the probability of your friend being happy, happy, sad for three consecutive days given weather as sunny, cloudy, sunny? Use given transition/emission probabilities.**

**Given (reconstructed from assignment):**
```
States: Weather = {Rainy, Cloudy, Sunny}
Observations: Mood = {Sad, Happy}

Initial: π = [Rainy:0.218, Cloudy:0.273, Sunny:0.509]

Transition Matrix A (rows→current, cols→next):
          Rainy  Cloudy  Sunny
Rainy     0.5     0.3     0.2
Cloudy    0.4     0.2     0.4  
Sunny     0.0     0.3     0.7

Emission Matrix B (rows→state, cols→observation):
          Sad   Happy
Rainy    0.9    0.1
Cloudy   0.6    0.4
Sunny    0.2    0.8

Observation Sequence: O = [Happy, Happy, Sad]
Weather Sequence (given): W = [Sunny, Cloudy, Sunny]
```

**Solution: Probability of Observations Given States**
```
Since weather sequence is GIVEN (not hidden), this is simpler:

P(O|W) = P(Happy|Sunny) × P(Happy|Cloudy) × P(Sad|Sunny)
       = B[Sunny,Happy] × B[Cloudy,Happy] × B[Sunny,Sad]
       = 0.8 × 0.4 × 0.2
       = 0.064

✅ Answer: P(Observations | Given Weather) = 0.064 = 6.4%

⚠️ Note: If weather were HIDDEN, we'd use Forward Algorithm:
   α₁(i) = πᵢ·Bᵢ(o₁)
   αₜ₊₁(j) = [Σᵢ αₜ(i)·Aᵢⱼ] · Bⱼ(oₜ₊₁)
   P(O) = Σᵢ αₜ(i)
```

---

## 3.5 NEURAL NETWORKS: FOUNDATIONS

### Biological Inspiration → Artificial Perceptron

```
Biological Neuron:
    Dendrites (inputs) → Cell Body (process) → Axon (output if threshold exceeded)

Artificial Perceptron:
    Inputs x₁,x₂,...,xₙ → Weighted Sum → Activation → Output

Mathematical Form:
    z = w₁x₁ + w₂x₂ + ... + wₙxₙ + b = wᵀx + b
    y = f(z)  where f = activation function
```

### ASCII Diagram: Perceptron

```
Inputs      Weights      Summation    Activation    Output
  x₁ ──────► w₁ ──┐
  x₂ ──────► w₂ ──┼──► [ Σ wᵢxᵢ + b ] ──► [ f(·) ] ──► y
   ⋮          ⋮   │
  xₙ ──────► wₙ ──┘
                ▲
                │
               b (bias)
```

### Multi-Layer Perceptron (MLP) / Feed-Forward Network

```
Architecture:
    INPUT LAYER → HIDDEN LAYER(S) → OUTPUT LAYER
    
    • Fully connected: Each neuron connects to all in next layer
    • Feed-forward: No cycles; information flows one direction
    • Universal Approximator: Sufficient hidden units can approximate any function

Forward Pass Computation:
    Layer 1: z⁽¹⁾ = W⁽¹⁾x + b⁽¹⁾; a⁽¹⁾ = f(z⁽¹⁾)
    Layer 2: z⁽²⁾ = W⁽²⁾a⁽¹⁾ + b⁽²⁾; a⁽²⁾ = f(z⁽²⁾)
    ...
    Output: ŷ = a⁽ᴸ⁾
```

### Backpropagation: Training Neural Networks

**Core Idea:** Use chain rule to compute gradients of loss w.r.t. all weights.

```
Algorithm:
1. FORWARD PASS: Compute predictions ŷ and loss L(ŷ, y)
2. BACKWARD PASS: 
   a. Output layer: δ⁽ᴸ⁾ = ∇ₐL ⊙ f'(z⁽ᴸ⁾)
   b. Hidden layers (l = L-1 to 1): 
        δ⁽ˡ⁾ = (W⁽ˡ⁺¹⁾ᵀ δ⁽ˡ⁺¹⁾) ⊙ f'(z⁽ˡ⁾)
   c. Gradients: ∂L/∂W⁽ˡ⁾ = δ⁽ˡ⁾ (a⁽ˡ⁻¹⁾)ᵀ; ∂L/∂b⁽ˡ⁾ = δ⁽ˡ⁾
3. UPDATE: W⁽ˡ⁾ ← W⁽ˡ⁾ - α·∂L/∂W⁽ˡ⁾ (Gradient Descent)

where ⊙ = element-wise multiplication (Hadamard product)
```

### Activation Functions Comparison

| Function | Formula | Range | Pros | Cons | Best For |
|----------|---------|-------|------|------|----------|
| **Sigmoid** | 1/(1+e⁻ᶻ) | (0,1) | Probabilistic output | Vanishing gradient; not zero-centered | Output layer (binary) |
| **Tanh** | (eᶻ-e⁻ᶻ)/(eᶻ+e⁻ᶻ) | (-1,1) | Zero-centered; stronger gradient | Still vanishes for large \|z\| | Hidden layers (legacy) |
| **ReLU** | max(0,z) | [0,∞) | No vanishing gradient; sparse; fast | Dying ReLU (z<0 → gradient=0) | Hidden layers (default) |
| **Leaky ReLU** | max(αz, z), α≈0.01 | (-∞,∞) | Fixes dying ReLU | Slightly more complex | Hidden layers (when ReLU fails) |
| **Softmax** | eᶻⁱ/Σⱼeᶻʲ | (0,1), Σ=1 | Multi-class probabilities | Requires careful numerical implementation | Output layer (multi-class) |

### CIA2 Assignment: Activation Function Outputs

> **Q: A neuron receives inputs z = [-3, -1, 0, 2, 4]. Compute ReLU output for each value.**

**Solution:**
```
ReLU Function: f(z) = max(0, z)

Apply element-wise:
    z = -3 → f(-3) = max(0, -3) = 0
    z = -1 → f(-1) = max(0, -1) = 0  
    z =  0 → f( 0) = max(0,  0) = 0
    z =  2 → f( 2) = max(0,  2) = 2
    z =  4 → f( 4) = max(0,  4) = 4

✅ Output: [0, 0, 0, 2, 4]

Observation: ReLU "kills" negative inputs (sets to 0), 
   passes positive inputs unchanged → introduces sparsity.
```

### CIA2 Assignment: Weighted Sum Calculation

> **Q: Neuron has Inputs x₁=1, x₂=2, Weights w₁=0.5, w₂=0.3, Bias b=0.2. Compute weighted sum z.**

**Solution:**
```
Weighted Sum Formula: z = Σ wᵢxᵢ + b

Step-by-Step:
    w₁x₁ = 0.5 × 1 = 0.5
    w₂x₂ = 0.3 × 2 = 0.6
    Sum of weighted inputs = 0.5 + 0.6 = 1.1
    Add bias: z = 1.1 + 0.2 = 1.3

✅ Answer: Weighted sum z = 1.3

Next Step (if asked): Apply activation, e.g., 
    ReLU: f(1.3) = 1.3
    Sigmoid: σ(1.3) = 1/(1+e⁻¹·³) ≈ 0.785
```

### CIA2 Assignment: Perceptron Classification

> **Q: Perceptron with w₁=0.4, w₂=-0.6, b=0.2, input x₁=1, x₂=0, step activation. Compute output and class.**

**Solution:**
```
Step 1: Compute Weighted Sum
    z = w₁x₁ + w₂x₂ + b = (0.4)(1) + (-0.6)(0) + 0.2 = 0.4 + 0 + 0.2 = 0.6

Step 2: Apply Step Activation Function
    f(z) = 1 if z ≥ 0, else 0
    Since z = 0.6 ≥ 0 → Output = 1

Step 3: Class Assignment
    Typically: Output 1 → Class 1; Output 0 → Class 0
    → Prediction: Class 1

✅ Answer: Perceptron output = 1 → Point belongs to Class 1
```

### CIA2 Assignment: Activation Function Comparison

> **Q: Compute outputs applying Sigmoid, ReLU, Tanh for z = [-2, -1, 0, 1, 2]. Compare behavior.**

**Solution Table:**
```
z    | Sigmoid σ(z)      | ReLU max(0,z) | Tanh tanh(z)
-----|-------------------|---------------|---------------
-2   | 1/(1+e²)=0.119    | 0             | (e⁻²-e²)/(e⁻²+e²)=-0.964
-1   | 1/(1+e¹)=0.269    | 0             | -0.762
 0   | 0.5               | 0             | 0
 1   | 0.731             | 1             | 0.762
 2   | 0.881             | 2             | 0.964

Behavior Comparison:
✅ Sigmoid: Smooth, bounded (0,1); saturates at extremes → vanishing gradient
✅ ReLU: Zero for negatives, linear for positives; sparse; no saturation for z>0
✅ Tanh: Zero-centered (-1,1); stronger gradients than sigmoid; still saturates

When to Use:
• Output layer (binary): Sigmoid (probabilities)
• Output layer (multi-class): Softmax
• Hidden layers: ReLU (default), Leaky ReLU if dying neurons
• When zero-centered needed: Tanh (but ReLU usually better in practice)
```

---

## 3.6 LIMITATIONS OF MACHINE LEARNING

### Critical Challenges (Exam Essential!)

| Limitation | Explanation | Mitigation Strategies |
|------------|-------------|----------------------|
| **Data Dependency** | "Garbage in, garbage out"; needs large, clean, labeled data | Data augmentation, transfer learning, active learning |
| **Overfitting** | Model memorizes training noise; poor generalization | Regularization, dropout, cross-validation, early stopping |
| **Underfitting** | Model too simple; misses patterns | More complex model, more features, longer training |
| **Bias & Fairness** | Biased training data → discriminatory predictions | Fairness-aware algorithms, diverse data, bias audits |
| **Interpretability** | Deep models = black boxes; hard to explain decisions | LIME, SHAP, attention visualization, simpler models when possible |
| **Computational Cost** | Deep learning needs GPUs, long training times | Model compression, distillation, efficient architectures |
| **Distribution Shift** | Test data distribution ≠ training → performance drop | Domain adaptation, online learning, robust training |
| **Adversarial Vulnerability** | Small input perturbations → wrong predictions | Adversarial training, input preprocessing, detection |

### CIA1-QP: Overfitting Identification

> **Q: A model performs well on training data but poorly on new data. Identify the issue and explain.**

**Answer:**
```
Issue: OVERFITTING (High Variance)

Symptoms:
• Training accuracy: Very high (e.g., 99%)
• Test/validation accuracy: Significantly lower (e.g., 70%)
• Large gap between train and test performance

Causes:
1️⃣ Model too complex relative to data size
   • Too many parameters → memorization capacity
2️⃣ Insufficient training data
   • Model learns noise instead of signal
3️⃣ No regularization
   • Weights grow large; model fits training noise
4️⃣ Training too long
   • Model starts fitting random fluctuations

Solutions:
✅ Regularization: L1/L2 penalties constrain weight magnitudes
✅ Dropout: Randomly deactivate neurons during training
✅ Cross-Validation: Monitor validation performance; early stopping
✅ Data Augmentation: Artificially expand training set
✅ Simplify Model: Reduce layers/neurons; feature selection
✅ Ensemble Methods: Average multiple models to reduce variance

✅ Key Insight: Goal is good GENERALIZATION, not perfect training fit.
   Use validation set to tune complexity and detect overfitting early.
```

---

## 3.7 DEEP LEARNING ARCHITECTURES

### Why Deep Learning? When to Use?

```
✅ Use Deep Learning When:
• Data is unstructured: images, text, audio, video
• Large labeled dataset available (10k+ samples)
• Computational resources sufficient (GPUs/TPUs)
• Feature engineering is difficult or domain expertise limited
• State-of-the-art performance is critical

❌ Use Traditional ML When:
• Tabular data with clear features
• Small dataset (<1k samples)
• Interpretability is required (healthcare, finance)
• Computational resources limited
• Quick prototyping needed
```

### Traditional ML vs Deep Learning Comparison

| Aspect | Traditional ML | Deep Learning |
|--------|---------------|---------------|
| **Features** | Hand-crafted by domain experts | Learned automatically from raw data |
| **Data Needs** | Hundreds to thousands of samples | Thousands to millions of samples |
| **Interpretability** | Often interpretable (trees, linear models) | Black box; requires post-hoc explanation |
| **Compute** | CPU sufficient | GPU/TPU often required |
| **Training Time** | Minutes to hours | Hours to days/weeks |
| **Best For** | Tabular data, structured problems | Images, text, speech, complex patterns |

---

## 3.8 CONVOLUTIONAL NEURAL NETWORKS (CNNs)

### Why CNNs for Images?

```
Key Insights:
1️⃣ Local Connectivity: Pixels near each other are more related
   • Neuron connects to small local region (receptive field)
   • Not fully connected → fewer parameters

2️⃣ Weight Sharing: Same filter detects feature anywhere in image
   • Translation invariance: "cat ear" pattern same whether top-left or bottom-right
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

### Output Size Formula (Critical for Exams!)

```
Output_Size = (Input_Size - Filter_Size + 2×Padding) / Stride + 1

Example:
    Input: 32×32 image
    Filter: 5×5
    Padding: 0 ("valid")
    Stride: 1
    Output = (32 - 5 + 0)/1 + 1 = 28 → 28×28 feature map

With 32 filters: Output volume = 28×28×32
```

### ASCII Diagram: CNN Layer Flow

```
Input Image (32×32×3 RGB)
        │
        ▼
[CONV: 5×5 filters, 32 filters, stride=1, pad=0]
        │
        ▼
Feature Maps (28×28×32)
        │
        ▼
[ReLU Activation]
        │
        ▼
[MaxPool: 2×2 window, stride=2]
        │
        ▼
Downsampled Maps (14×14×32)
        │
        ▼
[CONV → ReLU → Pool] × N times
        │
        ▼
[Flatten] → [FC Layers] → [Softmax] → Class Probabilities
```

### CIA2-QP: CNN vs RNN Distinction

> **Q: Distinguish between Convolutional Neural Network and Recurrent Neural Network based on their application to image and sequence data.**

**Model Answer:**
```
1. DATA STRUCTURE ASSUMPTIONS
   • CNN: Assumes grid-like topology (images: 2D grid; video: 3D grid)
     - Exploits spatial locality and translation invariance
     - Filters slide across spatial dimensions
   
   • RNN: Assumes sequential/temporal structure (text, speech, time series)
     - Exploits order and temporal dependencies
     - Hidden state carries information across time steps

2. CONNECTIVITY PATTERNS
   • CNN: Local connectivity + weight sharing
     - Each neuron connects to small local region (receptive field)
     - Same filter weights applied across entire input
     - Parameter-efficient for high-dimensional grid data
   
   • RNN: Recurrent connections
     - Hidden state hₜ depends on hₜ₋₁ and current input xₜ
     - Same weights (W, U) shared across all time steps
     - Naturally handles variable-length sequences

3. INVARIANCE PROPERTIES
   • CNN: Translation invariance
     - Pattern detected regardless of position in image
     - Pooling adds robustness to small shifts/distortions
   
   • RNN: Order sensitivity
     - "I love cats" ≠ "Cats love I"
     - Captures dependencies like subject-verb agreement

4. TYPICAL APPLICATIONS
   • CNN: Image classification, object detection, segmentation, 
          medical imaging, facial recognition
   
   • RNN/LSTM/GRU: Language modeling, machine translation, 
                   speech recognition, time series forecasting,
                   video captioning (often combined with CNN)

5. LIMITATIONS
   • CNN: Struggles with variable input sizes; ignores long-range 
          dependencies without very deep networks
   
   • RNN: Vanishing gradients limit learning long-term dependencies;
          sequential computation limits parallelization (addressed by Transformers)

✅ Modern Trend: Hybrid architectures
   • CNN + RNN: Image captioning (CNN extracts features, RNN generates text)
   • Transformers: Self-attention handles both spatial and sequential dependencies
```

---

## 3.9 RECURRENT NEURAL NETWORKS (RNNs)

### RNN Core Equation

```
Hidden State Update:
    hₜ = f(W·xₜ + U·hₜ₋₁ + b)

Output:
    yₜ = g(V·hₜ + c)

where:
• xₜ = input at time t
• hₜ = hidden state (memory) at time t  
• hₜ₋₁ = previous hidden state
• W, U, V = weight matrices (shared across time)
• f, g = activation functions (typically tanh for h, softmax for y)
```

### ASCII Diagram: RNN Unrolled Through Time

```
Folded Representation:          Unrolled Representation:
                                    
    xₜ → [ RNN ] → yₜ            x₁ → [h₁] → y₁
          ↑  │                          ↑   │
          └──┘                          │   │
          hₜ                           x₂ → [h₂] → y₂
                                            ↑   │
                                            │   │
                                           x₃ → [h₃] → y₃
```

### Vanishing Gradient Problem

**Why it happens:**
```
During Backpropagation Through Time (BPTT):
    ∂L/∂h₁ = ∂L/∂hₜ · ∂hₜ/∂hₜ₋₁ · ∂hₜ₋₁/∂hₜ₋₂ · ... · ∂h₂/∂h₁

If ‖∂hₖ₊₁/∂hₖ‖ < 1 (e.g., tanh derivative ≤ 1), product shrinks exponentially.
→ Gradients for early time steps → 0 → weights don't update → can't learn long dependencies
```

### Solutions: LSTM and GRU

**LSTM (Long Short-Term Memory): Gating Mechanism**
```
Three Gates Control Information Flow:
1. Forget Gate: fₜ = σ(W_f·[hₜ₋₁,xₜ] + b_f)
   → What to discard from cell state
   
2. Input Gate: iₜ = σ(W_i·[hₜ₋₁,xₜ] + b_i)
   → What new information to store
   
3. Output Gate: oₜ = σ(W_o·[hₜ₋₁,xₜ] + b_o)
   → What to output from cell state

Cell State Update:
    Cₜ = fₜ ⊙ Cₜ₋₁ + iₜ ⊙ tanh(W_C·[hₜ₋₁,xₜ] + b_C)
    hₜ = oₜ ⊙ tanh(Cₜ)

Key: Cell state Cₜ has additive updates → gradients flow unchanged → no vanishing
```

**GRU (Gated Recurrent Unit): Simplified Alternative**
```
Two Gates:
1. Update Gate: zₜ = σ(W_z·[hₜ₋₁,xₜ])
   → Balance between keeping old state vs updating with new
   
2. Reset Gate: rₜ = σ(W_r·[hₜ₋₁,xₜ])
   → How much past to ignore when computing candidate

Update:
    h̃ₜ = tanh(W·[rₜ ⊙ hₜ₋₁, xₜ])  (candidate)
    hₜ = (1-zₜ) ⊙ hₜ₋₁ + zₜ ⊙ h̃ₜ

Advantage: Fewer parameters than LSTM; often comparable performance
```

### CIA2-QP: RNN Hidden State Equation

> **Q: Write the RNN hidden state update equation. What problem does it face?**

**Answer:**
```
Hidden State Equation:
    hₜ = f(W·xₜ + U·hₜ₋₁ + b)

Components:
• hₜ: Hidden state at time t (network's "memory")
• xₜ: Input at time t
• hₜ₋₁: Previous hidden state (carries historical information)
• W: Input-to-hidden weight matrix
• U: Hidden-to-hidden (recurrent) weight matrix  
• b: Bias vector
• f: Activation function (typically tanh or ReLU)

Key Property: Same weights W, U, b used at ALL time steps → parameter sharing

Primary Problem: VANISHING GRADIENT
• During BPTT, gradients multiply by U repeatedly
• If spectral radius ρ(U) < 1, gradients shrink exponentially
• Early time steps receive near-zero gradient → weights don't learn
• Result: RNN struggles with long-term dependencies (e.g., pronoun reference across paragraphs)

Solutions:
1️⃣ Gradient Clipping: Cap gradient norm to prevent explosion (helps stability)
2️⃣ LSTM/GRU: Gating mechanisms create "gradient highways" for long-range flow
3️⃣ Residual Connections: Skip connections preserve gradient magnitude
4️⃣ Transformers: Self-attention directly connects any two positions (no recurrence)

✅ Modern Practice: Use LSTM/GRU for moderate sequences (<100 steps);
   Transformers for long sequences or when parallelization needed.
```

---

## 🎯 FINAL EXAM MASTER CHEAT SHEET

```
┌─────────────────────────────────────────────────────────┐
│  📊 ALL MODULES: KEY FORMULAS AT A GLANCE               │
├─────────────────────────────────────────────────────────┤
│  MODULE 1: Foundations                                  │
│  • Bayes: P(A\|B) = P(B\|A)P(A)/P(B)                   │
│  • Entropy: H = -ΣP·log₂P; IG = H(parent)-Σw·H(child) │
│  • Gradient Descent: w ← w - α∇L(w)                    │
│  • Eigenvalue: Av = λv; det(A-λI)=0                    │
│  • Euclidean: d = √Σ(xᵢ-yᵢ)²                           │
├─────────────────────────────────────────────────────────┤
│  MODULE 2: Supervised/Unsupervised                      │
│  • Logistic: ŷ = σ(wᵀx); Log Loss = -[y·logŷ+...]     │
│  • SVM: Min (1/2)‖w‖² s.t. yᵢ(wᵀxᵢ+b)≥1; Margin=2/‖w‖│
│  • KNN: c⁽ⁱ⁾ = argminₖ ‖x⁽ⁱ⁾-μₖ‖²                      │
│  • K-Means: J = ΣₖΣ‖x-μₖ‖²; μₖ = mean(Cₖ)             │
│  • PCA: C = (1/n)X'ᵀX'; EVR = λᵢ/Σλ                    │
│  • Metrics: Prec=TP/(TP+FP); Rec=TP/(TP+FN); F1=2PR/(P+R)│
├─────────────────────────────────────────────────────────┤
│  MODULE 3: Probabilistic & Deep Learning                │
│  • Naive Bayes: C* = argmax [log P(C) + Σlog P(xᵢ\|C)]│
│  • MLE: θ* = argmax Σlog P(x\|θ); MAP adds log P(θ)   │
│  • HMM: αₜ₊₁(j) = [Σᵢαₜ(i)Aᵢⱼ]·Bⱼ(oₜ₊₁)              │
│  • Perceptron: z = wᵀx+b; y = f(z)                     │
│  • CNN Output: (W-F+2P)/S + 1                          │
│  • RNN: hₜ = f(Wxₜ + Uhₜ₋₁ + b)                        │
├─────────────────────────────────────────────────────────┤
│  🎯 100/100 EXAM STRATEGY                               │
│  1️⃣ Part A (2-mark): Direct definitions, formulas,     │
│     short calculations → memorize cheat sheet           │
│  2️⃣ Part B (16-mark): Use frameworks:                  │
│     • Define → Explain → Example → Diagram → Limitation│
│     • Show ALL steps in numericals (partial credit!)    │
│  3️⃣ Diagrams: Draw ASCII only when asked or critical   │
│  4️⃣ Time Mgmt: Part A: 30 min; Part B: 60 min         │
│  5️⃣ Verify: Check eigenvalues (Trace=Σλ), Bayes denom │
└─────────────────────────────────────────────────────────┘
```

---

## 📚 APPENDIX: ALL CIA QUESTIONS INTEGRATED

### CIA1 Questions → Mapped to Topics

| Q# | Question | Topic | Page |
|----|----------|-------|------|
| A1 | List two ML applications | 1.1 Applications | 3 |
| A2 | What is overfitting? | 2.3 Under/Overfitting | 23 |
| A3 | Why ML data-dependent? | 3.6 Limitations | 55 |
| A4 | Random variable definition | 1.4 Probability | 12 |
| A5 | E-commerce recommendation suitability | 2.13 Recommendation Systems | 47 |
| A6 | Gmail spam classification | 3.1 Naive Bayes | 48 |
| A7 | Sales prediction task type | 1.2 Supervised Learning | 5 |
| A8 | House price model selection | 2.2 Linear Regression | 21 |
| A9 | Bayes' theorem statement | 1.4 Bayesian Probability | 13 |
| B1 | Logistic regression for loan default | 2.5 Logistic Regression | 27 |
| B2 | Medical test Bayes calculation | 1.4 Bayes Application | 14 |
| B3 | Cosine similarity for users | 2.7 KNN/Collaborative Filtering | 33 |
| B4 | Customer purchase behavior ML application | 1.1 Applications | 3 |
| B5 | Cross-validation for exam prediction | 2.4 Cross-Validation | 25 |
| B6 | Underfitting/overfitting solutions | 2.3 Regularization | 23 |
| B7 | Lasso for feature selection | 2.3 Lasso Regression | 24 |

### CIA2 Questions → Mapped to Topics

| Q# | Question | Topic | Page |
|----|----------|-------|------|
| A1 | Euclidean distance calculation | 1.3 Linear Algebra | 9 |
| A2 | Decision Tree vs KNN classification | 2.7-2.8 Tree/KNN | 33,36 |
| A3 | K-Means K value effect | 2.11 Clustering | 43 |
| A4 | Naive Bayes posterior calculation | 3.1 Naive Bayes | 48 |
| A5 | MLE vs MAP comparison | 3.2 MLE/MAP | 49 |
| A6 | HMM state sequence identification | 3.4 HMM | 52 |
| A7 | Neuron output with sigmoid | 3.5 Activation Functions | 57 |
| A8 | CNN vs RNN distinction | 3.8-3.9 CNN/RNN | 58,61 |
| A9 | Overfitting: DL vs traditional ML | 3.6 Limitations | 55 |
| B10i | Decision Tree (ID3/CART) for customer classification | 2.8 Decision Trees | 36 |
| B10ii | K-Means clustering by hand | 2.11 K-Means | 43 |
| B11i | Naive Bayes spam classification | 3.1 Naive Bayes | 48 |
| B11ii | HMM/RNN for sequence prediction | 3.4-3.9 HMM/RNN | 52,61 |
| B12i | Perceptron output calculation | 3.5 Perceptron | 57 |
| B12ii | Activation functions comparison | 3.5 Activation Functions | 57 |
| B13i | Information gain for decision tree root | 2.8 ID3/Entropy | 36 |
| B13ii | Traditional ML vs DL for image recognition | 3.7 Why Deep Learning | 56 |

### Assignment Questions → Mapped to Topics

| Q# | Question | Topic | Page |
|----|----------|-------|------|
| A1 | ID3 vs CART differentiation | 2.8 Decision Trees | 36 |
| A2 | User similarity in recommendations | 2.13 Recommendation Systems | 47 |
| A3 | EM algorithm definition | 2.13 EM Algorithm | 47 |
| A4 | Elbow Method for K selection | 2.11 Cluster Validity | 45 |
| A5 | Bias role in perceptron | 3.5 Perceptron | 54 |
| A6 | Feedforward NN components | 3.5 MLP Architecture | 55 |
| A7 | ReLU output computation | 3.5 Activation Functions | 57 |
| A8 | Weighted sum calculation | 3.5 Perceptron | 57 |
| A9 | Traditional ML limitations | 3.6 Limitations | 55 |
| B10i | K-Means on distance matrix | 2.11 K-Means | 43 |
| B10ii | PCA principal component computation | 2.12 PCA | 46 |
| B11i | Bayesian classification example | 3.1 Naive Bayes | 48 |
| B11ii | HMM probability calculation | 3.4 HMM | 52 |
| B12i | Perceptron classification | 3.5 Perceptron | 57 |
| B12ii | Activation functions comparison | 3.5 Activation Functions | 57 |
| B13i | Information gain for root node | 2.8 ID3/Entropy | 36 |
| B13ii | Traditional ML vs DL for images | 3.7-3.8 CNN | 56,58 |

---

## 🏆 FINAL TIPS FOR 100/100

```
✅ BEFORE EXAM:
• Memorize the Cheat Sheet formulas (1 page)
• Practice 2 numericals from each module (show all steps)
• Draw 3 ASCII diagrams from memory (SVM margin, K-means, RNN unrolled)

✅ DURING EXAM:
• Part A: Answer in 2-3 lines; include formula if applicable
• Part B: Use framework: Definition → Explanation → Example → Diagram → Limitation
• Numericals: Box final answer; show units; verify with properties (e.g., Σλ=Trace)
• Time: Spend max 3 min on Part A questions; 15 min on Part B

✅ COMMON PITFALLS TO AVOID:
• Forgetting to compute P(B) in Bayes problems
• Using Euclidean distance without feature scaling in KNN
• Confusing precision/recall formulas
• Not checking eigenvalue properties (Trace, Det)
• Drawing diagrams without labeling components

✅ LAST-MINUTE REVISION (1 hour before):
1. Bayes theorem + spam example
2. Entropy/IG calculation steps  
3. K-Means iteration workflow
4. PCA eigenvalue interpretation
5. Backpropagation chain rule intuition
6. CNN output size formula
7. RNN vanishing gradient + LSTM solution

🎯 YOU'VE GOT THIS! 
   This guide covers 100% of CIA1 + CIA2 + Assignment content.
   Focus on understanding frameworks, not rote memorization.
   Show your working → partial credit → centum secured! ✨
```

---

*End of Machine Learning Techniques (23CSC02) Centum Study Guide*  
*Total Pages: ~60 | Target: 100/100 | Last Updated: April 2026*  
*Sri Krishna College of Technology | B.E. CSE(AIML) | Semester 4*

> "The best way to predict the future is to learn the patterns that create it." — ML Proverb 🤖📈
