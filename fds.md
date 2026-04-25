# 📚DATA SCIENCE STUDY GUIDE
## 🎯 Complete Path to 100/100 | Units 1-5 Merged

---

# 📖 MODULE 1: INTRODUCTION AND DESCRIBING DATA

## 1.1 DATA SCIENCE: FOUNDATIONS & BENEFITS

### What is Data Science?

**Data Science** is the domain of study that deals with vast volumes of data using modern tools and techniques (like machine learning) to:
- ✅ Find unseen patterns
- ✅ Derive meaningful information  
- ✅ Make business decisions

```
                    +-------------------+
                    |   DATA SCIENCE    |
                    |  (Uncovering      |
                    |   Patterns &      |
                    | Driving Decisions)|
                    +-------------------+
                           /|\
                          / | \
                         /  |  \
                        /   |   \
           +-----------+    |    +------------+
           |  MATH &   |----+----|  COMPUTER  |
           | STATISTICS|         |  SCIENCE/IT|
           +-----------+         +------------+
                        \   |   /
                         \  |  /
                          \ | /
                           \|/
                    +------------+
                    |  BUSINESS  |
                    |   DOMAIN   |
                    |  KNOWLEDGE |
                    +------------+
```

### Core Activities in Data Science

1. **Asking correct questions** and analyzing raw data
2. **Modeling data** using complex, efficient machine learning algorithms
3. **Visualizing data** to get a better perspective
4. **Understanding the data** to make better decisions

### Benefits of Data Science

| Benefit | Description |
|---------|-------------|
| 🔍 Better Decision Making | Data-driven decisions by analyzing patterns, reducing guesswork |
| 🎯 Identifying Target Audiences | Segment valuable customer groups for effective marketing |
| 💡 Identifies Opportunities | Discover new business opportunities through pattern recognition |
| ⚡ Improves Performance | Optimize business processes and operational efficiency |

### Uses and Applications

**Applications:**
- Fraud & Risk Detection
- Delivery Logistics
- Gaming
- Price Comparison Websites
- Recommender Systems (Netflix, Amazon)
- Digital Advertisements
- Internet Search (Google)
- Speech/Image Recognition

**Real-World Uses:**
- Predicts future outcomes
- Lowers risks (e.g., driverless cars)
- Customizes therapeutics (genomics)
- Transforms user data into profitable information

---

## 1.2 FACETS OF DATA

Data exists in multiple forms. Understanding these is crucial for proper data handling.

### 1. Structured Data ✅
**Definition:** Organized in rows and columns format with fixed schema.

**Characteristics:**
- Easily searchable by data type
- Understood by both computers and humans
- Fixed schema

**Examples:**
```
+----------+----------+----------+----------+
|   ID     |   Name   |   Age    |  Salary  |
+----------+----------+----------+----------+
|    1     |  Alice   |    25    |  50000   |
|    2     |   Bob    |    30    |  60000   |
+----------+----------+----------+----------+
```

### 2. Unstructured Data ✅
**Definition:** Does not follow a specified format or structural rules.

**Key Facts:**
- Makes up **>80% of all data**
- Unpredictable in nature
- No predefined data model

**Examples:** Emails, PDFs, customer feedback, images, videos, audio files

### 3. Semi-structured Data ✅
**Definition:** Contains tags/markers to separate elements; has some organizational properties but not rigid structure.

**Examples:** JSON, XML files

### 4. Natural Language ✅
**Definition:** Human speech and text requiring **NLP (Natural Language Processing)**.

**NLP Capabilities:**
- Understand meaning
- Recognize entities
- Summarize text
- Perform sentiment analysis

**Examples:** Social media posts, chat logs, news articles, customer reviews

### 5. Machine-Generated Data ✅
**Definition:** Created without human interaction by computer processes.

**Types:**
- **M2M (Machine-to-Machine)** interactions
- **H2M (Human-to-Machine)** interactions

**Examples:** Web server logs, IoT sensor data, call detail records, telemetry data

### 6. Graph-Based (Network) Data ✅
**Definition:** Describes relationships (edges) between entities (nodes).

```
        (Alice)-----(Bob)
           |           |
           |           |
        (Carol)-----(David)
           \         /
            \       /
           (Eve)
```

**Storage:** Graph databases, queries like SPARQL

### 7. Audio, Image, and Video (Multimedia) ✅
**Characteristics:**
- Time-based media storage
- Trivial for humans, challenging for computers
- Requires deep learning and computer vision techniques

### 8. Streaming Data ✅ *(From PDF)*
**Definition:** Data generated continuously by thousands of sources simultaneously.

**Characteristics:**
- Real-time generation
- High velocity
- Continuous flow in small sizes (Kilobytes)

**Examples:** Live ecommerce purchases, in-game player activity, financial trading, social media feeds

```
📊 Data Distribution in Organizations:
┌─────────────────────────────────┐
│ Unstructured: ████████████ 80%+ │
│ Structured:   ████ 15%          │
│ Semi-struct:  █ 5%              │
└─────────────────────────────────┘
```

---


## 1.3 THE DATA SCIENCE PROCESS (6 Steps)

```
    +----------------+     +----------------+     +----------------+
    | 1. Setting     | --> | 2. Retrieving  | --> | 3. Data        |
    | Research Goal  |     |    Data        |     | Preparation    |
    +----------------+     +----------------+     +----------------+
           ^                                              |
           |                                              v
    +----------------+     +----------------+     +----------------+
    | 6. Presentation| <-- | 5. Data        | <-- | 4. Data        |
    | & Automation   |     | Modeling       |     | Exploration    |
    +----------------+     +----------------+     +----------------+
```

### Step 1: Setting the Research Goal 🎯

**Purpose:** Define the **what, how, and why** so all stakeholders are aligned.

**Project Charter Contains:**
| Component | Description |
|-----------|-------------|
| Clear research goal | What problem are we solving? |
| Project mission/context | Why does this matter? |
| Analysis plan | How will we approach it? |
| Required resources | What do we need? |
| Proof of concept | Can it be done? |
| Deliverables | What will we produce? |
| Timeline | When will it be completed? |

**⚠️ Warning:** Without a well-defined research goal, the project can drift in the wrong direction, wasting time and resources.

### Step 2: Retrieving Data 📥

**Data Sources:**

| Type | Examples |
|------|----------|
| **Internal** | Company databases, data marts, data warehouses, data lakes |
| **External** | Purchased data (Nielsen), Twitter APIs, government datasets |

**Quality Checks at This Stage:**
- Check for missing values
- Verify data types
- Identify duplicates
- Validate ranges

### Step 3: Data Preparation ⚙️ *(CRUCIAL - 80% of Time!)*

#### A. Data Cleansing:
1. **Fixing errors and typos** - Correct spelling mistakes, formatting inconsistencies
2. **Handling Missing Values:**
   ```
   • Imputation: Fill with mean/median/mode
   • Forward fill (ffill): Use previous value
   • Backward fill (bfill): Use next value
   • Deletion: Remove rows/columns with missing data
   ```
3. **Handling Outliers:**
   ```
   • Cap them (set maximum threshold)
   • Remove them entirely
   • Transform the data
   ```
4. **Removing Duplicates** - Prevents bias in analysis

#### B. Data Transformation:
1. Aggregating data to suitable level
2. Deriving new computed measures (e.g., profit margin)
3. Creating dummy variables for categorical data
4. Joining multiple datasets
5. Converting formats (text to numbers)

### Step 4: Data Exploration (EDA) 🔍

**Purpose:** Dive deeper into cleaned data using descriptive statistics and visualization to discover patterns before modeling.

**Techniques:**
| Technique | Purpose |
|-----------|---------|
| Histograms | Distribution of single variable |
| Density plots | Smoothed distribution |
| Box plots | Quartiles and outliers |
| Scatter plots | Relationships between two variables |
| Brushing & Linking | Select observations in one plot, highlight in others |

### Step 5: Data Modeling 🤖

**Key Sub-tasks:**

1. **Model Selection** - Choose algorithm based on:
   - Performance requirements
   - Ease of implementation
   - Explainability
   - Maintenance cost

2. **Execution** - Using Python libraries:
   ```python
   # Key libraries
   import sklearn      # Machine learning algorithms
   import statsmodels  # Statistical models
   import numpy, pandas # Data manipulation
   ```

3. **Model Evaluation** - Holdout Sample strategy:
   ```
   • Typical split: 80% training / 20% testing
   • Train on training data, evaluate on unseen test data
   • Error measures: MSE, RMSE, R²
   ```

### Step 6: Presentation and Automation 📊

**A. Presentation:**
- Create clear visual reports
- Build dashboards (Tableau, Power BI)
- Prepare executive summaries
- Translate findings into actionable business recommendations

**B. Automation:**
- Set up automated pipelines
- Model scores new data automatically
- Update reports without manual intervention
- Schedule retraining cycles

---

## 1.4 DATA MINING vs DATA WAREHOUSING

### DATA WAREHOUSING

**Definition:** A **subject-oriented, integrated, time-varying, and non-volatile** database system designed for analytical analysis.

**Key Characteristics:**
| Characteristic | Description |
|---------------|-------------|
| **Subject-Oriented** | Organized around business subjects (sales, customers), not operational processes |
| **Integrated** | Combines data from multiple heterogeneous sources into consistent format |
| **Time-Varying** | Stores historical data over time for trend analysis |
| **Non-Volatile** | Data is loaded and read, NOT frequently updated or deleted |

**ETL Process:**
```
┌─────────────┐    ┌──────────────┐    ┌─────────────┐
│   EXTRACT   │ -> │  TRANSFORM   │ -> │    LOAD     │
└─────────────┘    └──────────────┘    └─────────────┘
│                    │                    │
v                    v                    v
Multiple sources    Clean, standardize,   Warehouse for
(Sales, CRM, etc.)  restructure data      querying
```

**Advantages:** Easy to understand, continuous updates, stores historical data, faster reporting
**Disadvantages:** Risk of accumulating irrelevant data, complex cleansing from multiple sources
**Managed by:** Data Engineers / IT teams

### DATA MINING

**Definition:** Process of analyzing large datasets using **AI, machine learning, and statistical techniques** to discover meaningful patterns and predict future outcomes.

**Key Techniques:**
| Technique | Description | Example |
|-----------|-------------|---------|
| **Classification** | Assigning items into predefined categories | Spam vs. not spam detection |
| **Clustering** | Grouping similar data points without labels | Customer segmentation |
| **Association Rule Mining** | Finding "if-then" patterns | "Customers who buy bread also buy butter" |
| **Prediction/Regression** | Forecasting continuous numerical outcomes | Predicting house prices |

**Advantages:** Fault detection, cost-effective, actionable knowledge
**Disadvantages:** Not 100% accurate, resource-heavy, privacy concerns
**Managed by:** Data Scientists / Business Users

### 📊 Comparison Table: Data Warehousing vs Data Mining *(CIA Exam Ready)*

| Feature | Data Warehousing | Data Mining |
|---------|-----------------|-------------|
| **Definition** | Database system for analytical analysis | Process of analyzing data to find patterns |
| **Process** | ETL (Extract, Transform, Load) | AI, ML, Statistics |
| **Purpose** | Store & report on historical data | Discover hidden patterns & predict outcomes |
| **Data Handling** | Pools all relevant data together | Extracts knowledge from large datasets |
| **Managed By** | Data Engineers | Data Scientists / Business Users |
| **Functionality** | Subject-oriented, integrated, time-varying, non-volatile | AI, statistics, databases, machine learning |
| **Task** | Extracting and storing data for efficient reporting | Pattern recognition logic to find patterns |
| **Uses** | Makes reporting easier and faster | Aids in identification of access patterns |
| **Example** | Consolidating sales from 50 stores into one server | Finding "customers who buy X also buy Y" |

---

## 1.5 TYPES OF DATA & VARIABLES

### Qualitative vs Quantitative Data

```
                        DATA
                          |
            +-------------+-------------+
            |                           |
    QUALITATIVE                  QUANTITATIVE
   (Categorical)                   (Numerical)
            |                           |
    +-------+-------+           +-------+-------+
    |               |           |               |
NOMINAL        ORDINAL      DISCRETE      CONTINUOUS
```

| Type | Description | Examples |
|------|-------------|----------|
| **Qualitative** | Describes qualities, non-numeric | Gender, color, brand name |
| **Quantitative** | Represents measurable quantities | Height, weight, temperature |
| **Discrete** | Countable, whole numbers only | Number of students, cars |
| **Continuous** | Measurable, infinite decimals allowed | Height, temperature, time |

### Four Scales of Measurement (NOIR)

| Scale | Order? | Equal Intervals? | True Zero? | Examples |
|-------|--------|-----------------|------------|----------|
| **Nominal** | ❌ | ❌ | ❌ | Gender, colors, countries |
| **Ordinal** | ✅ | ❌ | ❌ | Star ratings, education level |
| **Interval** | ✅ | ✅ | ❌ | Temperature °C, calendar years |
| **Ratio** | ✅ | ✅ | ✅ | Weight, income, age, height |

### Types of Variables

| Variable | Role | Also Called | Example |
|----------|------|-------------|---------|
| **Independent (IV)** | Hypothesized cause, manipulated | Predictor, Explanatory | Study hours |
| **Dependent (DV)** | Effect/outcome, measured | Response, Outcome | Exam scores |
| **Control** | Held constant to prevent bias | - | Room temperature |
| **Confounding** | Hidden variable affecting both IV & DV | - | Temperature in ice cream/drowning study |

---

## 1.6 DESCRIPTIVE STATISTICS

### Measures of Central Tendency

#### Mean (Arithmetic Average)
```
        Σx
   μ = ─────
        n
```
**Characteristics:** Uses all data, sensitive to outliers, best for symmetric data

**Example:**
```
Data: {40, 45, 50, 55, 60}
Sum = 250, n = 5
Mean = 250/5 = 50
```

#### Median
**Definition:** Exact middle value when data is ordered.

**How to Find:**
```
• Odd n: Median = middle value at position (n+1)/2
• Even n: Median = average of two middle values
```
**Characteristics:** NOT affected by outliers, preferred for skewed data

**Example with Outliers:**
```
Salaries: [30000, 32000, 35000, 38000, 200000]
Mean = ₹67,000 (skewed by outlier)
Median = ₹35,000 (representative!)
```

#### Mode
**Definition:** Most frequently occurring value.

**Types:** Unimodal (1), Bimodal (2), Multimodal (>2), No mode

### Measures of Variability (Dispersion)

#### Range
```
Range = Maximum - Minimum
```
**Characteristics:** Simplest measure, heavily affected by outliers

#### Variance (σ²)
```
          Σ(x - μ)²
   σ² = ───────────
             n
```
**Characteristics:** Uses all data, squared units, always positive

#### Standard Deviation (σ)
```
   σ = √σ²
```
**Characteristics:** In original units, most widely used measure of spread

#### Coefficient of Variation (CV)
```
         σ
   CV = ─── × 100%
         μ
```
**Interpretation:**
- CV < 10% → Low variability
- CV 10-30% → Moderate variability  
- CV > 30% → High variability

**Example - Comparing Datasets:**
```
Dataset A: Mean=100, SD=10 → CV = 10%
Dataset B: Mean=50, SD=10  → CV = 20%
→ Dataset B is MORE variable relative to its mean!
```

### Linear Transformation Effects

| Operation | Mean | Median | Variance | SD |
|-----------|------|--------|----------|-----|
| **Add constant (+c)** | +c | +c | Same | Same |
| **Multiply by constant (×c)** | ×c | ×c | ×c² | ×c |

---

## 1.7 DISTRIBUTION SHAPES & VISUALIZATION

### Skewness (Symmetry)

```
Symmetric:           Right-Skewed:        Left-Skewed:
     ▲                    ▲                    ▲
     │       ╱─╲          │         ╱─╲        │  ╱─╲
     │     ╱     ╲        │       ╱       ╲    │╱     
     │   ╱         ╲      │     ╱           ╲  │       ╲
     │ ╱             ╲    │   ╱               ╲│        ╲
     └─────────────────   └────────────────────└─────────────────
     M=Md=Mo              Mo  Md   M            M   Md  Mo
```

| Distribution | Relationship | Example |
|-------------|--------------|---------|
| **Symmetric** | Mean = Median = Mode | Heights of adults |
| **Right-Skewed** | Mean > Median > Mode | Income distribution |
| **Left-Skewed** | Mean < Median < Mode | Age at retirement |

### Kurtosis (Peakedness)

| Type | Description | Kurtosis | Outliers |
|------|-------------|----------|----------|
| **Mesokurtic** | Normal bell shape | = 3 | Normal |
| **Leptokurtic** | High peak, heavy tails | > 3 | More outliers |
| **Platykurtic** | Flat, light tails | < 3 | Fewer outliers |

### Frequency Distribution Tables

**Ungrouped (Individual Values):**
```
Marks    Frequency
10         2
15         5
20         8
25         3
30         2
```

**Grouped (Class Intervals):**
```
Class Interval    Frequency    Midpoint
10-14             3            12
15-19             7            17
20-24            12            22
25-29             5            27
30-34             3            32
```

### Data Visualization Types

| Chart | Best For | Key Features |
|-------|----------|--------------|
| **Histogram** | Continuous data distribution | Contiguous bars, shows shape/spread |
| **Frequency Polygon** | Comparing multiple distributions | Line connecting midpoints |
| **Bar Chart** | Categorical data comparison | Gaps between bars |
| **Pie Chart** | Showing proportions | Slices of circle, total=100% |
| **Line Graph** | Trends over time | Points connected by lines |
| **Box Plot** | Quartiles and outliers | 5-number summary, IQR |
| **Scatter Plot** | Relationship between 2 variables | X-Y points, shows correlation |

---
### Box Plot Components *(Important for CIA)*

```
    Value
      90 |                    ○ (outlier)
      80 |                    │
      75 |              +-----+ ← Q3 (75th percentile)
      70 |              │     │
      65 |         +----+     │
      60 |         │    │     │
      55 |         │    │     │
      50 |    +----+    │     │ ← Q1 (25th percentile)
      45 |    │         │     │
      40 +----+---------+-----+
           Min         Med    Max
```

**5-Number Summary:**
- Minimum
- Q1 (25th percentile)
- Median/Q2 (50th percentile)
- Q3 (75th percentile)
- Maximum

**IQR (Interquartile Range):** Q3 - Q1

**Outlier Detection:**
- Lower fence: Q1 - 1.5×IQR
- Upper fence: Q3 + 1.5×IQR
- Points beyond fences = outliers

---


## 1.8 NORMAL DISTRIBUTION & Z-SCORES

### Normal Distribution Properties

```
        Normal Distribution Curve
        
           ▲
           │           ╱─╲
           │         ╱     ╲
           │       ╱         ╲
  Frequency│     ╱             ╲
           │   ╱                 ╲
           │ ╱                     ╲
           │                         ╲
           └─────────────────────────────►
              μ-3σ μ-2σ μ-1σ μ μ+1σ μ+2σ μ+3σ
```

**Characteristics:**
- ✅ Symmetric around mean
- ✅ Mean = Median = Mode
- ✅ Bell-shaped curve
- ✅ Tails never touch x-axis
- ✅ Total area = 1 (100%)

### Empirical Rule (68-95-99.7)

```
        68%           95%            99.7%
    ┌─────────┐   ┌───────────┐   ┌─────────────┐
    │         │   │           │   │             │
    │   ╱─╲   │   │   ╱───╲   │   │   ╱─────╲   │
    │ ╱     ╲ │   │ ╱       ╲ │   │ ╱         ╲ │
    │╱       ╲│   │╱         │   │╱           ╲│
    └─────────┘   └───────────┘   └─────────────┘
    μ-1σ   μ+1σ   μ-2σ     μ+2σ   μ-3σ       μ+3σ
```

| Range | Percentage | Example (μ=50, σ=8) |
|-------|------------|---------------------|
| μ ± 1σ | 68% | 42 to 58 |
| μ ± 2σ | 95% | 34 to 66 |
| μ ± 3σ | 99.7% | 26 to 74 |

**Example Problem:**
```
Given: μ=50, σ=8
Q: What % beyond 66?
A: 66 = μ+2σ → 95% within ±2σ → 5% outside → 2.5% beyond 66
```

### Z-Score (Standard Score)

```
         X - μ
   Z = ─────────
          σ
```

**Interpretation:**
| Z-Score | Meaning |
|---------|---------|
| Z = 0 | Value equals mean |
| Z > 0 | Value above mean |
| Z < 0 | Value below mean |
| \|Z\| > 3 | Potential outlier |

**Applications:**
1. Comparing scores from different distributions
2. Identifying outliers
3. Finding percentiles
4. Standardizing variables

**Example - Comparing Tests:**
```
SAT Math: Score=650, μ=500, σ=100 → Z = (650-500)/100 = 1.5
ACT Math: Score=28, μ=21, σ=5     → Z = (28-21)/5 = 1.4
→ SAT performance is slightly better relative to distribution
```

---

# 📖 MODULE 2: DESCRIBING RELATIONSHIPS

## 2.1 CORRELATION

### Definition & Key Points

**Correlation** measures the **strength and direction** of the **linear relationship** between two quantitative variables.

**Key Facts:**
- ✅ Range: **-1.0 to +1.0**
- ✅ Symmetric: Correlation of X with Y = Correlation of Y with X
- ✅ **Does NOT imply causation**
- ✅ Only measures **linear** relationships

### Types of Correlation

```
Strong Positive (r≈0.9)    Weak Positive (r≈0.4)    No Correlation (r≈0)
     ▲                          ▲                        ▲
     │  ●●●                    │ ●  ●                 │●  ● ●
     │ ●●●●                    │● ●● ●                 │ ● ●●
     │●●●●●                    │ ● ● ●                 │● ● ●
     │●●●                      │  ● ●                  │ ●● ●
     │                         │                       │● ● ●
     └────────►               └────────►              └────────►

Strong Negative (r≈-0.9)   Weak Negative (r≈-0.4)
     ▲                          ▲
     │●●●                      │  ● ●
     │ ●●●●                    │ ● ●●
     │  ●●●●●                  │● ● ●
     │   ●●●                   │ ●● ●
     │                         │● ●
     └────────►               └────────►
```

### Interpreting r Values

| r Value Range | Interpretation |
|---------------|----------------|
| **+0.8 to +1.0** | Strong positive correlation |
| **+0.3 to +0.7** | Moderate positive correlation |
| **0 to +0.2** | Weak or no positive correlation |
| **0** | No linear correlation |
| **-0.2 to 0** | Weak or no negative correlation |
| **-0.3 to -0.7** | Moderate negative correlation |
| **-0.8 to -1.0** | Strong negative correlation |

### Pearson Correlation Coefficient

**Computational Formula:**
```
           n(ΣXY) - (ΣX)(ΣY)
   r = ─────────────────────────────────────
       √{[nΣX² - (ΣX)²] × [nΣY² - (ΣY)²]}
```

**Step-by-Step Example:**
```
Data: Study Hours (X) vs Exam Scores (Y)
Student  X   Y   X²   Y²   XY
   1     2  50    4 2500  100
   2     4  60   16 3600  240
   3     6  70   36 4900  420
   4     8  80   64 6400  640
   5    10  90  100 8100  900
────────────────────────────
Σ      30 350  220 25500 2300

n=5
r = [5(2300) - (30)(350)] / √{[5(220)-900][5(25500)-122500]}
r = 1000 / √(200×5000) = 1000/1000 = 1.0

Answer: Perfect positive correlation!
```

### Spearman Rank Correlation (ρ)

**Used when:**
- Data is ordinal (ranked)
- Relationship is monotonic but not linear
- Data has outliers
- Data is not normally distributed

**Formula:**
```
          6Σd²
   ρ = 1 - ─────────
         n(n² - 1)
```
Where d = difference between ranks of X and Y

### Coefficient of Determination (R²)

```
   R² = r²
```

**Interpretation:** Proportion of variance in Y explained by X.

**Example:**
```
r = 0.85 → R² = 0.7225 = 72.25%
→ 72.25% of variation in Y is explained by X
→ Remaining 27.75% due to other unmeasured factors
```

---

## 2.2 REGRESSION

### Correlation vs Regression

| Correlation | Regression |
|-------------|------------|
| Measures strength of relationship | Models functional relationship |
| Symmetric (X↔Y) | Asymmetric (X→Y) |
| Single value (r) | Equation (Ŷ = a + bX) |
| No prediction | Enables prediction |

### Regression Line (Line of Best Fit)

**Equation:**
```
   Ŷ = a + bX

Where:
Ŷ = Predicted value of Y
a = Y-intercept (predicted Y when X=0)
b = Slope (change in Y per 1-unit increase in X)
X = Independent variable
```

### Least Squares Principle

**Concept:** Finds line that **minimizes sum of squared residuals**:
```
   Minimize: Σ(Y - Ŷ)²
```

**Formulas:**
```
           n(ΣXY) - (ΣX)(ΣY)
   b = ─────────────────────────
           nΣX² - (ΣX)²

   a = Ȳ - bX̄
```

**Interpretation:**
- **Slope (b):** Change in Y for one-unit increase in X
- **Intercept (a):** Predicted Y when X=0 (may not be meaningful)

### Complete Regression Example

**Problem:** Predict exam scores from study hours

```
X(Hours): 2, 4, 6, 8, 10
Y(Score): 50, 60, 70, 80, 90

Calculation:
ΣX=30, ΣY=350, ΣX²=220, ΣY²=25500, ΣXY=2300, n=5
X̄=6, Ȳ=70

b = [5(2300) - (30)(350)] / [5(220) - 900] = 1000/200 = 5
a = 70 - 5(6) = 40

Equation: Ŷ = 40 + 5X

Prediction for 7 hours: Ŷ = 40 + 5(7) = 75
```

### Finding Equation from Means and SDs

**When given:** x̄, ȳ, Sₓ, Sᵧ, r

```
              Sᵧ
   b = r × ───────
              Sₓ
   
   a = ȳ - b(x̄)
```

**Example:**
```
Given: x̄=5, ȳ=10, Sₓ=2, Sᵧ=4, r=0.75

b = 0.75 × (4/2) = 1.5
a = 10 - 1.5(5) = 2.5

Equation: Ŷ = 2.5 + 1.5X
```

### Limitations of Regression

1. ❌ **Doesn't prove causation** - Need experimental design
2. ❌ **Extrapolation is unreliable** - Don't predict outside data range
3. ❌ **Sensitive to outliers** - Single outlier can drastically change line
4. ❌ **Only fits linear patterns** - Need polynomial/non-linear for curves

---

## 2.3 STANDARD ERROR OF ESTIMATE (SEE)

### Definition & Formula

**SEE** measures **prediction accuracy** by finding average distance between observed and predicted values.

```
           Σ(Y - Ŷ)²
   SEE = √───────────
             n - 2
```

### Interpretation

| SEE Value | Meaning |
|-----------|---------|
| **Smaller SEE** | Better predictions (points closer to line) |
| **Larger SEE** | Less accurate predictions |
| **Units** | Same as Y variable (unlike R² which is %) |

**Relationship with R²:**
- Higher R² → Lower SEE (better model)
- Lower R² → Higher SEE (worse model)

### Example Calculation

```
Actual(Y)  Predicted(Ŷ)  Residual  Residual²
   50          45          +5         25
   60          62          -2          4
   70          68          +2          4
   80          83          -3          9
   90          87          +3          9
─────────────────────────────────────
Σ(Y-Ŷ)² = 51

SEE = √(51/(5-2)) = √17 = 4.12

Interpretation: Predictions are off by ~4.12 units on average
```

---

## 2.4 MULTIPLE REGRESSION

### From Simple to Multiple

**Simple Regression:**
```
Ŷ = β₀ + β₁X
• One predictor
• Fits straight line
```

**Multiple Regression:**
```
Ŷ = β₀ + β₁X₁ + β₂X₂ + ... + βₙXₙ
• Multiple predictors
• Fits hyperplane in n-dimensions
• Explains more variance
```

### Anatomy of Multiple Regression Equation

```
Ŷ = β₀ + β₁X₁ + β₂X₂ + β₃X₃ + ε

Term          Meaning
─────────────────────────────────
Ŷ            Predicted value (model's estimate)
β₀           Intercept (Y when ALL predictors = 0)
β₁, β₂, β₃   Coefficients (change in Y per 1-unit 
              increase in Xᵢ, holding others constant)
X₁, X₂, X₃   Predictors/Features (independent variables)
ε            Error term (unexplained residual)
```

**🔑 Key Power:** Each coefficient shows the **isolated effect** of one variable while controlling for all others!

### Worked Example: House Price Prediction

**Equation:**
```
Price = 10 + 0.8(Size) - 0.5(Age) + 3.2(Bedrooms)
```

**Interpretation:**
| Coefficient | Value | Meaning |
|-------------|-------|---------|
| β₀ | 10 | Base price: ₹10L when all inputs = 0 |
| β₁ | +0.8 | Each extra m² adds ₹0.8L (holding others constant) |
| β₂ | -0.5 | Each year older reduces price by ₹0.5L |
| β₃ | +3.2 | Each extra bedroom adds ₹3.2L |

**Prediction:**
```
For 120m², 5 years old, 3 bedrooms:
Price = 10 + 0.8(120) - 0.5(5) + 3.2(3)
Price = 10 + 96 - 2.5 + 9.6 = ₹113.1 Lakhs
```

### Key Assumptions of Multiple Regression

| Assumption | Check Method | Solution if Violated |
|------------|--------------|---------------------|
| **Linearity** | Scatter plots, residual vs fitted | Transform variables, use non-linear models |
| **No Multicollinearity** | VIF < 10 | Remove/combine correlated predictors |
| **Homoscedasticity** | Residuals vs fitted plot | Robust regression, transform variables |
| **Independence of Errors** | Durbin-Watson test | Time-series models (ARIMA) |
| **Normality of Residuals** | Q-Q plot, Shapiro-Wilk | Transform dependent variable |
| **No Endogeneity** | Domain knowledge | Include all relevant variables |

**Variance Inflation Factor (VIF):**
```
          1
VIF = ─────────
      1 - R²ⱼ

Interpretation:
VIF = 1    : No multicollinearity
VIF < 5    : Acceptable
VIF > 10   : Problematic
```

---

## 2.5 REGRESSION TO THE MEAN

### Definition

**Regression to the Mean (RTM)** is the statistical tendency for **extreme measurements** to move **closer to the average** on subsequent measurement, purely due to **random variation** — NOT because of any real change.

### Why It Happens

```
┌─────────────────────────────────────────┐
│         MEASUREMENT COMPOSITION         │
├─────────────────────────────────────────┤
│                                         │
│  Observed Score = True Score + Error   │
│                                         │
│  Example:                              │
│  Exam Score = Actual Knowledge + Luck  │
│                                         │
│  Extreme HIGH score:                   │
│  → High knowledge + Unusually good luck│
│                                         │
│  Next attempt:                         │
│  → High knowledge + Normal luck        │
│  → Score moves closer to true ability  │
└─────────────────────────────────────────┘
```

### Mathematical Formula

```
E[Y₂ | Y₁] = μ + ρ × (Y₁ - μ)

Where:
E[Y₂ | Y₁] = Expected 2nd measurement given 1st
μ          = Population mean
ρ (rho)    = Correlation between measurements (0 to 1)
Y₁ - μ     = Deviation from mean
```

**Key Insight:** The further Y₁ is from the mean AND the weaker the correlation, the stronger the RTM effect.

### Real-World Examples

| Domain | Scenario | RTM Explanation | Common Mistake |
|--------|----------|----------------|----------------|
| **Sports** | Record-breaking debut season | True ability + exceptional luck | Blame "sophomore slump" on pressure |
| **Medicine** | High BP patients improve | Extreme reading + measurement error | Credit treatment without control group |
| **Education** | Low-scoring students improve | True ability + bad luck/anxiety | Attribute all gain to tutoring |
| **Finance** | Top funds underperform next year | Skill + exceptional luck | Assume strategy change needed |

### Visualizing RTM

```
Attempt 1 Scores          Attempt 2 Scores (regressed)
● Extreme HIGH  →         ● Closer to mean
│
│
●                     ●
│
│                     │
─────┼───── Mean ──────────┼─────
│                     │
│
●                     ●
│
│
● Extreme LOW   →         ● Closer to mean

What's Happening:
✓ Extreme HIGH scorers tend to score LOWER next time
✓ Extreme LOW scorers tend to score HIGHER next time
✓ Average scorers stay near average
✓ Purely due to random variation - NOT improvement/decline!
```

### How to Avoid RTM Fallacy

```
┌─────────────────────────────────────────┐
│         PROPER EXPERIMENTAL DESIGN      │
├─────────────────────────────────────────┤
│                                         │
│  Treatment Group:                      │
│  Low scorers → Tutoring → Test again  │
│                                         │
│  Control Group:                        │
│  Low scorers → No tutoring → Test again│
│                                         │
│  Compare:                              │
│  (Treatment improvement) -             │
│  (Control improvement)                 │
│  = TRUE tutoring effect                │
│                                         │
│  The control group accounts for RTM!   │
└─────────────────────────────────────────┘
```

**Solutions:**
✅ Always include a **control group**
✅ Use **randomized controlled trials**
✅ Take **multiple baseline measurements**
✅ Understand that RTM exists and question extreme-to-moderate changes

---

# 📖 MODULE 3: PYTHON LIBRARIES FOR DATA WRANGLING

## 3.1 NUMPY BASICS

### Why NumPy Over Python Lists?

| Feature | NumPy Array | Python List |
|---------|-------------|-------------|
| **Data Type** | Homogeneous (single type) | Heterogeneous (mixed) |
| **Memory** | Compact, efficient | Extra overhead per element |
| **Speed** | Orders of magnitude faster | Slower (Python loops) |
| **Operations** | Vectorized (element-wise) | Requires explicit loops |
| **Functionality** | Built-in math functions | Limited |

### Creating NumPy Arrays

```python
import numpy as np

# From a list
arr1 = np.array([1, 2, 3, 4, 5])

# 2D array (matrix)
arr2 = np.array([[1, 2, 3],
                 [4, 5, 6]])

# Special arrays
zeros = np.zeros((3, 4))           # 3×4 array of zeros
ones = np.ones((2, 3))             # 2×3 array of ones
range_arr = np.arange(0, 10, 2)    # [0, 2, 4, 6, 8]
linspace_arr = np.linspace(0, 1, 5) # [0, 0.25, 0.5, 0.75, 1]
random_arr = np.random.randn(3, 3)  # 3×3 normal distribution
```

### Array Attributes

```python
import numpy as np
np.random.seed(0)

x1 = np.random.randint(10, size=5)        # 1D array
x2 = np.random.randint(10, size=(2, 4))   # 2D array
x3 = np.random.randint(10, size=(3, 4, 5))# 3D array

print("x3 ndim:", x3.ndim)      # → 3 (dimensions)
print("x3 shape:", x3.shape)    # → (3, 4, 5) (size per dimension)
print("x3 size:", x3.size)      # → 60 (total elements)
print("x3 dtype:", x3.dtype)    # → int64 (data type)
print("itemsize:", x3.itemsize) # → 8 bytes per element
print("nbytes:", x3.nbytes)     # → 480 bytes total
```

**ASCII Visualization of Dimensions:**
```
1D Array          2D Array (Matrix)      3D Array (Depth)
+---+            +---+---+---+---+       /---+---+---+---+
| 0 |            |0,0|0,1|0,2|0,3|      / / / / /
+---+            +---+---+---+---+     / / / / /
| 1 |            |1,0|1,1|1,2|1,3|    / / / / /
+---+            +---+---+---+---+   / / / / /
| 2 |                              / / / / /
+---+                             / / / / /
/ / / / /
+---+---+---+---+
```

### Array Indexing - Accessing Single Elements

```python
import numpy as np

# 1D indexing
x1 = np.array([5, 0, 3, 3, 7, 9])
x1[0]    # → 5 (first element)
x1[-1]   # → 9 (last element, negative index)
x1[-2]   # → 7 (second from last)

# 2D indexing (comma-separated tuple)
x2 = np.array([[3, 5, 2, 4],
               [7, 6, 8, 8],
               [1, 6, 7, 7]])
x2[0, 0]   # → 3 (row 0, col 0)
x2[2, 0]   # → 1 (row 2, col 0)
x2[2, -1]  # → 7 (row 2, last col)

# 3D indexing
arr = np.array([[[1, 2, 3], [4, 5, 6]],
                [[7, 8, 9], [10, 11, 12]]])
print(arr[0, 1, 2])  # → 6
```

### Array Slicing - Accessing Subarrays

**Syntax:** `x[start:stop:step]`

```python
import numpy as np
x = np.arange(10)  # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

x[:5]      # → [0, 1, 2, 3, 4] (first 5)
x[5:]      # → [5, 6, 7, 8, 9] (from index 5)
x[4:7]     # → [4, 5, 6] (middle subarray)
x[::2]     # → [0, 2, 4, 6, 8] (every other element)
x[1::2]    # → [1, 3, 5, 7, 9] (every other, starting from 1)
x[::-1]    # → [9, 8, 7, 6, 5, 4, 3, 2, 1, 0] (reversed)

# Multi-dimensional slicing
x2 = np.array([[20, 5, 2, 4],
               [7, 6, 8, 8],
               [1, 6, 7, 7]])
x2[:2, :3]    # First 2 rows, first 3 cols
x2[:3, ::2]   # All rows, every other column
x2[:, 0]      # All rows, col 0 → [20, 7, 1]
x2[0, :]      # Row 0, all cols → [20, 5, 2, 4]
```

### Reshaping, Concatenation, and Splitting

```python
import numpy as np

# RESHAPING
grid = np.arange(1, 10).reshape((3, 3))
# → [[1, 2, 3],
#    [4, 5, 6],
#    [7, 8, 9]]

x = np.array([1, 2, 3])
x.reshape((1, 3))  # row vector: [[1, 2, 3]]
x.reshape((3, 1))  # column vector: [[1], [2], [3]]

# CONCATENATION
y = np.array([3, 2, 1])
np.concatenate([x, y])  # → [1, 2, 3, 3, 2, 1]

grid2 = np.array([[1, 2, 3],
                  [4, 5, 6]])
np.concatenate([grid2, grid2])        # Vertical (axis=0)
np.concatenate([grid2, grid2], axis=1)  # Horizontal (axis=1)

np.vstack([x, grid2])   # Vertical stack
np.hstack([grid2, grid2])  # Horizontal stack

# SPLITTING
arr = np.arange(8)  # [0, 1, 2, 3, 4, 5, 6, 7]
x1, x2, x3 = np.split(arr, [3, 5])
# x1 = [0, 1, 2], x2 = [3, 4], x3 = [5, 6, 7]

np.vsplit(grid2, 2)  # Vertical split
np.hsplit(grid2, 3)  # Horizontal split
```

---

## 3.2 NUMPY AGGREGATIONS & UNIVERSAL FUNCTIONS

### Aggregation Functions

```python
import numpy as np
L = np.random.random(100)  # 100 random numbers

# Basic aggregations
np.sum(L)      # Sum of all elements
np.min(L)      # Minimum value
np.max(L)      # Maximum value
np.mean(L)     # Mean (average)
np.std(L)      # Standard deviation
np.var(L)      # Variance
np.median(L)   # Median

# Other useful aggregations
np.prod(L)              # Product of all elements
np.argmin(L)            # Index of minimum value
np.argmax(L)            # Index of maximum value
np.percentile(L, 25)    # 25th percentile

# Boolean aggregations
np.any(L > 0.5)  # True if ANY element > 0.5
np.all(L > 0)    # True if ALL elements > 0

# Multi-dimensional aggregations
M = np.random.random((3, 4))
M.min(axis=0)  # Min of each column
M.max(axis=1)  # Max of each row
M.mean(axis=0) # Mean of each column
```

**Key Difference:**
- **Aggregations** reduce dimensions (return fewer values)
- **UFuncs** maintain same shape (element-wise operations)

### Universal Functions (UFuncs)

**Arithmetic UFuncs:**
```python
import numpy as np
x = np.array([1, 2, 3, 4])

x + 5          # np.add(x, 5)       → [6, 7, 8, 9]
x - 2          # np.subtract(x, 2)  → [-1, 0, 1, 2]
x * 3          # np.multiply(x, 3)  → [3, 6, 9, 12]
x / 2          # np.divide(x, 2)    → [0.5, 1.0, 1.5, 2.0]
x // 2         # np.floor_divide()  → [0, 1, 1, 2]
x ** 2         # np.power(x, 2)     → [1, 4, 9, 16]
x % 2          # np.mod(x, 2)       → [1, 0, 1, 0]
-x             # np.negative(x)     → [-1, -2, -3, -4]
```

### Trigonometric Functions

**⚠️ Important:** Angles must be in **RADIANS**!

```python
import numpy as np

# Convert degrees to radians
Arr = np.array([0, 30, 60, 90])
arr = Arr * np.pi / 180  # Convert to radians

# Basic trig
np.sin(arr)   # → [0.0, 0.5, 0.866, 1.0]
np.cos(arr)   # → [1.0, 0.866, 0.5, 0.0]
np.tan(arr)   # → [0.0, 0.577, 1.732, ∞]

# Inverse trig
np.arcsin(arr)
np.arccos(arr)
np.arctan(arr)

# Hyperbolic
np.sinh(arr)
np.cosh(arr)
np.tanh(arr)

# Conversion
np.deg2rad(Arr)  # Degrees → Radians
np.rad2deg(arr)  # Radians → Degrees
```

### Exponents and Logarithms

```python
import numpy as np
x = np.array([1, 2, 4, 10])

# Exponents
np.exp(x)        # e^x
np.exp2(x)       # 2^x
np.power(3, x)   # 3^x

# Logarithms
np.log(x)    # Natural log (ln)
np.log2(x)   # Base-2 log
np.log10(x)  # Base-10 log
```

### Other Mathematical Functions

```python
import numpy as np

# Rounding
arr = np.array([3.14159, 2.71828])
np.around(arr, 3)  # Round to 3 decimals → [3.142, 2.718]
np.floor(arr)      # Round down → [3., 2.]
np.ceil(arr)       # Round up → [4., 3.]

# Absolute values
np.abs(np.array([-2, -1, 0, 1, 2]))  # → [2, 1, 0, 1, 2]
```

---

## 3.3 COMPARISONS, MASKS & BOOLEAN LOGIC

### Comparison Operators

Comparison operators return **boolean arrays** (True/False per element).

```python
import numpy as np
a = np.reshape(np.arange(16), (4, 4))
# → [[ 0,  1,  2,  3],
#    [ 4,  5,  6,  7],
#    [ 8,  9, 10, 11],
#    [12, 13, 14, 15]]

# Comparison returns boolean array
large_values = (a > 10)
# → [[False, False, False, False],
#    [False, False, False, False],
#    [False, False, False,  True],
#    [ True,  True,  True,  True]]

# Boolean operators
np.equal(a, 5)        # == element-wise
np.not_equal(a, 5)    # !=
np.less(a, 5)         # <
np.less_equal(a, 5)   # <=
np.greater(a, 5)      # >
np.greater_equal(a, 5)# >=
```

### Logical Operators on Boolean Arrays

```python
import numpy as np
a = np.arange(16)

# NOT (negation)
~(a > 10)

# AND
(a > 5) & (a < 12)

# OR
(a < 5) | (a > 12)

# XOR
(a < 5) ^ (a > 12)
```

### Boolean Masking

**Masking** means extracting, modifying, counting, or manipulating values based on some criterion.

```python
import numpy as np
data = np.array([15, 42, 8, 73, 29, 55, 3, 90])

# Create a boolean mask
mask = data > 30
# mask → [False, True, False, True, False, True, False, True]

# Apply the mask to filter values
filtered = data[mask]
# filtered → [42, 73, 55, 90]

# Combined condition (values between 20 and 60)
filtered2 = data[(data > 20) & (data < 60)]
# filtered2 → [42, 29, 55]

# Count elements meeting condition
count = np.sum(data > 30)  # → 4

# Extract all even elements
even_values = (a % 2 == 0)
print(a[even_values])  # All even elements
```

**💡 Important Tip:** Always wrap compound conditions in parentheses:
```python
# Correct:
a[(a > 2) & (a < 5)]

# Wrong:
a[a > 2 & a < 5]  # Error!
```

---

## 3.4 FANCY INDEXING & STRUCTURED ARRAYS

### Fancy Indexing

**Definition:** Indexing an array with another NumPy array, a Python list, or a sequence of integers whose values select elements.

```python
import numpy as np
A = np.linspace(0, 1, 11)
# → [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]

# Using another array to index
print(A[np.array([0, 2, 4])])  # → [0.0, 0.2, 0.4]

# Using a list to index
print(A[[0, 2, 4]])  # → [0.0, 0.2, 0.4]

# More complex example
arr = np.array([10, 20, 30, 40, 50, 60, 70, 80])
# Select elements at indices 0, 3, and 6
print(arr[[0, 3, 6]])  # → [10, 40, 70]

# Using a NumPy index array
indices = np.array([1, 4, 7])
print(arr[indices])  # → [20, 50, 80]

# 2D fancy indexing
B = np.array([[1, 2, 3],
              [4, 5, 6],
              [7, 8, 9]])
print(B[[0, 2], [1, 2]])  # → [2, 9]
# (row 0 col 1, row 2 col 2)
```

**⚠️ Important Note:**
```python
# Fancy indexing returns a COPY
a = np.array([1, 2, 3, 4, 5])
b = a[[0, 1, 2]]
b[0] = 99
print(a)  # [1 2 3 4 5] - Original unchanged!

# Slicing returns a VIEW
c = a[0:3]
c[0] = 99
print(a)  # [99 2 3 4 5] - Original changed!
```

### Structured Arrays

**Definition:** Unlike regular NumPy arrays (homogeneous), structured arrays allow **different data types in each column** using a dtype definition.

**Method 1: Dictionary**
```python
import numpy as np
dtype = np.dtype({
    'names': ('name', 'age', 'weight'),
    'formats': ('U10', 'i4', 'f8')
})
data = np.array([('Alice', 25, 55.0),
                 ('Bob', 30, 75.5)], dtype=dtype)
print(data['name'])   # → ['Alice' 'Bob']
print(data['age'])    # → [25 30]
print(data['weight']) # → [55.0 75.5]
```

**Method 2: List of Tuples**
```python
dtype2 = np.dtype([('name', 'U10'),
                   ('age', 'i4'),
                   ('weight', 'f8')])
data2 = np.array([('Alice', 25, 55.0),
                  ('Bob', 30, 75.5)], dtype=dtype2)
```

**NumPy Type Codes:**
| Code | Type |
|------|------|
| **U** | Unicode string |
| **i** | Signed integer |
| **f** | Float |
| **b** | Boolean |
| **u** | Unsigned integer |
| **c** | Complex |
| **m** | Timedelta |
| **M** | Datetime |

---

## 3.5 PANDAS: SERIES & DATAFRAME

### Introduction to Pandas

**Pandas** is a high-level data manipulation tool built on NumPy.

**Key Data Structures:**

```
Series (1D):              DataFrame (2D):
+-------+-------+         +-------+-------+-------+
| Index | Value |         | Index | Col A | Col B |
+-------+-------+         +-------+-------+-------+
|   0   | val_0 |         |   0   |   1   |   2   |
+-------+-------+         +-------+-------+-------+
|   1   | val_1 |         |   1   |   3   |   4   |
+-------+-------+         +-------+-------+-------+
|   2   | val_2 |         |   2   |   5   |   6   |
+-------+-------+         +-------+-------+-------+
```

### Pandas Series

**Creating Series:**
```python
import pandas as pd
import numpy as np

# Method 1: From a list
data = pd.Series([0.25, 0.5, 0.75])

# Method 2: With explicit index
data = pd.Series([0.25, 0.5, 0.75], index=['a', 'b', 'c'])
print(data['b'])  # → 0.5

# Method 3: From NumPy array
arr = np.array([10, 20, 30])
series = pd.Series(arr)

# Method 4: From dictionary
dict_data = {'one': 1, 'two': 2, 'three': 3}
s = pd.Series(dict_data)
```

**Key Series Methods:**
```python
s.head(3)           # First 3 rows
s.tail(3)           # Last 3 rows
s.sort_values()     # Sort by values
s.sort_index()      # Sort by index
s.size              # Number of elements
s.is_unique         # True if all values unique
s.idxmax()          # Index of maximum value
s.describe()        # Statistical summary
```

### Pandas DataFrame

**Creating DataFrame:**
```python
import pandas as pd

# Method 1: From dictionary of lists
raw_data = {
    'firstname': ['Rupa', 'Rakshita', 'Rupal'],
    'lastname': ['deri', 'Mani', 'deri'],
    'RNO': [12, 22, 12],
    'Testscore': [12, 22, 12]
}
df = pd.DataFrame(raw_data)

# Method 2: Drop duplicates
df.drop_duplicates()  # Removes duplicate rows

# Method 3: From nested dictionary
scottish_hills = {
    'Ben Nevis': (1345, 5),
    'Ben Macdui': (1405, 5)
}
dataframe = pd.DataFrame(scottish_hills)
```

**Essential DataFrame Methods:**
```python
df.head(n)        # First n rows
df.tail(n)        # Last n rows
df.info()         # Column types & NaN count
df.describe()     # Summary statistics
df.shape          # (rows, columns)
df.dtypes         # Column data types
df.isnull()       # Find missing values
df.columns        # Column names
df.index          # Row indices
```

---

## 3.6 DATA INDEXING AND SELECTION IN PANDAS

### Label-Based Indexing (.loc)

**Accesses data by row and column labels.**

```python
import pandas as pd
df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Carol', 'David'],
    'Dept': ['Sales', 'IT', 'Sales', 'IT'],
    'Salary': [50000, 75000, 48000, 82000],
    'Experience': [3, 7, 2, 9]
})

# Select single row by label
print(df.loc[0])

# Select range of rows and columns
print(df.loc[0:2, 'Name':'Salary'])

# Select specific rows and columns
print(df.loc[[0, 2], ['Name', 'Salary']])
```

### Position-Based Indexing (.iloc)

**Accesses data by integer position (0-based indexing).**

```python
# Select first row by position
print(df.iloc[0])

# Select first 2 rows, first 3 columns
print(df.iloc[0:2, 0:3])

# Select last row
print(df.iloc[-1])

# Select specific positions
print(df.iloc[[0, 3], [1, 3]])
```

### Boolean Indexing

**Filter rows based on conditions.**

```python
# Filter: Sales department with salary > 45000
result = df[(df['Dept'] == 'Sales') & (df['Salary'] > 45000)]

# Filter: Experience > 5 OR Salary > 70000
result2 = df[(df['Experience'] > 5) | (df['Salary'] > 70000)]

# Filter: Salary between 50000 and 80000
result3 = df[df['Salary'].between(50000, 80000)]
```

### Fast Scalar Access (.at and .iat)

```python
# .at uses label (faster for single value)
df.at[0, 'Name']  # → 'Alice'

# .iat uses position (faster for single value)
df.iat[2, 1]  # → 35

# Comparison:
# .loc/.iloc - Label/Position based, can select multiple
# .at/.iat   - Label/Position based, single value only (faster)
```

---

## 3.7 OPERATING ON DATA

### Vectorized Operations

**Perform operations on entire columns without loops.**

```python
import pandas as pd

df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Carol'],
    'Age': [25, 30, 35],
    'Score': [88, 92, 79]
})

# Vectorized multiplication
df['Score2'] = df['Score'] * 2
# Output: [176, 184, 158]

# Vectorized addition
df['Bonus'] = df['Score'] + 10
# Output: [98, 102, 89]

# Element-wise operations between columns
df['Age_Score_Ratio'] = df['Age'] / df['Score']
```

### apply() Function

**Apply any function row-wise or column-wise.**

```python
# Apply to Series
df['Grade'] = df['Score'].apply(
    lambda x: 'A' if x >= 90 else 'B'
)

# Apply to DataFrame
def normalize(col):
    return (col - col.mean()) / col.std()

df[['Age', 'Score']].apply(normalize)

# Apply row-wise
df.apply(lambda row: row['Age'] + row['Score'], axis=1)
```

### map() and applymap()

```python
# map() - Element-wise on Series
df['Name'] = df['Name'].map(str.upper)  # → ['ALICE', 'BOB', 'CAROL']

# Using dictionary mapping
grade_map = {'A': 4, 'B': 3, 'C': 2}
df['Grade_Point'] = df['Grade'].map(grade_map)

# applymap() - Element-wise on DataFrame (deprecated in newer pandas)
df[['Age', 'Score']].applymap(lambda x: round(x, 2))
# Use DataFrame.map() instead in newer versions
```

### NumPy ufuncs on DataFrames

```python
import numpy as np

# Square root
df['Sqrt_Score'] = np.sqrt(df['Score'])

# Logarithm
df['Log_Score'] = np.log(df['Score'])

# Exponential
df['Exp_Age'] = np.exp(df['Age'] / 10)

# Trigonometric
df['Sin_Score'] = np.sin(df['Score'])
```

---

## 3.8 MISSING DATA HANDLING

### Understanding Missing Data

**Missing values in Pandas are marked as NaN (Not a Number).**

```python
import pandas as pd
import numpy as np

df = pd.DataFrame({
    'A': [1, 2, np.nan, 4],
    'B': [5, np.nan, 7, 8],
    'C': [10, 11, 12, 13]
})
```

### Detecting Missing Values

```python
# Check for missing values (returns boolean DataFrame)
df.isnull()

# Count missing values per column
df.isnull().sum()
# Output:
# A    1
# B    1
# C    0

# Total missing values
df.isnull().sum().sum()  # → 2

# Check for non-null values
df.notnull()
```

### Methods to Handle Missing Data

| Method | When to Use | Example |
|--------|-------------|---------|
| **Forward Fill (ffill)** | Time-series data | Stock prices, temperature |
| **Backward Fill (bfill)** | Time-series with future data | Forecasting models |
| **Mean/Median Fill** | Numerical continuous data | Age, income, test scores |
| **Mode Fill** | Categorical data | Gender, city, product category |
| **Drop Rows** | When missing data is minimal (<5%) | Small datasets |
| **Drop Columns** | When column has too many missing (>50%) | Irrelevant features |

**Code Examples:**
```python
# Fill with constant value
df.fillna(0)

# Forward fill
df.fillna(method='ffill')  # or df.fillna(method='pad')

# Backward fill
df.fillna(method='bfill')  # or df.fillna(method='backfill')

# Fill with column mean/median
df.fillna(df.mean())
df.fillna(df.median())

# Drop rows with NaN
df.dropna()                    # Drop any row with NaN
df.dropna(how='all')           # Drop only if ALL values are NaN
df.dropna(subset=['A'])        # Drop only if NaN in specific column

# Drop columns with NaN
df.dropna(axis=1)
```

### Interpolation (For Numerical Series)

```python
# Linear interpolation
df['B'].interpolate()

# Full interpolation
df.interpolate()

# Different methods
df.interpolate(method='linear')
df.interpolate(method='polynomial', order=2)
df.interpolate(method='time')
```

---

## 3.9 HIERARCHICAL INDEXING (MULTIINDEX)

### What is MultiIndex?

**Definition:** Enables storing and manipulating higher-dimensional data (3D, 4D) within standard 1D Series and 2D DataFrame structures.

**Purpose:**
- Organize data with multiple levels of categories
- Efficient grouping and aggregation
- Reshape data easily

### MultiIndexed Series

```python
import pandas as pd
import numpy as np

# Create MultiIndex Series
index = [
    ["Maths", "Maths", "Maths", "Science", "Science", "Science"],
    ["Test1", "Test2", "Test3", "Test1", "Test2", "Test3"]
]
data = pd.Series([85, 90, 88, 78, 82, 80], index=index)

print(data)
# Output:
# Maths    Test1    85
#          Test2    90
#          Test3    88
# Science  Test1    78
#          Test2    82
#          Test3    80

# Access data by outer index
print(data["Maths"])

# Access specific value
print(data["Maths"]["Test1"])  # → 85

# Partial slicing
print(data["Maths":"Science"])
```

**ASCII Visualization:**
```
MultiIndex Series Structure:
Outer Index (Subject) → Maths
↓
Inner Index (Test)   → Test1  Test2  Test3
↓      ↓      ↓
Values               →   85     90     88
```

### Unstack and Stack Operations

```python
# Unstack: Converts MultiIndex Series to 2D DataFrame
df = data.unstack()
print(df)
# Output:
#         Test1  Test2  Test3
# Maths      85     90     88
# Science    78     82     80

# Stack back to Series
df.stack()
```

### MultiIndexed DataFrame

```python
# Create MultiIndex DataFrame
arrays = [
    ['A', 'A', 'B', 'B'],
    [1, 2, 1, 2]
]
index = pd.MultiIndex.from_arrays(arrays, names=['Class', 'Exam'])
df = pd.DataFrame({
    'Python': [85, 90, 78, 82],
    'DS': [88, 92, 80, 85],
    'CA': [90, 88, 85, 87]
}, index=index)

print(df)
# Output:
#            Python   DS   CA
# Class Exam
# A     1        85   88   90
#       2        90   92   88
# B     1        78   80   85
#       2        82   85   87

# Sort by specific level
df.sort_index(level='Exam')

# Access by outer index
df.loc['A']

# Access by both indices
df.loc[('A', 1)]
```

### Practical Use Case: Student Exam Scores

```python
# MultiIndex: Outer = Subject, Inner = Test Number
index = [
    ["Maths", "Maths", "Science", "Science", "English", "English"],
    ["Test1", "Test2", "Test1", "Test2", "Test1", "Test2"]
]
scores = pd.Series([85, 90, 78, 88, 92, 87], index=index)

# Access all Maths scores
print(scores["Maths"])

# Access specific test
print(scores["Science"]["Test2"])  # → 88

# Convert to DataFrame for easier viewing
scores_df = scores.unstack()

# Calculate average per subject
subject_avg = scores.groupby(level=0).mean()
print(subject_avg)
# Output:
# English    89.5
# Maths      87.5
# Science    83.0
```

---

## 3.10 COMBINING DATASETS

### Three Ways to Unite DataFrames

```
1. concat()  - Stack vertically or side-by-side
2. merge()   - SQL-style joins on key columns
3. join()    - Index-based joining
```

### 1. pd.concat()

**Purpose:** Stack DataFrames **vertically** (axis=0) or **side-by-side** (axis=1).

```python
import pandas as pd

# Concatenate Series
ser1 = pd.Series(['A', 'B', 'C'], index=[1, 2, 3])
ser2 = pd.Series(['X', 'Y', 'Z'], index=[4, 5, 6])
result = pd.concat([ser1, ser2])

# Concatenate DataFrames (vertical - axis=0)
df1 = pd.DataFrame({'Language': ['Python', 'NumPy', 'Pandas']})
df2 = pd.DataFrame({'Language': ['C', 'C++', 'Java']})
df = pd.concat([df1, df2])

# Concatenate horizontally (axis=1)
df3 = pd.DataFrame({'A': [1, 2, 3]})
df4 = pd.DataFrame({'B': [4, 5, 6]})
df_horizontal = pd.concat([df3, df4], axis=1)
```

**Key Parameters:**
| Parameter | Description |
|-----------|-------------|
| `axis` | 0 (rows) or 1 (columns) |
| `ignore_index` | Reset index |
| `keys` | Add hierarchical index for identification |
| `join` | 'outer' (default) or 'inner' |

### 2. Append Method

```python
# Append one DataFrame to another
df1 = pd.DataFrame({'A': [1, 2], 'B': [3, 4]})
df2 = pd.DataFrame({'A': [5, 6], 'B': [7, 8]})
result = df1.append(df2, ignore_index=True)
# Output:
#    A  B
# 0  1  3
# 1  2  4
# 2  5  7
# 3  6  8

# ⚠️ Note: append() is deprecated in newer pandas
# Use pd.concat() instead
```

### 3. Merge/Join (SQL-style Joins)

```python
df1 = pd.DataFrame({
    'key': ['A', 'B', 'C'],
    'value1': [1, 2, 3]
})
df2 = pd.DataFrame({
    'key': ['A', 'B', 'D'],
    'value2': [4, 5, 6]
})

# Inner Join (only matching keys)
pd.merge(df1, df2, on='key', how='inner')
# Output:
#   key  value1  value2
# 0   A       1       4
# 1   B       2       5

# Left Join (all from left, matching from right)
pd.merge(df1, df2, on='key', how='left')
# Output:
#   key  value1  value2
# 0   A       1     4.0
# 1   B       2     5.0
# 2   C       3     NaN

# Right Join (all from right, matching from left)
pd.merge(df1, df2, on='key', how='right')

# Outer Join (all records from both)
pd.merge(df1, df2, on='key', how='outer')

# Different column names
df3 = pd.DataFrame({'EmpID': [2, 3], 'Score': [90, 85]})
pd.merge(df1, df3, left_on='key', right_on='EmpID')
```

**Comparison:**
```
merge()  - More flexible, SQL-like, join on columns
join()   - Simpler, index-based, shorthand for merge
concat() - Stacking, not relational joining
```

---

## 3.11 AGGREGATION AND GROUPBY

### GroupBy: Split-Apply-Combine Strategy

```
1. SPLIT:   Group rows by key
2. APPLY:   Aggregate/Transform each group
3. COMBINE: Merge results back
```

### Basic GroupBy Operations

```python
import pandas as pd

df = pd.DataFrame({
    'Dept': ['Sales', 'IT', 'Sales', 'IT', 'HR', 'HR'],
    'Salary': [50000, 75000, 48000, 82000, 52000, 55000],
    'Experience': [3, 7, 2, 9, 4, 6]
})

# Group by Department
grouped = df.groupby('Dept')

# Sum of salaries per department
print(grouped['Salary'].sum())
# Output:
# Dept
# HR     107000
# IT     157000
# Sales   98000

# Mean salary per department
print(grouped['Salary'].mean())

# Multiple aggregations
print(grouped['Salary'].agg(['mean', 'min', 'max', 'count']))

# Group by multiple columns
df2 = df.copy()
df2['Year'] = [2022, 2022, 2023, 2023, 2022, 2023]
print(df2.groupby(['Dept', 'Year'])['Salary'].sum())
```

### Common Aggregation Functions

| Function | Description | Example |
|----------|-------------|---------|
| `sum()` | Sum of values | `grouped['Salary'].sum()` |
| `mean()` | Average | `grouped['Salary'].mean()` |
| `min()` | Minimum value | `grouped['Salary'].min()` |
| `max()` | Maximum value | `grouped['Salary'].max()` |
| `count()` | Count non-null values | `grouped['Salary'].count()` |
| `std()` | Standard deviation | `grouped['Salary'].std()` |
| `var()` | Variance | `grouped['Salary'].var()` |
| `first()` | First value in group | `grouped['Salary'].first()` |
| `last()` | Last value in group | `grouped['Salary'].last()` |
| `size()` | Total count (including NaN) | `grouped.size()` |
| `describe()` | Statistical summary | `grouped['Salary'].describe()` |

### Transform and Filter

```python
# transform() - Return same shape
df['Dept_Avg_Salary'] = df.groupby('Dept')['Salary'].transform('mean')

# Standardize within groups
df['Salary_Z'] = df.groupby('Dept')['Salary'].transform(
    lambda x: (x - x.mean()) / x.std()
)

# filter() - Keep/drop groups
df.groupby('Dept').filter(lambda x: len(x) > 2)
df.groupby('Dept').filter(lambda x: x['Salary'].mean() > 60)
```

### Iterating Over Groups

```python
for name, group in df.groupby('Dept'):
    print(f"Department: {name}")
    print(group)
    print()
```

---

## 3.12 PIVOT TABLES

### What are Pivot Tables?

**Definition:** Reshape and summarize data from column-wise format into 2D tabular format for easy comparison across two dimensions.

**Purpose:**
- Cross-tabulation of data
- Multi-dimensional analysis
- Summarize large datasets

### pd.pivot_table() - Basic Syntax

```python
pd.pivot_table(df, 
               values='column_to_summarize',
               index='row_grouping',
               columns='column_grouping',
               aggfunc='aggregation_function')
```

**Example:**
```python
import pandas as pd

sales_data = pd.DataFrame({
    'Region': ['North', 'North', 'South', 'South', 'East', 'East'],
    'Product': ['A', 'B', 'A', 'B', 'A', 'B'],
    'Year': [2022, 2022, 2022, 2022, 2023, 2023],
    'Sales': [100, 200, 150, 250, 180, 220]
})

# Basic pivot table
pivot = pd.pivot_table(
    sales_data,
    index='Region',           # Rows
    columns='Product',        # Columns
    values='Sales',           # Values to aggregate
    aggfunc='sum'             # Aggregation function
)
print(pivot)
# Output:
# Product    A    B
# Region
# East     180  220
# North    100  200
# South    150  250
```

### Advanced Pivot Tables

**With Totals (Margins):**
```python
pivot_with_totals = pd.pivot_table(
    sales_data,
    index='Region',
    columns='Product',
    values='Sales',
    aggfunc='sum',
    margins=True,           # Add row/column totals
    margins_name='Total'    # Name for totals
)
```

**Multiple Aggregations:**
```python
pd.pivot_table(sales_data,
               index=['Region', 'Year'],
               values='Sales',
               aggfunc=['sum', 'mean'])
```

**Multiple Values:**
```python
pd.pivot_table(sales_data,
               values=['Sales', 'Quantity'],
               index='Region',
               columns='Product',
               aggfunc='sum')
```

### df.pivot() - Simple Reshape (No Aggregation)

```python
# Purpose: Simple reshape WITHOUT aggregation
# Requirements: Unique index-column combinations

df.pivot(index='Region',
         columns='Product',
         values='Sales')

# ⚠️ Error with duplicates:
# ValueError: Index contains duplicate entries
# → Use pivot_table instead!
```

### Pivot Table Parameters

| Parameter | Description |
|-----------|-------------|
| `values` | Column(s) to aggregate |
| `index` | Row grouping |
| `columns` | Column grouping |
| `aggfunc` | Aggregation function(s): 'mean', 'sum', 'count', etc. |
| `fill_value` | Replace NaN with value |
| `margins` | Add row/column totals (True/False) |
| `margins_name` | Label for totals ('All', 'Total') |

### Comparison: GroupBy vs Pivot Table

| Feature | GroupBy | Pivot Table |
|---------|---------|-------------|
| **Output Shape** | 1D Series or DataFrame | 2D cross-tabular format |
| **Best For** | Single-dimension grouping | Multi-dimensional comparison |
| **Flexibility** | More flexible aggregations | Easier visualization |
| **Syntax** | `df.groupby('col').agg()` | `pd.pivot_table()` |
| **Example** | Sales by Region | Sales by Region × Product |

---

# 📖 MODULE 4: DATA VISUALIZATION

## 4.1 IMPORTING MATPLOTLIB

### Introduction to Matplotlib

**Matplotlib** is the foundational plotting library for Python.

**Installation:**
```bash
pip install matplotlib
```

**Basic Import:**
```python
import matplotlib.pyplot as plt
import numpy as np
```

**Setting Style:**
```python
# Use predefined styles
plt.style.use('seaborn-v0_8')
plt.style.use('ggplot')
plt.style.use('fivethirtyeight')

# View available styles
print(plt.style.available)
```

### Basic Plot Structure

```python
# Create figure and axes
fig, ax = plt.subplots()

# Plot data
ax.plot(x, y)

# Customize
ax.set_xlabel('X Label')
ax.set_ylabel('Y Label')
ax.set_title('Title')

# Display
plt.show()
```

**Figure and Axes Hierarchy:**
```
Figure
└── The entire window/figure
    └── Axes
        └── The actual plot area
            ├── Data
            ├── Labels
            └── Legends
```

---

## 4.2 LINE PLOTS

### What is a Line Plot?

**Definition:** A line plot connects data points with straight lines.

**Best For:**
- ✅ Showing trends over time
- ✅ Continuous variables
- ✅ Time series data

### Basic Line Plot

```python
import matplotlib.pyplot as plt
import numpy as np

# Create data
x = np.linspace(0, 10, 100)
y = np.sin(x)

# Create plot
plt.figure(figsize=(8, 4))
plt.plot(x, y)
plt.title('Simple Line Plot')
plt.xlabel('X Value')
plt.ylabel('Y Value')
plt.grid(True)
plt.show()
```

### Key Parameters

```python
plt.plot(x, y,
         color='blue',        # Line color
         linestyle='-',       # Line style
         linewidth=2,         # Line width
         marker='o',          # Marker style
         markersize=5,        # Marker size
         label='sin(x)')      # Legend label
```

**Line Styles:**
```
'-'   - Solid (default)
'--'  - Dashed
':'   - Dotted
'-.'  - Dash-dot
```

**Marker Styles:**
```
'o'   - Circle    's'   - Square    '^'   - Triangle up
'v'   - Triangle down  'D'   - Diamond   '*'   - Star
'+'   - Plus     'x'   - X
```

### Multiple Lines

```python
x = np.linspace(0, 4*np.pi, 200)

plt.figure(figsize=(8, 4))

# Plot multiple lines
plt.plot(x, np.sin(x),
         color='blue', linestyle='-', linewidth=2, label='sin(x)')

plt.plot(x, np.cos(x),
         color='red', linestyle='--', linewidth=2, label='cos(x)')

plt.plot(x, np.sin(x)*np.exp(-x/10),
         color='green', linewidth=2, linestyle=':', label='damped sin')

# Add labels and legend
plt.title('Line Plot Example')
plt.xlabel('x')
plt.ylabel('y')
plt.legend()
plt.grid(True, alpha=0.4)
plt.tight_layout()
plt.show()
```

### Saving Figures

```python
plt.savefig('myplot.png',
            dpi=300,              # High resolution
            transparent=True,     # Transparent background
            bbox_inches='tight')  # Remove extra whitespace
```

---

## 4.3 SCATTER PLOTS

### What is a Scatter Plot?

**Definition:** Shows correlation between two numerical variables.

**Characteristics:**
- ✅ Each point = one observation
- ✅ X-axis = Independent variable
- ✅ Y-axis = Dependent variable
- ✅ Reveals relationships, clusters, outliers

### Basic Scatter Plot

```python
import matplotlib.pyplot as plt
import numpy as np

# Create data
x = np.random.rand(50)
y = np.random.rand(50)

# Create scatter plot
plt.figure(figsize=(6, 4))
plt.scatter(x, y)
plt.xlabel('X Variable')
plt.ylabel('Y Variable')
plt.title('Scatter Plot')
plt.show()
```

### Key Parameters

```python
plt.scatter(x, y,
            s=50,            # Marker size
            c='blue',        # Color
            alpha=0.75,      # Transparency
            marker='o',      # Marker shape
            edgecolors='white',  # Edge color
            linewidths=0.5,  # Edge width
            cmap='viridis')  # Colormap
```

### Scatter Plot with Groups

```python
fig, ax = plt.subplots(figsize=(6, 4))

# Create groups
colors = ['blue', 'red', 'green']
groups = ['Group A', 'Group B', 'Group C']

for i, (grp, col) in enumerate(zip(groups, colors)):
    x = np.random.randn(60) + i*2
    y = np.random.randn(60) + i
    
    ax.scatter(x, y,
               alpha=0.75, s=50, color=col,
               label=grp, edgecolors='white', lw=0.5)

ax.set_title('Scatter Plot — Groups')
ax.legend()
ax.set_xlabel('X')
ax.set_ylabel('Y')
plt.tight_layout()
plt.show()
```

### Color Mapping

```python
# Color by third variable
x = np.random.rand(100)
y = np.random.rand(100)
colors = np.random.rand(100)
sizes = 1000 * np.random.rand(100)

plt.scatter(x, y,
            c=colors, s=sizes,
            alpha=0.5, cmap='viridis')

plt.colorbar()  # Show color scale
plt.show()
```

### Adding Regression Line

```python
from scipy import stats

x = np.array([1, 2, 3, 4, 5])
y = np.array([2, 4, 5, 4, 5])

# Calculate regression
slope, intercept, r_value, p_value, std_err = stats.linregress(x, y)

# Create line
line = slope * x + intercept

# Plot
plt.scatter(x, y, label='Data')
plt.plot(x, line, 'r-', label=f'Fit: y={slope:.2f}x+{intercept:.2f}')
plt.legend()
plt.show()
```

---

## 4.4 VISUALIZING ERRORS

### Why Show Errors?

**Purpose:** Display uncertainty in measurements or predictions.

**Common Uses:**
- ✅ Experimental error bars
- ✅ Confidence intervals
- ✅ Standard deviation
- ✅ Standard error

### plt.errorbar()

```python
import matplotlib.pyplot as plt
import numpy as np

x = np.arange(1, 6)
y = np.array([2.1, 3.4, 2.8, 4.2, 3.7])
yerr = np.array([0.3, 0.5, 0.4, 0.6, 0.35])

plt.errorbar(x, y,
             yerr=yerr,       # Vertical errors
             fmt='-o',        # Format: line + marker
             color='blue',
             ecolor='lightblue',  # Error bar color
             capsize=5,       # Cap width
             lw=2,            # Line width
             elinewidth=2)    # Error bar width

plt.title('Error Bar Plot')
plt.xlabel('X')
plt.ylabel('Y ± Error')
plt.show()
```

### Parameters

```python
plt.errorbar(x, y,
             yerr=0.5,        # Constant error
             xerr=0.1,        # X errors
             fmt='o',         # Marker only
             capsize=5,       # End caps
             ecolor='red',    # Error color
             elinewidth=2,    # Error width
             alpha=0.5)       # Transparency
```

### Asymmetric Errors

```python
yerr_lower = [0.3, 0.4, 0.5, 0.3, 0.4]
yerr_upper = [0.5, 0.6, 0.4, 0.7, 0.5]

plt.errorbar(x, y,
             yerr=[yerr_lower, yerr_upper],
             fmt='-o')
```

### fill_between() - Confidence Bands

```python
x = np.linspace(0, 2*np.pi, 100)
y = np.sin(x)

plt.plot(x, y, 'b-', label='sin(x)')

# Fill confidence band
plt.fill_between(x,
                 y - 0.3,     # Lower bound
                 y + 0.3,     # Upper bound
                 alpha=0.25,
                 color='blue',
                 label='± 0.3 band')

plt.title('Confidence Interval')
plt.legend()
plt.show()
```

---

## 4.5 DENSITY AND CONTOUR PLOTS

### Kernel Density Estimation (KDE)

**Definition:** Smoothed probability density estimate.

**Purpose:**
- ✅ Show distribution shape
- ✅ Better than histogram for continuous data
- ✅ No binning artifacts

```python
from scipy.stats import gaussian_kde
import matplotlib.pyplot as plt
import numpy as np

# Generate data
data = np.random.randn(500)

# Calculate KDE
kde = gaussian_kde(data)
x = np.linspace(-4, 4, 200)

# Plot histogram and KDE
plt.hist(data, bins=25, density=True, alpha=0.4, label='Histogram')
plt.plot(x, kde(x), lw=2.5, label='KDE')

plt.legend()
plt.title('Density Estimation')
plt.show()
```

### Using Seaborn for KDE

```python
import seaborn as sns

# Simple KDE
sns.kdeplot(data, fill=True)

# Multiple distributions
sns.kdeplot(data1, label='Group 1')
sns.kdeplot(data2, label='Group 2')
plt.legend()
```

### Contour Plots

**Purpose:** Show 3D data in 2D using contour lines.

```python
import numpy as np
import matplotlib.pyplot as plt

def f(x, y):
    return np.sin(x)**10 + np.cos(10 + y * x) * np.cos(x)

x = np.linspace(0, 5, 50)
y = np.linspace(0, 5, 40)
X, Y = np.meshgrid(x, y)  # creates 2D coordinate arrays
Z = f(X, Y)

plt.style.use('seaborn-white')

# Line contour
plt.contour(X, Y, Z, colors='black')

# Filled contour
plt.contourf(X, Y, Z)

plt.show()
```

**ASCII Visualization:**
```
Contour Plot (Topographic Map):
Y
↑
┌───┼───┐
│ ╱ ╱ ╱ │  ← Contour lines
│╱ ╱ ╱ ╱│     (equal values)
│╲ ╲ ╲ ╲│
│ ╲ ╲ ╲ │
└───┼───┘
→ X
```

### Parameters

```python
plt.contourf(X, Y, Z,
             levels=20,       # Number of levels
             cmap='plasma',   # Colormap
             alpha=0.8)       # Transparency

# Add contour lines on top
plt.contour(X, Y, Z,
            levels=20,
            colors='black',
            linewidths=0.5,
            alpha=0.5)
```

---

## 4.6 HISTOGRAMS

### What is a Histogram?

**Definition:** Shows frequency distribution of a single variable.

**Characteristics:**
- ✅ Contiguous (touching) bars
- ✅ X-axis = Value ranges (bins)
- ✅ Y-axis = Frequency or density

### Basic Histogram

```python
import matplotlib.pyplot as plt
import numpy as np

data = np.random.normal(50, 15, 1000)

plt.hist(data,
         bins=20,           # Number of bins
         edgecolor='white', # Bar edges
         alpha=0.7)         # Transparency

plt.xlabel('Value')
plt.ylabel('Frequency')
plt.title('Histogram')
plt.show()
```

### Key Parameters

```python
plt.hist(data,
         bins=30,           # Number of bins or array
         range=(0, 100),    # Min/max range
         density=True,      # Probability density
         cumulative=False,  # Cumulative histogram
         histtype='bar',    # Type: 'bar', 'barstacked', 'step', 'stepfilled'
         orientation='horizontal',  # 'vertical' or 'horizontal'
         edgecolor='black',
         linewidth=1,
         alpha=0.7)
```

### Overlapping Histograms

```python
# Generate two datasets
scores_A = np.random.normal(60, 10, 300)
scores_B = np.random.normal(75, 8, 300)

plt.hist(scores_A,
         bins=20, alpha=0.65, color='blue',
         label='Class A', edgecolor='white')

plt.hist(scores_B,
         bins=20, alpha=0.65, color='red',
         label='Class B', edgecolor='white')

plt.xlabel('Score')
plt.ylabel('Frequency')
plt.legend()
plt.title('Comparison of Two Classes')
plt.show()
```

### 2D Histogram

```python
# Generate data
x = np.random.randn(1000)
y = np.random.randn(1000)

plt.hist2d(x, y, bins=30, cmap='Blues')

plt.colorbar(label='Count')
plt.xlabel('X')
plt.ylabel('Y')
plt.title('2D Histogram')
plt.show()
```

### Custom Bins

```python
# Define custom bin edges
bins = [0, 10, 20, 30, 50, 100]

plt.hist(data, bins=bins, edgecolor='black')
plt.xticks(bins)
plt.show()
```

### Normalized Histogram

```python
plt.hist(data, bins=20, density=True, alpha=0.6)

# Overlay normal distribution
from scipy.stats import norm
x = np.linspace(min(data), max(data), 100)
plt.plot(x, norm.pdf(x, np.mean(data), np.std(data)),
         'r-', linewidth=2)
```

---

## 4.7 LEGENDS, COLORS & CUSTOMIZATION

### Legends

```python
# Basic legend
plt.plot(x, y1, label='Line 1')
plt.plot(x, y2, label='Line 2')
plt.legend()

# Legend parameters
plt.legend(loc='best',        # Location
           fontsize=12,       # Font size
           framealpha=0.9,    # Frame transparency
           fancybox=True,     # Rounded corners
           shadow=True,       # Shadow
           title='Legend',    # Title
           ncol=2,           # Number of columns
           frameon=True)     # Show frame
```

**Location Options:**
```
'best'=0, 'upper right'=1, 'upper left'=2, 'lower left'=3,
'lower right'=4, 'right'=5, 'center left'=6, 'center right'=7,
'lower center'=8, 'upper center'=9, 'center'=10
```

### Color Specifications

**Named Colors:**
```python
plt.plot(x, y, color='red')
plt.plot(x, y, color='blue')
plt.plot(x, y, color='green')
```

**Hex Colors:**
```python
plt.plot(x, y, color='#2563EB')   # Blue
plt.plot(x, y, color='#DC2626')   # Red
```

**RGB/RGBA:**
```python
plt.plot(x, y, color=(0.3, 0.6, 0.9))      # RGB (0-1)
plt.plot(x, y, color=(0.3, 0.6, 0.9, 0.7)) # RGBA (with alpha)
```

### Colormaps

| Type | Examples | Use Case |
|------|----------|----------|
| **Sequential** | 'viridis', 'plasma', 'inferno', 'Blues' | Light to dark progression |
| **Diverging** | 'coolwarm', 'Seismic', 'RdBu' | Two-color comparison |
| **Qualitative** | 'Set1', 'Set2', 'tab10', 'tab20' | Distinct categories |

```python
# Scatter plot with colormap
plt.scatter(x, y, c=values, cmap='viridis')
plt.colorbar(label='Value')

# Heatmap
plt.imshow(data, cmap='plasma', aspect='auto')
plt.colorbar()
```

### Customization

```python
# rcParams - Global Settings
import matplotlib as mpl
plt.rcParams['font.size'] = 14
plt.rcParams['axes.facecolor'] = 'white'
plt.rcParams['figure.figsize'] = (10, 6)

# Spines Customization
ax.spines['top'].set_visible(False)
ax.spines['right'].set_visible(False)
ax.spines['bottom'].set_position('zero')

# Ticks Customization
plt.xticks([0, 2, 4, 6, 8, 10])
plt.xticks([0, 1, 2], ['A', 'B', 'C'])
ax.tick_params(labelsize=12, length=6, width=2)
plt.xticks(rotation=45, ha='right')
```

---

## 4.8 SUBPLOTS & ANNOTATIONS

### Multiple Subplots

```python
# Create 2x2 grid
fig, axes = plt.subplots(2, 2, figsize=(10, 6))

# Access individual axes
axes[0, 0].plot(x, np.sin(x))
axes[0, 0].set_title('Sin')

axes[0, 1].scatter(x, y, s=20, alpha=0.7)
axes[0, 1].set_title('Scatter')

axes[1, 0].bar(['A', 'B', 'C'], [3, 5, 4])
axes[1, 0].set_title('Bar')

axes[1, 1].hist(data, bins=20)
axes[1, 1].set_title('Histogram')

plt.tight_layout()
plt.show()
```

**ASCII Visualization:**
```
Subplot Grid (2 rows × 3 cols):
┌─────┬─────┬─────┐
│  1  │  2  │  3  │
├──────────┼─────┤
│  4  │  5  │  6  │
└─────┴─────┴─────┘
```

### Parameters

```python
plt.subplots(nrows=2,
             ncols=2,
             figsize=(10, 6),
             sharex=True,      # Share x-axis
             sharey=True,      # Share y-axis
             squeeze=False)    # Keep 2D array
```

### Text and Annotation

```python
# ax.text() - Place text at coordinates
ax.text(0.2, -0.9, 'sin(x) function',
        fontsize=9, style='italic',
        bbox=dict(boxstyle='round', facecolor='lightyellow'))

# ax.annotate() - Text with Arrow
idx = np.argmax(np.sin(x))
ax.annotate('Maximum',
            xy=(x[idx], np.sin(x[idx])),    # Point to annotate
            xytext=(x[idx]+0.8, 0.6),       # Text position
            arrowprops=dict(                # Arrow style
                facecolor='black',
                shrink=0.05,
                width=2,
                headwidth=8))
```

**Arrow Styles:**
```
'-'   - Simple line    '->'  - Simple arrow
'-['  - Bracket        '-|>' - Filled arrow
'fancy' - Fancy arrow
```

---

## 4.9 THREE-DIMENSIONAL PLOTTING

### Introduction to 3D Plots

```python
from mpl_toolkits.mplot3d import Axes3D
import matplotlib.pyplot as plt
import numpy as np
```

### 3D Surface Plot

```python
fig = plt.figure(figsize=(8, 4))
ax = fig.add_subplot(111, projection='3d')

# Create data
u = v = np.linspace(-3, 3, 50)
X, Y = np.meshgrid(u, v)
Z = np.sin(np.sqrt(X**2 + Y**2))

# Plot surface
ax.plot_surface(X, Y, Z,
                cmap='viridis',
                alpha=0.85,
                edgecolor='none')

ax.set_title('3D Surface Plot')
plt.show()
```

### Parameters

```python
ax.plot_surface(X, Y, Z,
                cmap='plasma',     # Colormap
                alpha=0.9,         # Transparency
                rstride=1,         # Row step
                cstride=1,         # Column step
                linewidth=0,       # Edge width
                antialiased=True)  # Smoothing
```

### 3D Scatter Plot

```python
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

# Generate data
xs = np.random.rand(100)
ys = np.random.rand(100)
zs = np.random.rand(100)
colors = np.random.rand(100)

ax.scatter(xs, ys, zs,
           c=colors, cmap='viridis',
           marker='o', s=50, alpha=0.6)

ax.set_xlabel('X')
ax.set_ylabel('Y')
ax.set_zlabel('Z')
plt.show()
```

### View Angle

```python
# Set viewing angle
ax.view_init(elev=30,    # Elevation
             azim=45)    # Azimuth

# Interactive rotation
# Click and drag in interactive mode
```

**ASCII Visualization:**
```
3D Scatter Plot:
Z
↑
/|\
/ | \
/  |  \
/   |   \
/    ●    \
/   ●   ●   \
/ ●         ● \
└───────────────→ Y
/
/
X
```

---

## 4.10 GEOGRAPHIC DATA WITH BASEMAP

### Introduction to Basemap

**⚠️ Note:** Basemap is deprecated. Use Cartopy for new projects.

**Installation:**
```bash
pip install basemap
```

### Basic Map

```python
from mpl_toolkits.basemap import Basemap
import matplotlib.pyplot as plt

# Create figure
fig = plt.figure(figsize=(10, 6))

# Setup Basemap
m = Basemap(projection='mill',
            llcrnrlat=-60, urcrnrlat=80,
            llcrnrlon=-180, urcrnrlon=180)

# Draw features
m.drawcoastlines(linewidth=0.8)
m.drawcountries(linewidth=0.5)
m.fillcontinents(color='lightgreen', lake_color='lightblue')
m.drawmapboundary(fill_color='lightblue')

# Draw grid
m.drawparallels(range(-60, 80, 30))
m.drawmeridians(range(-180, 180, 60))

plt.title('World Map')
plt.show()
```

### Projections

```
'mill'      - Miller cylindrical
'robin'     - Robinson
'ortho'     - Orthographic (globe view)
'merc'      - Mercator
'cyl'       - Cylindrical equidistant
'laea'      - Lambert azimuthal
```

### Plotting Points

```python
# Convert coordinates
x, y = m(-74.0, 40.7)  # New York

# Plot
m.plot(x, y, 'ro', markersize=5)

# Multiple points
lats = [40.7, 51.5, 35.7]  # NYC, London, Tokyo
lons = [-74.0, -0.1, 139.7]
x, y = m(lons, lats)
m.plot(x, y, 'ro')
```

### Drawing Great Circles

```python
# Draw flight path
m.drawgreatcircle(-74, 40.7,    # NYC
                  -0.1, 51.5,    # London
                  linewidth=2,
                  color='red')
```

### Basemap Methods

| Method | Purpose |
|--------|---------|
| `contour()` / `contourf()` | Draw contour lines / filled contours |
| `imshow()` / `pcolor()` | Draw image / pseudo-color plot |
| `plot()` / `scatter()` | Draw lines / points |
| `quiver()` / `barbs()` | Draw vectors / wind barbs |

---

## 4.11 VISUALIZATION WITH SEABORN

### Introduction to Seaborn

**Seaborn** is built on Matplotlib for attractive statistical graphics.

**Installation:**
```bash
pip install seaborn
```

**Import:**
```python
import seaborn as sns
import matplotlib.pyplot as plt
```

### Matplotlib vs Seaborn

| Feature | Matplotlib | Seaborn |
|---------|------------|---------|
| **Use Case** | Base library. Works with arrays. | Enhanced. Uses Matplotlib+NumPy+Pandas. |
| **Syntax** | Comparatively lengthy & complex | Comparatively simple & elegant |
| **Multiple Figs** | Can open multiple at a time | Automatically manages multiple figures |
| **Flexibility** | Highly customizable & powerful | Provides default production themes |

### Seaborn Examples

```python
import seaborn as sns
import pandas as pd

df = pd.read_csv("WorldHappiness2016.csv")

# Scatter plot
sns.scatterplot(data=df, x="Economy", y="Happiness")

# Line plot
sns.lineplot(data=df, x='x', y='y')

# Bar plot
sns.barplot(data=df, x='cat', y='val')

# Histogram
sns.histplot(data=df, x='col', bins=20)

# Box plot
sns.boxplot(data=df, x='cat', y='val')

# Heatmap (correlation matrix)
sns.heatmap(df.corr(), annot=True)

# Pair plot (all pairwise relationships)
sns.pairplot(df)

# Violin plot
sns.violinplot(data=df, x='cat', y='val')

# Set style
sns.set_style("whitegrid")  # darkgrid, dark, white, ticks
```

### Styling Options

```python
# Set style
sns.set_style('whitegrid')
sns.set_style('darkgrid')
sns.set_style('white')
sns.set_style('ticks')

# Set context (font sizes)
sns.set_context('paper')
sns.set_context('talk')
sns.set_context('poster')

# Set color palette
sns.set_palette('husl')
sns.set_palette('muted')
sns.set_palette('bright')
```

---

# 📚 QUICK REFERENCE CHEATSHEET

## NUMPY

```python
# Array Creation
np.array([1,2,3])              # Create 1D array
np.zeros((3,4))                # Array of zeros (3x4)
np.ones((2,3))                 # Array of ones
np.arange(0,10,2)              # 0, 2, 4, 6, 8
np.linspace(0,1,5)             # 5 evenly spaced in [0,1]
np.random.randn(3,3)           # 3x3 random normal array

# Array Operations
arr.reshape(2,3)               # Reshape to 2 rows 3 cols
arr.T                          # Transpose
np.concatenate([a,b])          # Join arrays
np.split(arr,[3,5])            # Split at indices 3 & 5

# Aggregations
np.sum/np.min/np.max/np.mean/np.std  # Basic aggregations
np.argmin/np.argmax            # Index of min/max
np.percentile(L, 25)           # 25th percentile

# Indexing
a[a > 5]                       # Boolean mask
a[[1,3,5]]                     # Fancy indexing
a[rows, cols]                  # 2D indexing

# Universal Functions
np.sqrt(a)                     # Square root
np.exp(a)                      # Exponential
np.log(a)                      # Natural log
np.sin(a)/np.cos(a)/np.tan(a)  # Trigonometric
```

## PANDAS

```python
# Creation
pd.Series([1,2,3])             # Create Series
pd.DataFrame(data)             # Create DataFrame

# Inspection
df.head(5)/df.tail(5)          # First 5 rows/Last 5 rows
df.info()                      # Column types & NaN count
df.describe()                  # Statistical summary
df.shape                       # (rows, columns)

# Missing Data
df.isnull().sum()              # Count missing per column
df.fillna(0)                   # Fill NaN with 0
df.dropna()                    # Drop rows with NaN
df.drop_duplicates()           # Remove duplicate rows

# Indexing & Selection
df.loc[r,c]                    # Label based
df.iloc[r,c]                   # Position based
df[mask]                       # Boolean filtering
df.at/i                        # Fast scalar access

# Operations
df * scalar                    # Vectorized ops
.apply(fn)                     # Apply function
.map()                         # Element-wise Series
.applymap()                    # Element-wise DataFrame

# Grouping & Aggregation
df.groupby("col").sum()        # GroupBy and sum
.transform()                   # Return same shape
.filter()                      # Keep/drop groups

# Combining Data
pd.concat([df1,df2])           # Concatenate DataFrames
pd.merge(df1,df2,on='key')     # Merge (SQL join)
df.join()                      # Index-based join

# Pivot Tables
pd.pivot_table(df, index=["a"], aggfunc="mean")  # Pivot table
```

## MATPLOTLIB

```python
# Import & Setup
import matplotlib.pyplot as plt
plt.style.use('seaborn-v0_8')  # Set style

# Basic Plots
plt.plot(x,y)                  # Line plot
plt.scatter(x,y)               # Scatter plot
plt.hist(x,bins=20)            # Histogram
plt.bar(x,height)              # Bar chart
plt.errorbar(x, y, yerr=e)     # Error bar
plt.contour(X,Y,Z)             # Contour lines
plt.contourf(X,Y,Z)            # Filled contour

# Customization
plt.xlabel("x"); plt.ylabel("y")  # Axis labels
plt.title("Title")             # Set title
plt.legend(loc='best')         # Show legend
plt.grid(True)                 # Enable grid
plt.xticks(rotation=45)        # Rotate labels

# Display & Save
plt.show()                     # Display plot
plt.savefig("out.png",dpi=300) # Save figure

# Subplots
plt.subplot(rows,cols,pos)     # Create subplot
fig, axes = plt.subplots(2,2)  # Multiple subplots

# Annotations
plt.annotate("text", xy, xytext, arrowprops)  # Annotation

# 3D Support
from mpl_toolkits.mplot3d import Axes3D
ax = fig.add_subplot(111, projection='3d')
```

## SEABORN

```python
# Import
import seaborn as sns

# Statistical Plots
sns.scatterplot(data=df, x="x", y="y")  # Scatter
sns.lineplot(data=df, x="x", y="y")     # Line
sns.histplot(data=df, x="col")          # Histogram
sns.boxplot(data=df, x="cat", y="val")  # Box plot
sns.violinplot(data=df, x="cat", y="val")  # Violin
sns.heatmap(df.corr(), annot=True)      # Heatmap
sns.pairplot(df)                        # Pair plot
sns.regplot(data=df, x="x", y="y")      # Regression

# Styling
sns.set_style("whitegrid")              # Set style
sns.set_context("talk")                 # Set context
sns.set_palette("husl")                 # Set palette
```

---

## 📖 FORMULAS QUICK REFERENCE

### Statistics

```
Mean:           μ = Σx / n

Variance:       σ² = Σ(x - μ)² / n

Standard Dev:   σ = √σ²

Z-Score:        Z = (X - μ) / σ

Range:          Range = Max - Min

CV:             CV = (σ / μ) × 100%
```

### Correlation & Regression

```
Pearson r:
        n(Σxy) - (Σx)(Σy)
r = ─────────────────────────────────────
    √{[nΣx² - (Σx)²] × [nΣy² - (Σy)²]}

Coefficient of Determination: R² = r²

Regression Line: Ŷ = a + bX

Slope:          b = [n(ΣXY) - (ΣX)(ΣY)] / [nΣX² - (ΣX)²]

Intercept:      a = Ȳ - bX̄

Standard Error: SEE = √[Σ(Y - Ŷ)² / (n - 2)]
```

### Empirical Rule

```
μ ± 1σ → 68% of data
μ ± 2σ → 95% of data
μ ± 3σ → 99.7% of data
```

### Multiple Regression

```
Ŷ = β₀ + β₁X₁ + β₂X₂ + ... + βₙXₙ

VIF = 1 / (1 - R²ⱼ)  [Check multicollinearity]
```

---
