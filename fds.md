# 📚 DATA SCIENCE STUDY GUIDE
## Your Complete Path to 100/100

---

# 📖 MODULE 1: INTRODUCTION AND DESCRIBING DATA

## 1.1 DATA SCIENCE: BENEFITS AND USES

### What is Data Science?

**Data Science** is the domain of study that deals with vast volumes of data using modern tools and techniques to:
- Find unseen patterns
- Derive meaningful information
- Make business decisions

Data Science sits at the **intersection** of three critical domains:

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

### Importance of Data Science

- **Global data projection**: Expected to grow to **175 zettabytes by 2025** (IDC)
- **Speed**: Replaces traditional days/weeks of analysis, processing data in **hours**
- **Insights**: Allows companies to understand gigantic data and derive valuable insights

### Benefits of Data Science

1. **Identifying business opportunities** - Discovering new markets and trends
2. **Helping make better decisions** - Data-driven decision making
3. **Improving performance** - Optimizing operations and processes
4. **Identifying target audiences** - Precise customer segmentation
5. **Fighting competitors** - Strategic advantage through insights

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

**Uses:**
- Transforming user data into profitable information
- Lowering accidents in transport (e.g., driverless cars)
- Therapeutic customization in genetics/genomics

---

## 1.2 FACETS OF DATA

Data comes in various types. Understanding these facets is crucial for proper data handling.

### 1. Structured Data

**Definition:** Data organized in an identifiable structure, like rows and columns methodology.

**Characteristics:**
- Easily searchable by data type
- Understood by both computers and humans
- Fixed schema

**Examples:**
- Excel tables
- Database Management Systems (SQL databases)
- Spreadsheets

```
+----------+----------+----------+----------+
|   ID     |   Name   |   Age    |  Salary  |
+----------+----------+----------+----------+
|    1     |  Alice   |    25    |  50000   |
|    2     |   Bob    |    30    |  60000   |
|    3     |  Carol   |    28    |  55000   |
+----------+----------+----------+----------+
```

### 2. Unstructured Data

**Definition:** Data that does not follow a specified format, structural rules, or sequence.

**Characteristics:**
- Unpredictable in nature
- Makes up **over 80%** of modern organizational data
- No predefined data model

**Examples:**
- Documents (PDFs, Word files)
- Email messages
- Customer feedback
- Audio files
- Video files
- Images

### 3. Natural Language

**Definition:** A special type of unstructured data representing human speech/text.

**Requirements:**
- Requires **NLP (Natural Language Processing)** to help machines:
  - Understand meaning
  - Recognize entities
  - Summarize text
  - Perform sentiment analysis

**Examples:**
- Social media posts
- Chat logs
- News articles
- Customer reviews

### 4. Machine-Generated Data

**Definition:** Information created **without human interaction** by computer processes.

**Types:**
- **M2M (Machine-to-Machine)** interactions
- **H2M (Human-to-Machine)** interactions

**Examples:**
- Web server logs
- Call detail records
- Telemetry data
- RFID technology data
- Sensor data (IoT devices)

### 5. Graph-Based (Network) Data

**Definition:** Describes relationships/interactions in complex systems.

**Components:**
- **Nodes**: Entities/objects
- **Edges**: The interactions between them

**Storage:**
- Graph Databases
- Queries like **SPARQL**
- Like sketching ideas on a whiteboard rather than using tables

```
        (Alice)-----(Bob)
           |           |
           |           |
        (Carol)-----(David)
           \         /
            \       /
           (Eve)
```

### 6. Audio, Image, and Video (Multimedia)

**Characteristics:**
- Time-based media storage
- **Trivial for humans** (e.g., recognizing a face)
- **Highly challenging for computers** to transform and index

**Examples:**
- Surveillance footage
- Medical imaging (X-rays, MRIs)
- Music files
- Video streams

### 7. Streaming Data

**Definition:** Data generated **continuously** by thousands of sources simultaneously in small sizes (Kilobytes).

**Characteristics:**
- Real-time generation
- High velocity
- Continuous flow

**Examples:**
- Live ecommerce purchases
- In-game player activity
- Financial trading floors
- Social media feeds
- Sensor networks

---

## 1.3 DATA SCIENCE PROCESS: OVERVIEW

The Data Science Process is the **lifecycle of a data project**, broken into **6 essential steps**:

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

### Step 1: Setting the Research Goal

**Purpose:** Defining the **what, how, and why** of the project so all stakeholders understand.

**Primary Output: Project Charter**

The Project Charter contains:
1. **Clear research goal** - What problem are we solving?
2. **Project mission/context** - Why does this matter?
3. **Analysis plan** - How will we approach it?
4. **Required resources** - What do we need?
5. **Proof of concept** - Can it be done?
6. **Deliverables** - What will we produce?
7. **Timeline** - When will it be completed?

**Example:**
If a retail company wants to reduce customer churn:
- **Goal**: Identify customers likely to leave in next 3 months
- **Mission**: Reduce churn by 15% to increase revenue
- **Plan**: Analyze purchase history, customer service interactions
- **Resources**: Data analyst, ML engineer, customer data
- **Deliverable**: Churn prediction model with 85% accuracy
- **Timeline**: 3 months

### Step 2: Retrieving Data

**Purpose:** Finding and acquiring the data needed for analysis.

**Sources of Data:**

**A. Internal Data:**
- Company databases
- Data marts
- Data warehouses
- Data lakes

**B. External Data:**
- Bought/sourced from third parties
- Examples: Nielsen data, Twitter API, government databases

**Data Quality Checks:**
Done at this stage to prevent spending hours fixing easily preventable import issues:
- Check for missing values
- Verify data types
- Identify duplicates
- Validate ranges

**Example:**
For a customer analytics project:
- **Internal**: Customer database, transaction logs, CRM system
- **External**: Demographic data from census, social media sentiment

### Step 3: Data Preparation (Data Cleansing & Transformation)

**⚠️ CRITICAL:** Expect to spend **up to 80% of project time** here!

**A. Data Cleansing:**
Fixing issues in raw data:
1. **Errors** - Incorrect values
2. **Physically impossible values** - Age = 150, negative height
3. **Missing values** - NULL, NaN entries
4. **Outliers** - Extreme values that may skew results
5. **Typos** - Spelling errors
6. **Duplicate data** - Repeated records

**B. Data Transformation:**
Converting data into usable format:
1. **Aggregating data** - Summarizing at different levels
2. **Deriving new measures** - Creating calculated fields
3. **Creating dummy variables** - Converting categories to numbers
4. **Reducing variables** - Feature selection
5. **Joining datasets** - Combining multiple sources

**Example:**
Raw customer data issues:
```
Before Cleansing:
ID  | Name    | Age | Purchase
----+---------+-----+----------
1   | Alice   | 25  | 100
2   | Bob     |     | 150
3   | Carol   | 150 | 200
4   | Alice   | 25  | 100  (duplicate)
5   | Dave    | -5  | 50
```

```
After Cleansing:
ID  | Name    | Age | Purchase
----+---------+-----+----------
1   | Alice   | 25  | 100
2   | Bob     | 30* | 150   (*imputed mean)
3   | Carol   | 50* | 200   (*corrected)
4   | Dave    | 35* | 50    (*corrected)
```

### Step 4: Data Exploration (EDA - Exploratory Data Analysis)

**Purpose:** Diving deeper into data using descriptive statistics and visual techniques.

**Techniques:**

**A. Simple Graphs:**
- **Histograms** - Distribution of single variable
- **Density plots** - Smoothed distribution

**B. Combined Graphs:**
- **Scatter plots** - Relationship between two variables

**C. Brushing and Linking:**
- Selecting observations in one plot
- System highlights those same observations in other plots simultaneously
- Helps identify patterns across multiple views

**Goals:**
- Find hidden patterns
- Identify outliers
- Understand distributions
- Detect relationships
- Generate hypotheses

**Example:**
Exploring sales data:
- Histogram shows most sales are between $50-$200
- Scatter plot reveals higher sales on weekends
- Box plot identifies 3 outlier transactions > $1000

### Step 5: Data Modeling

**Purpose:** Using ML and statistical techniques to achieve the goal.

**A. Model Selection:**
Deciding based on:
1. **Performance** - Accuracy, precision, recall
2. **Ease of implementation** - Complexity
3. **Maintenance** - Ongoing requirements
4. **Explainability** - Can we interpret results?

**B. Execution:**
Using Python libraries:
- **Scikit-learn** - Machine learning algorithms
- **StatsModels** - Statistical models

**C. Model Comparison:**
Using a **Holdout Sample**:
- Typical split: **80% Train / 20% Test**
- Model trained on one part
- Evaluated on "unseen" test data
- Calculate error measures:
  - **Mean Square Error (MSE)**
  - **Root Mean Square Error (RMSE)**
  - **R-squared**

**Example:**
Predicting house prices:
- **Algorithm**: Linear Regression
- **Training**: 800 houses
- **Testing**: 200 houses
- **MSE**: 15,000
- **R²**: 0.85 (85% variance explained)

### Step 6: Presentation and Automation

**Purpose:** Presenting findings to stakeholders and automating for future use.

**A. Presentation:**
- Create reports
- Visualizations
- Dashboards
- PowerPoint presentations
- Executive summaries

**B. Automation:**
- Automating model scoring
- Updating reports automatically
- Excel sheet generation
- Scheduled retraining
- API deployment

**Key Principle:** Analysis doesn't have to be entirely redone manually each time.

**Example:**
Monthly sales forecast:
- **Dashboard**: Interactive Tableau/Power BI
- **Report**: Automated PDF sent to managers
- **Model**: Retrains monthly with new data
- **API**: Allows real-time predictions

---

## 1.4 DATA MINING

### Definition

**Data Mining** is the process of analyzing data to discover meaningful patterns and predict future outcomes.

### Technology Used

- **Artificial Intelligence (AI)**
- **Machine Learning** algorithms
- **Statistics**
- **Pattern recognition logic**

### Process Flow

```
Raw Data → Preprocessing → Pattern Discovery → Validation → Knowledge
```

### Advantages

1. **Fault detection** - Identify anomalies and errors
2. **Cost-effective** - Automated pattern discovery
3. **Easily accessible knowledge** - Insights from large datasets
4. **Predictive capabilities** - Forecast future trends
5. **Hidden pattern discovery** - Find relationships not obvious

### Disadvantages

1. **Not 100% accurate** - Can lead to breaches or false positives
2. **Resource-heavy** - Requires significant training/implementation
3. **Privacy concerns** - May reveal sensitive information
4. **Complexity** - Requires specialized skills
5. **Overfitting risk** - Models may not generalize well

### Carried Out By

- **Business users**
- **Data Scientists**

### Data Mining Techniques

**1. Classification:**
- Assigning data into predefined categories
- **Example**: Spam vs Not Spam email detection

**2. Clustering:**
- Grouping data based on similarities
- No predefined classes
- **Example**: Grouping customers into personas

**3. Association Rule Mining:**
- Finding "If-Then" patterns
- **Example**: Market basket analysis - "If customer buys bread, they also buy butter"

**4. Prediction:**
- Forecasting continuous numerical outcomes
- **Example**: Predicting house prices, stock values

---

## 1.5 DATA WAREHOUSING

### Definition

A **Data Warehouse** is a:
- **Subject-oriented** database system
- **Integrated** from multiple sources
- **Time-varying** (historical data)
- **Non-volatile** (data doesn't change once loaded)
- Designed for **analytical analysis** (NOT transactional work)

### Process: ETL

**Extract, Transform, Load (ETL)**

```
+----------+     +----------+     +----------+
| Extract  | --> |Transform | --> |  Load    |
+----------+     +----------+     +----------+
    |                |                |
    v                v                v
 Multiple       Clean &          Central
Sources         Format          Warehouse
```

**Extract:** Pull data from various sources
**Transform:** Clean, format, integrate data
**Load:** Store in data warehouse

### Advantages

1. **Easy to understand** - Unified view of data
2. **Continuous updates** - Regular refresh cycles
3. **Stores historical data** - For trend evaluation
4. **Improved data quality** - Cleansed during ETL
5. **Better decision making** - Single source of truth

### Disadvantages

1. **Risk of accumulating useless data** - Storage costs
2. **Cleansing data from multiple sources is difficult** - Complex ETL
3. **High initial cost** - Infrastructure and setup
4. **Time-consuming** - ETL processes take time
5. **Data latency** - Not always real-time

### Carried Out By

- **Data Engineers**
- **IT Professionals**

### Data Mining vs Data Warehousing Comparison

```
+------------------+---------------------------+---------------------------+
|    Feature       |    Data Warehousing       |      Data Mining          |
+------------------+---------------------------+---------------------------+
| Definition       | Database system for       | Process of analyzing      |
|                  | analytical analysis       | data to discover patterns |
+------------------+---------------------------+---------------------------+
| Process          | ETL (Extract, Transform,  | Regular analysis using    |
|                  | Load) periodically        | AI and ML algorithms      |
+------------------+---------------------------+---------------------------+
| Data Handling    | Pooling relevant data     | Extracting insights from  |
|                  | into central location     | large datasets            |
+------------------+---------------------------+---------------------------+
| Managed By       | Data Engineers / IT       | Data Scientists /         |
|                  |                           | Business Users            |
+------------------+---------------------------+---------------------------+
| Example          | Consolidating sales data  | Finding patterns like     |
|                  | from 50 stores into one   | "customers who buy X      |
|                  | server                    | also buy Y"               |
+------------------+---------------------------+---------------------------+
```

---

## 1.6 BASIC STATISTICAL DESCRIPTIONS OF DATA

### Why Describe Data?

1. **Organize raw data** - Make sense of chaos
2. **Identify trends/noise/outliers** - Understand patterns
3. **Communicate insights visually** - Share findings
4. **Make data-driven decisions** - Evidence-based actions

### Types of Descriptive Statistics

**1. Distribution:**
- Frequencies of responses
- How data is spread across values

**2. Central Tendency:**
- The "average" or typical value
- **Measures**: Mean, Median, Mode

**3. Variability:**
- Spread or dispersion
- **Measures**: Range, Variance, Standard Deviation, IQR

---

## 1.7 TYPES OF DATA

### Main Classifications

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

### Qualitative (Categorical) Data

**Definition:** Describes qualities, non-numeric characteristics.

**Examples:**
- Color (Red, Blue, Green)
- Gender (Male, Female, Other)
- Brand (Apple, Samsung, Google)
- Country (India, USA, UK)

**Cannot perform arithmetic operations**

### Quantitative (Numerical) Data

**Definition:** Describes measurable quantities.

**Two Types:**

**A. Discrete Data:**
- Countable whole numbers
- **Question**: "Can I count it?"
- **Examples**:
  - Number of students in class (25, 30, 35)
  - Number of cars (1, 2, 3)
  - Number of defects (0, 1, 2)

**B. Continuous Data:**
- Any value in a range
- Decimals allowed
- **Question**: "Can I measure it?"
- **Examples**:
  - Height (175.5 cm, 180.2 cm)
  - Temperature (36.7°C, 37.2°C)
  - Weight (68.5 kg, 72.3 kg)
  - Time (3.14 seconds)

---

## 1.8 TYPES OF VARIABLES

### Four Scales of Measurement

**1. Nominal Scale:**
- Categories with **NO order**
- Only **Mode** can be calculated
- **Examples**:
  - Gender (Male/Female)
  - Blood type (A, B, AB, O)
  - Eye color (Blue, Brown, Green)

**2. Ordinal Scale:**
- Ordered categories
- **Gaps between categories are unknown**
- **Examples**:
  - 1-5 star ratings (⭐⭐⭐⭐⭐)
  - Education level (High School < Bachelor < Master < PhD)
  - Customer satisfaction (Very Unsatisfied < Unsatisfied < Neutral < Satisfied < Very Satisfied)

**3. Interval Scale:**
- Ordered categories
- **Equal intervals** between values
- **NO true zero** (zero doesn't mean absence)
- **Examples**:
  - Temperature in Celsius (0°C doesn't mean "no temperature")
  - Calendar years
  - IQ scores

**4. Ratio Scale:**
- Ordered categories
- **Equal intervals**
- **TRUE ZERO** (zero means complete absence)
- **Examples**:
  - Weight (0 kg means no weight)
  - Height (0 cm means no height)
  - Income (₹0 means no income)
  - Age (0 years means birth)

### Variables in Research

**1. Independent Variable (IV):**
- Hypothesized **cause**
- **Predictor** variable
- **Manipulated** by researcher
- **Example**: Study hours, dosage of medicine

**2. Dependent Variable (DV):**
- **Outcome** measured
- The **response**
- What we're trying to predict
- **Example**: Exam score, patient recovery

**3. Control Variable:**
- **Held constant** to reduce bias
- Prevents confounding
- **Example**: Same exam for all students, same room temperature

**4. Confounding Variable:**
- A **hidden variable** affecting both IV and DV
- Causes a **false relationship**
- **Example**: Hot weather causing both ice cream sales AND sunburns (not that ice cream causes sunburns!)

---

## 1.9 DESCRIBING DATA WITH TABLES AND GRAPHS

### Frequency Distributions

**Definition:** A systematic arrangement of data showing the frequency (count) of each value or class interval.

**Types:**

**A. Ungrouped Frequency Distribution:**
- Individual scores and their frequencies
- Used for small datasets

**Example:**
```
Test Scores of 10 Students: 85, 90, 85, 78, 90, 92, 85, 78, 90, 88

Score    Tally        Frequency
-----------------------------
  78      ||             2
  85      |||            3
  88      |              1
  90      |||            3
  92      |              1
-----------------------------
Total                    10
```

**B. Grouped Frequency Distribution:**
- Data grouped into **Class Intervals**
- Used for large datasets

**Components:**
- **Class Interval**: Range of values (e.g., 10-20, 20-30)
- **Class Width**: Difference between upper and lower limits
- **Midpoint**: (Lower limit + Upper limit) / 2

**Example:**
```
Ages of 50 People:

Class Interval    Tally        Frequency    Midpoint
----------------------------------------------------
   10-20           |||            3           15
   20-30           |||||          5           25
   30-40           |||||||        7           35
   40-50           ||||||||||    10           45
   50-60           |||||||||      9           55
   60-70           ||||||||||    10           65
   70-80           |||||          5           75
   80-90           |              1           85
----------------------------------------------------
Total                           50
```

### Visualizing Data

**1. Histogram:**

**Characteristics:**
- **Contiguous (touching) bars** of equal width
- **X-axis**: Class intervals
- **Y-axis**: Frequency
- Shows **shape and spread** of distribution
- Used for **continuous data**

```
    Frequency
       10 |           ████
        8 |        ████████
        6 |     ████████████
        4 |  ████████████████
        2 |██████████████████
        0 +-------------------
          0   20  40  60  80  100
              Class Intervals
```

**Example:**
```python
import matplotlib.pyplot as plt
import numpy as np

data = np.random.normal(50, 15, 1000)
plt.hist(data, bins=20, edgecolor='white', density=False)
plt.xlabel('Value')
plt.ylabel('Frequency')
plt.title('Histogram of Data Distribution')
plt.show()
```

**2. Frequency Polygon:**

**Characteristics:**
- **Line graph** connecting histogram midpoints
- Good for **comparing multiple trends**
- Points plotted at midpoints

```
    Frequency
       10 |           ●
        8 |        ●     ●
        6 |     ●           ●
        4 |  ●                 ●
        2 |●                     ●
        0 +---●---●---●---●---●---
          0   20  40  60  80  100
```

**3. Bar Chart:**

**Characteristics:**
- Bars **NOT touching** (gaps between)
- Used for **categorical data**
- X-axis: Categories
- Y-axis: Frequency or value

```
    Frequency
       10 |       █
        8 |       █       █
        6 |   █   █   █   █
        4 |   █   █   █   █   █
        2 |   █   █   █   █   █
        0 +---+---+---+---+---+
           Red Blue Green Yellow
            Color Categories
```

**4. Pie Chart:**

**Characteristics:**
- **Proportions as slices**
- Shows parts of a whole
- **Limitation**: Hard to read with too many categories

```
              Sales by Region
                  
            ┌─────────┐
          ╱│    East  │╲
         │ │   30%    │ │
        │  └──────────┘  │
        │ North    │West│
        │  25%     │20% │
         │         │    │
          ╲        │   ╱
            ╲──────╱
              South
              25%
```

**5. Line Graph:**

**Characteristics:**
- **Connects points over time**
- Shows **trends**
- X-axis: Time periods
- Y-axis: Values

```
    Sales (₹L)
       100 |           ●
        80 |        ●     ●
        60 |     ●           ●
        40 |  ●                 ●
        20 |●                     ●
         0 +---●---●---●---●---●---
            Jan Feb Mar Apr May Jun
                  Time
```

**6. Ogive (Cumulative Frequency Curve):**

**Characteristics:**
- Shows **cumulative frequencies**
- Always increasing (or flat)
- Helps find percentiles

```
Cumulative Freq
      100 |                  ●
       80 |              ●
       60 |          ●
       40 |      ●
       20 |  ●
        0 +--●--●--●--●--●--
           0  20 40 60 80 100
```

**7. Box Plot (Box-and-Whisker Plot):**

**Characteristics:**
- Shows **median, quartiles, and outliers**
- **5-number summary**:
  - Minimum
  - Q1 (25th percentile)
  - Median (Q2, 50th percentile)
  - Q3 (75th percentile)
  - Maximum
- **IQR** = Q3 - Q1
- **Outliers** shown as individual points

```
    Value
      90 |                    ○ (outlier)
      80 |                    |
      75 |              +-----+
      70 |              |     |
      65 |         +----+     |
      60 |         |    |     |
      55 |         |    |     |
      50 |    +----+    |     |
      45 |    |         |     |
      40 +----+---------+-----+
           Min Q1      Med    Q3  Max
```

**Example:**
```python
import matplotlib.pyplot as plt
import numpy as np

data = [5, 7, 8, 6, 5, 9, 10, 6, 7, 8, 5, 6]
plt.boxplot(data)
plt.ylabel('Value')
plt.title('Box Plot')
plt.show()
```

---

## 1.10 DESCRIBING DATA WITH AVERAGES (CENTRAL TENDENCY)

### Mean (Arithmetic Average)

**Definition:** The sum of all values divided by the number of values.

**Formula:**
```
        Σx
   μ = ----
        n

Where:
μ = Population mean
Σx = Sum of all values
n = Number of values
```

**Characteristics:**
- Uses all data points
- Affected by outliers
- Best for symmetric distributions

**Example 1 - Basic Calculation:**

**Problem:** Calculate the mean of: 12, 15, 18, 20, 15, 22, 25, 15

**Solution:**
```
Step 1: Sum all values
Σx = 12 + 15 + 18 + 20 + 15 + 22 + 25 + 15 = 142

Step 2: Count values
n = 8

Step 3: Calculate mean
μ = 142 / 8 = 17.75

Answer: Mean = 17.75
```

**Example 2 - Sales Data:**

**Problem:** Monthly sales (₹1000s): 25, 30, 28, 35, 40, 32, 30, 29

**Solution:**
```
Step 1: Sum all values
Σx = 25 + 30 + 28 + 35 + 40 + 32 + 30 + 29 = 249

Step 2: Count values
n = 8

Step 3: Calculate mean
μ = 249 / 8 = 31.125

Interpretation: Average monthly sales = ₹31,125
```

### Median

**Definition:** The exact middle value of a dataset when ordered sequentially.

**Calculation:**

**For Odd n:**
```
Position = (n + 1) / 2
```

**For Even n:**
```
Median = Average of two middle values
Position 1 = n/2
Position 2 = (n/2) + 1
```

**Characteristics:**
- Not affected by outliers
- Best for skewed distributions
- Represents the 50th percentile

**Example 1 - Odd Number of Values:**

**Problem:** Find median of: 7, 2, 9, 4, 6

**Solution:**
```
Step 1: Arrange in order
2, 4, 6, 7, 9

Step 2: Find position
n = 5 (odd)
Position = (5 + 1) / 2 = 3

Step 3: Identify value at position 3
Median = 6
```

**Example 2 - Even Number of Values:**

**Problem:** Find median of: 12, 15, 18, 20, 15, 22, 25, 15

**Solution:**
```
Step 1: Arrange in order
12, 15, 15, 15, 18, 20, 22, 25

Step 2: Find positions
n = 8 (even)
Position 1 = 8/2 = 4
Position 2 = 4 + 1 = 5

Step 3: Identify values
Value at position 4 = 15
Value at position 5 = 18

Step 4: Calculate average
Median = (15 + 18) / 2 = 16.5

Answer: Median = 16.5
```

### Mode

**Definition:** The value that appears **most frequently** in a dataset.

**Characteristics:**
- Can have no mode, one mode, or multiple modes
- **Unimodal**: One mode
- **Bimodal**: Two modes
- **Multimodal**: More than two modes
- Not affected by outliers
- Only measure for nominal data

**Example 1 - Single Mode:**

**Problem:** Find mode of: 12, 15, 18, 20, 15, 22, 25, 15

**Solution:**
```
Count frequencies:
12: appears 1 time
15: appears 3 times
18: appears 1 time
20: appears 1 time
22: appears 1 time
25: appears 1 time

Most frequent = 15 (appears 3 times)

Answer: Mode = 15
```

**Example 2 - Bimodal:**

**Problem:** Find mode of: 5, 7, 8, 6, 5, 9, 10, 6, 7, 8, 5, 6

**Solution:**
```
Count frequencies:
5: appears 3 times
6: appears 3 times
7: appears 2 times
8: appears 2 times
9: appears 1 time
10: appears 1 time

Both 5 and 6 appear most frequently (3 times each)

Answer: Mode = 5 and 6 (Bimodal)
```

### Relationship Between Mean, Median, and Mode

**For Symmetric Distribution:**
```
Mean = Median = Mode
```

**For Right-Skewed (Positively Skewed):**
```
Mean > Median > Mode
```

**For Left-Skewed (Negatively Skewed):**
```
Mean < Median < Mode
```

```
Symmetric:           Right-Skewed:        Left-Skewed:
     ▲                    ▲                    ▲
     │                    │                    │
     │       ╱─╲          │         ╱─╲        │  ╱─╲
     │     ╱     ╲        │       ╱       ╲    │╱     
     │   ╱         ╲      │     ╱           ╲  │       ╲
     │ ╱             ╲    │   ╱               ╲│        ╲
     └─────────────────   └────────────────────└─────────────────
     M=Md=Mo              Mo  Md   M            M   Md  Mo
```

---

## 1.11 DESCRIBING VARIABILITY (DISPERSION)

### Range

**Definition:** The difference between the highest and lowest values.

**Formula:**
```
Range = Maximum Value - Minimum Value
```

**Characteristics:**
- Simplest measure
- Highly affected by outliers
- Only uses two values

**Example:**

**Problem:** Find range of: 12, 15, 18, 20, 15, 22, 25, 15

**Solution:**
```
Maximum = 25
Minimum = 12

Range = 25 - 12 = 13

Answer: Range = 13
```

### Variance

**Definition:** The average squared distance of all values from the mean.

**Formula (Population):**
```
          Σ(x - μ)²
   σ² = -----------
             n

Where:
σ² = Population variance
x = Each value
μ = Population mean
n = Number of values
```

**Formula (Sample):**
```
          Σ(x - x̄)²
   s² = -----------
            n - 1
```

**Characteristics:**
- Uses all data points
- Squared units (not intuitive)
- Foundation for standard deviation

**Example 1 - Basic Variance:**

**Problem:** Calculate variance of: 40, 45, 50, 55, 60

**Solution:**
```
Step 1: Calculate mean
μ = (40 + 45 + 50 + 55 + 60) / 5 = 250 / 5 = 50

Step 2: Calculate squared deviations
(40 - 50)² = (-10)² = 100
(45 - 50)² = (-5)²  = 25
(50 - 50)² = (0)²   = 0
(55 - 50)² = (5)²   = 25
(60 - 50)² = (10)²  = 100

Step 3: Sum squared deviations
Σ(x - μ)² = 100 + 25 + 0 + 25 + 100 = 250

Step 4: Calculate variance
σ² = 250 / 5 = 50

Answer: Variance = 50
```

**Example 2 - Sales Data Variance:**

**Problem:** Calculate variance for sales: 25, 30, 28, 35, 40, 32, 30, 29

**Solution:**
```
Step 1: Calculate mean
μ = 249 / 8 = 31.125

Step 2: Calculate squared deviations
(25 - 31.125)² = (-6.125)² = 37.516
(30 - 31.125)² = (-1.125)² = 1.266
(28 - 31.125)² = (-3.125)² = 9.766
(35 - 31.125)² = (3.875)²  = 15.016
(40 - 31.125)² = (8.875)²  = 78.766
(32 - 31.125)² = (0.875)²  = 0.766
(30 - 31.125)² = (-1.125)² = 1.266
(29 - 31.125)² = (-2.125)² = 4.516

Step 3: Sum squared deviations
Σ(x - μ)² = 37.516 + 1.266 + 9.766 + 15.016 + 78.766 
           + 0.766 + 1.266 + 4.516 = 148.878

Step 4: Calculate variance
σ² = 148.878 / 8 = 18.61

Answer: Variance ≈ 19.36 (using exact values)
```

### Standard Deviation

**Definition:** The square root of the variance. Shows the average distance of all values from the mean in **original units**.

**Formula:**
```
   σ = √σ²

Where:
σ = Standard deviation
σ² = Variance
```

**Characteristics:**
- In original units (not squared)
- Most common measure of spread
- Interpretable

**Example 1:**

**Problem:** Calculate standard deviation of: 40, 45, 50, 55, 60

**Solution:**
```
From previous calculation:
Variance σ² = 50

Standard Deviation:
σ = √50 = 7.07

Answer: Standard Deviation = 7.07

Interpretation: On average, values deviate from the mean by 7.07 units.
```

**Example 2:**

**Problem:** Calculate standard deviation for sales data

**Solution:**
```
From previous calculation:
Variance σ² = 19.359

Standard Deviation:
σ = √19.359 = 4.40

Interpretation: The average deviation of monthly sales from the mean 
is roughly ₹4,400.
```

### Coefficient of Variation (CV)

**Definition:** Relative measure of variability. Compares variability of datasets with different units.

**Formula:**
```
         σ
   CV = --- × 100%
         μ

Where:
σ = Standard deviation
μ = Mean
```

**Interpretation:**
- **CV < 10%**: Low variability / Stable
- **CV 10-30%**: Moderate variability
- **CV > 30%**: High variability

**Example:**

**Problem:** Compare variability of two datasets:
- Dataset A: Mean = 100, SD = 15
- Dataset B: Mean = 50, SD = 10

**Solution:**
```
Dataset A:
CV = (15 / 100) × 100% = 15%

Dataset B:
CV = (10 / 50) × 100% = 20%

Interpretation: Dataset B has higher relative variability (20%) 
compared to Dataset A (15%), even though A has higher absolute SD.
```

---

## 1.12 NORMAL DISTRIBUTIONS AND STANDARD (Z) SCORES

### Normal Distribution

**Definition:** A symmetric, bell-shaped distribution that is most common in nature.

**Characteristics:**
1. **Symmetric** around the center
2. **Mean = Median = Mode**
3. **Bell-shaped curve**
4. **Tails approach but never touch** the x-axis
5. **Total area under curve = 1** (or 100%)

**Examples in Nature:**
- Human heights
- IQ scores
- Blood pressure
- Measurement errors
- Test scores

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

### The Empirical Rule (68-95-99.7 Rule)

**Statement:** In a normal distribution:

```
• 68% of data falls within ±1 standard deviation of the mean
• 95% of data falls within ±2 standard deviations of the mean
• 99.7% of data falls within ±3 standard deviations of the mean
```

**Visual Representation:**

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

**Example 1:**

**Problem:** Test scores are normally distributed with Mean = 50, SD = 8.
a) What % of scores fall between 42 and 58?
b) What % of scores are beyond 66?

**Solution:**
```
Given:
μ = 50
σ = 8

a) Between 42 and 58:
   42 = 50 - 8 = μ - 1σ
   58 = 50 + 8 = μ + 1σ
   
   According to empirical rule:
   68% of data falls within ±1σ
   
   Answer: 68%

b) Beyond 66:
   66 = 50 + 16 = 50 + 2(8) = μ + 2σ
   
   According to empirical rule:
   95% of data falls between μ - 2σ and μ + 2σ
   (between 34 and 66)
   
   Remaining = 100% - 95% = 5%
   This 5% is split equally in both tails
   
   Beyond 66 = 5% / 2 = 2.5%
   
   Answer: 2.5%
```

### Z-Score (Standard Score)

**Definition:** A standardized score showing how many standard deviations a value is from the mean.

**Formula:**
```
         X - μ
   Z = ---------
          σ

Where:
Z = Z-score
X = Raw score
μ = Population mean
σ = Population standard deviation
```

**Interpretation:**
- **Z = 0**: Value equals the mean
- **Z > 0**: Value above the mean
- **Z < 0**: Value below the mean
- **Z = 1**: Value is 1 SD above mean
- **Z = -2**: Value is 2 SDs below mean

**Applications:**
1. Comparing scores from different distributions
2. Identifying outliers
3. Finding percentiles
4. Standardizing variables

**Example 1:**

**Problem:** Class mean = 60, SD = 5. Student scored 70. Calculate and interpret Z-score.

**Solution:**
```
Given:
X = 70
μ = 60
σ = 5

Formula:
       X - μ     70 - 60     10
   Z = ------- = --------- = ---- = 2.0
         σ          5        5

Interpretation: The student's score is exactly 2 standard deviations 
above the class mean, indicating excellent performance relative to 
the class.
```

**Example 2:**

**Problem:** Mean height = 165 cm, SD = 5 cm.
a) Find Z-score for height 170 cm
b) Find Z-score for height 155 cm

**Solution:**
```
Given:
μ = 165 cm
σ = 5 cm

a) For X = 170 cm:
         170 - 165     5
   Z = ------------- = --- = +1.0
            5         5
   
   Interpretation: 1 SD above average

b) For X = 155 cm:
         155 - 165    -10
   Z = ------------- = ---- = -2.0
            5          5
   
   Interpretation: 2 SDs below average
```

**Example 3 - Comparing Different Tests:**

**Problem:** 
- SAT Math: Score = 650, Mean = 500, SD = 100
- ACT Math: Score = 28, Mean = 21, SD = 5

Which is better?

**Solution:**
```
SAT Math:
       650 - 500    150
   Z = --------- = ----- = 1.5
         100       100

ACT Math:
       28 - 21     7
   Z = -------- = --- = 1.4
         5        5

Interpretation: The SAT score (Z = 1.5) is slightly better relative 
to its distribution than the ACT score (Z = 1.4).
```

### Outliers

**Definition:** An extreme data point that differs significantly from other observations in the dataset.

**Identification using Z-scores:**
- **|Z| > 3**: Potential outlier
- Often skews the mean

**Example:**

**Problem:** Identify outliers in: 10, 12, 11, 13, 50

**Solution:**
```
Step 1: Calculate mean
μ = (10 + 12 + 11 + 13 + 50) / 5 = 96 / 5 = 19.2

Step 2: Calculate SD
σ ≈ 15.8

Step 3: Calculate Z-scores
Z(10) = (10 - 19.2) / 15.8 = -0.58
Z(12) = (12 - 19.2) / 15.8 = -0.46
Z(11) = (11 - 19.2) / 15.8 = -0.52
Z(13) = (13 - 19.2) / 15.8 = -0.39
Z(50) = (50 - 19.2) / 15.8 = 1.95

In this small dataset, 50 might be an outlier, though |Z| < 3.
With larger datasets, use |Z| > 3 as threshold.
```

---

# 📖 MODULE 2: DESCRIBING RELATIONSHIPS AND PYTHON LIBRARIES

## 2.1 CORRELATION

### What is Correlation?

**Definition:** A statistical measure of the **strength and direction** of the linear relationship between two quantitative variables.

**Key Points:**
- Ranges from **-1 to +1**
- **Does NOT imply causation**
- Measures **association**, not cause-and-effect
- Symmetric: Correlation of X with Y = Correlation of Y with X

### Scatter Plots

**Definition:** A graphical representation showing the relationship between two quantitative variables using X and Y axes.

**Components:**
- **X-axis**: Independent variable
- **Y-axis**: Dependent variable
- **Each point**: One observation

**Patterns:**

```
Strong Positive      Weak Positive      No Correlation
Correlation (r≈0.9)  Correlation (r≈0.4) (r≈0)
     ▲                    ▲                    ▲
     │  ●●●              │ ●  ●             │●  ● ●
     │ ●●●●              │● ●● ●             │ ● ●●
     │●●●●●              │ ● ● ●             │● ● ●
     │●●●                │  ● ●              │ ●● ●
     │                   │                   │● ● ●
     └────────►         └────────►          └────────►

Strong Negative      Weak Negative
Correlation (r≈-0.9) Correlation (r≈-0.4)
     ▲                    ▲
     │●●●                 │  ● ●
     │ ●●●●               │ ● ●●
     │  ●●●●●             │● ● ●
     │   ●●●              │ ●● ●
     │                    │● ●
     └────────►         └────────►
```

### Correlation Coefficient (r)

**Definition:** A numerical value that quantifies the degree of linear correlation between two variables.

**Range:**
```
-1.0 ≤ r ≤ +1.0
```

**Interpretation:**

| r Value | Strength | Direction |
|---------|----------|-----------|
| +1.0 | Perfect | Positive |
| +0.8 to +1.0 | Strong | Positive |
| +0.5 to +0.8 | Moderate | Positive |
| +0.3 to +0.5 | Weak | Positive |
| 0 to +0.3 | Very Weak | Positive |
| 0 | None | None |
| -0.3 to 0 | Very Weak | Negative |
| -0.5 to -0.3 | Weak | Negative |
| -0.8 to -0.5 | Moderate | Negative |
| -1.0 to -0.8 | Strong | Negative |
| -1.0 | Perfect | Negative |

### Pearson Correlation Coefficient

**Formula (Computational):**
```
           n(Σxy) - (Σx)(Σy)
   r = -------------------------------------
       √[nΣx² - (Σx)²][nΣy² - (Σy)²]

Where:
n = Number of pairs
x = Values of variable 1
y = Values of variable 2
```

**Formula (Using Covariance):**
```
          Cov(X,Y)
   r = ------------
          σₓ × σ

Where:
Cov(X,Y) = Covariance between X and Y
σₓ = Standard deviation of X
σᵧ = Standard deviation of Y
```

**Example - Step by Step Calculation:**

**Problem:** Calculate correlation between Study Hours (X) and Exam Scores (Y)

```
Student  Hours(X)  Score(Y)
   1         2         50
   2         4         60
   3         6         70
   4         8         80
   5        10         90
```

**Solution:**
```
Step 1: Create calculation table

Student   X    Y    X²    Y²    XY
   1      2   50    4   2500   100
   2      4   60   16   3600   240
   3      6   70   36   4900   420
   4      8   80   64   6400   640
   5     10   90  100   8100   900
-----------------------------------
Σ       30  350  220  25500  2300

n = 5

Step 2: Apply formula

           n(Σxy) - (Σx)(Σy)
   r = -------------------------------------
       √[nΣx² - (Σx)²][nΣy² - (Σy)²]

           5(2300) - (30)(350)
   r = ---------------------------------
       √[5(220) - (30)²][5(25500) - (350)²]

           11500 - 10500
   r = -------------------------------
       √[1100 - 900][127500 - 122500]

           1000
   r = -------------------
       √[200][5000]

           1000
   r = -------------
       √1,000,000

           1000
   r = --------- = 1.0
       1000

Answer: r = 1.0 (Perfect positive correlation)

Interpretation: There is a perfect positive linear relationship 
between study hours and exam scores in this dataset.
```

### Spearman Rank Correlation (ρ)

**Definition:** Used for **monotonic** relationships and **ordinal (ranked)** data.

**Characteristics:**
- Resists non-normal distributions
- Based on ranks, not raw values
- Also ranges from -1 to +1

**When to Use:**
- Data is ordinal
- Relationship is monotonic but not linear
- Data has outliers
- Data is not normally distributed

### Coefficient of Determination (R²)

**Definition:** Square of correlation coefficient. Indicates the **proportion of variance explained** by the relationship.

**Formula:**
```
   R² = r²
```

**Interpretation:**
- R² = 0.81 means **81% of variance in Y is explained by X**
- Remaining 19% is due to other factors

**Example:**

**Problem:** If r = 0.85, calculate and interpret R²

**Solution:**
```
R² = (0.85)² = 0.7225 = 72.25%

Interpretation: 72.25% of the variation in the dependent variable 
is explained by the independent variable. The remaining 27.75% 
is due to other unmeasured factors.
```

**Example - Stress and Sleep:**

**Problem:** Correlation between stress levels and sleep hours is r = -0.68

**Solution:**
```
a) Interpretation of r:
   There is a moderate negative linear correlation.
   As stress goes up, sleep hours go down.

b) Calculate R²:
   R² = (-0.68)² = 0.4624 = 46.24%

c) Implication:
   46.24% of the variation in sleep hours is explained by stress levels.
   The other 53.76% is due to other unmeasured factors 
   (diet, exercise, caffeine, etc.)
```

---

## 2.2 REGRESSION

### What is Regression?

**Definition:** A statistical model representing the **functional relationship** between variables, used to **predict** the value of a dependent variable (Y) based on independent variables (X).

**Key Differences from Correlation:**

| Correlation | Regression |
|-------------|------------|
| Measures strength of relationship | Models functional relationship |
| Symmetric (X to Y = Y to X) | Asymmetric (X → Y) |
| Single value (r) | Equation (Y = a + bX) |
| No prediction | Enables prediction |

### Regression Line

**Definition:** A straight line that best summarizes the relationship between two variables, also known as the **"line of best fit."**

**Equation:**
```
   Ŷ = a + bX

Where:
Ŷ = Predicted value of Y
a = Y-intercept
b = Slope
X = Independent variable
```

### Least Squares Regression Line

**Principle:** Finds a line that **minimizes the sum of squared vertical distances (residuals)** between data points and the regression line.

**Formula:**
```
   Minimize: Σ(Y - Ŷ)²

Where:
Y = Actual value
Ŷ = Predicted value
```

### Calculating Slope and Intercept

**Slope (b):**
```
           n(ΣXY) - (ΣX)(ΣY)
   b = -----------------------
           nΣX² - (ΣX)²

Alternative formula:
         Σ(x - x̄)(y - ȳ)
   b = -------------------
           Σ(x - x̄)²
```

**Intercept (a):**
```
         ΣY        ΣX
   a = ----- - b(-----)
          n         n

Or simply:
   a = ȳ - b(x̄)
```

**Interpretation:**

**Slope (b):**
- Change in Y for a **one-unit increase in X**
- Positive b: Y increases as X increases
- Negative b: Y decreases as X increases

**Intercept (a):**
- Predicted value of Y when **X = 0**
- May not always be meaningful

**Example - Complete Calculation:**

**Problem:** Find regression equation for:

```
X (Hours):  2,  4,  6,  8, 10
Y (Score): 50, 60, 70, 80, 90
```

**Solution:**
```
Step 1: Create calculation table

   X    Y    X²    Y²    XY
   2   50    4   2500   100
   4   60   16   3600   240
   6   70   36   4900   420
   8   80   64   6400   640
  10   90  100   8100   900
----------------------------
  30  350  220  25500  2300

n = 5
ΣX = 30
ΣY = 350
ΣX² = 220
ΣY² = 25500
ΣXY = 2300

Step 2: Calculate means
x̄ = 30/5 = 6
ȳ = 350/5 = 70

Step 3: Calculate slope (b)

           n(ΣXY) - (ΣX)(ΣY)
   b = -----------------------
           nΣX² - (ΣX)²

           5(2300) - (30)(350)
   b = -------------------------
           5(220) - (30)²

           11500 - 10500
   b = -------------------
           1100 - 900

           1000
   b = -------- = 5
           200

Step 4: Calculate intercept (a)

   a = ȳ - b(x̄)
   a = 70 - 5(6)
   a = 70 - 30
   a = 40

Step 5: Write equation

   Ŷ = 40 + 5X

Interpretation:
- Intercept (40): Base score with 0 hours of study
- Slope (5): Each additional hour increases score by 5 points

Step 6: Make prediction

Predict score for 7 hours of study:
Ŷ = 40 + 5(7) = 40 + 35 = 75

Answer: Predicted score = 75
```

### Finding Equation from Means and SDs

**When given:**
- x̄, ȳ (means)
- Sₓ, S (standard deviations)
- r (correlation)

**Formula for slope:**
```
              Sᵧ
   b = r × -------
              Sₓ
```

**Example:**

**Problem:** Given: x̄ = 5, ȳ = 10, Sₓ = 2, Sᵧ = 4, r = 0.75
Find regression equation and predict Y when X = 8

**Solution:**
```
Step 1: Calculate slope (b)

         Sᵧ          4
   b = r × --- = 0.75 × --- = 0.75 × 2 = 1.5
         Sₓ          2

Step 2: Calculate intercept (a)

   a = ȳ - b(x̄)
   a = 10 - 1.5(5)
   a = 10 - 7.5
   a = 2.5

Step 3: Write equation

   Ŷ = 2.5 + 1.5X

Step 4: Predict Y when X = 8

   Ŷ = 2.5 + 1.5(8)
   Ŷ = 2.5 + 12
   Ŷ = 14.5

Answer: 
Regression equation: Ŷ = 2.5 + 1.5X
Predicted Y when X = 8: 14.5
```

### Limitations of Regression

1. **Doesn't prove causation**
   - Correlation ≠ Causation
   - Need experimental design for causality

2. **Extrapolation is unreliable**
   - Predicting outside data range is dangerous
   - Relationship may not hold beyond observed data

3. **Highly sensitive to outliers**
   - Single outlier can drastically change line
   - Always check for outliers

4. **Only fits linear patterns**
   - Cannot capture curved relationships
   - Need polynomial or non-linear regression

---

## 2.3 STANDARD ERROR OF ESTIMATE (SEE)

### Definition

**Standard Error of Estimate (SEE)** measures **prediction accuracy** by finding the **average distance between observed values and predicted values** on the regression line.

**Formula:**
```
           Σ(Y - Ŷ)²
   SEE = √-----------
             n - 2

Where:
Y = Actual value
Ŷ = Predicted value
n = Number of observations
```

### Interpretation

**Key Points:**
- **Smaller SEE = Better predictions** (points are closer to the line)
- Expressed in the **same units as Y** (unlike R² which is a percentage)
- Used to create **prediction intervals**

**Relationship with R²:**
- Higher R² (more variance explained) → Lower SEE
- Lower R² (less variance explained) → Higher SEE

### When to Use

**Use SEE when:**
- You need prediction intervals in actual units
- Comparing models with same Y variable

**Use R² when:**
- Comparing overall model fit
- Explaining variance to stakeholders

**Example:**

**Problem:** Given regression predictions:

```
Actual(Y)  Predicted(Ŷ)
   50          45
   60          62
   70          68
   80          83
   90          87
```

Calculate SEE

**Solution:**
```
Step 1: Calculate residuals (Y - Ŷ)

Y    Ŷ    (Y - Ŷ)    (Y - Ŷ)²
50   45      5          25
60   62     -2           4
70   68      2           4
80   83     -3           9
90   87      3           9
-------------------------
Σ(Y - Ŷ)² = 51

Step 2: Calculate SEE

           Σ(Y - Ŷ)²        51
   SEE = √----------- = √------- = √17 = 4.12
             n - 2          5-2

Interpretation: On average, predictions are off by about 
4.12 units.
```

---

## 2.4 MULTIPLE REGRESSION EQUATIONS

### From Simple to Multiple Regression

**Simple Regression:**
```
   Ŷ = β₀ + β₁X

• One predictor variable
• Fits a straight line
• Example: Height → Weight
```

**Multiple Regression:**
```
   Ŷ = β₀ + β₁X₁ + β₂X₂ + ... + βₙXₙ

• Multiple predictor variables
• Fits a hyperplane in n-dimensions
• Explains more variance in Y
• Example: Height + Age + Diet → Weight
```

### Anatomy of the Multiple Regression Equation

```
   Ŷ = β₀ + β₁X₁ + β₂X₂ + β₃X₃ + ε

Where:

Ŷ (Predicted Value)
└─ Our model's best estimate of the outcome variable

β₀ (Intercept)
└─ Value of Ŷ when ALL predictors = 0
   The baseline starting point

β₁, β₂, β₃ (Coefficients)
└─ Change in Ŷ for a 1-unit increase in X₁, X₂, X₃
   Keeping all other variables constant
   This is the POWER of multiple regression!

X₁, X₂, X₃ (Predictors/Features)
└─ The independent variables (inputs)
   Can be continuous, ordinal, or dummy-coded

ε (Error Term)
└─ Residual - the part of Y we can't explain
   Assumed to be normally distributed
```

### Worked Example: Predicting House Price

**Scenario:** Predict house price (in ₹ lakhs) using size, age, and number of bedrooms

**Regression Equation:**
```
Price = 10 + 0.8(Size m²) - 0.5(Age yrs) + 3.2(Bedrooms)
```

**Interpretation of Coefficients:**

```
β₀ = 10
└─ Base price: ₹10 lakhs when all inputs = 0

β₁ = +0.8
└─ Each extra m² of size adds ₹0.8 lakhs to price

β₂ = -0.5
└─ Each year older reduces price by ₹0.5 lakhs

β₃ = +3.2
└─ Each extra bedroom adds ₹3.2 lakhs to price
```

**Prediction Example:**

**Problem:** Calculate price for a 120 m² house, 5 years old, 3 bedrooms

**Solution:**
```
Price = 10 + 0.8(120) - 0.5(5) + 3.2(3)
Price = 10 + 96 - 2.5 + 9.6
Price = 113.1

Answer: ₹113.1 Lakhs
```

**Key Insight:**
Each coefficient tells you the **isolated effect** of one variable while all others stay constant. This is the power of multiple regression!

### Key Assumptions of Multiple Regression

**Statistical Assumptions:**

**1. Linearity**
- Relationship between each Xᵢ and Y is linear
- **Check**: Scatter plots, residual vs. fitted plots

**2. Independence**
- Observations are independent of each other
- Important for time-series data
- **Check**: Durbin-Watson test

**3. Normality of Errors**
- Errors (residuals) follow a normal distribution
- **Check**: Q-Q plot, Shapiro-Wilk test

**4. Homoscedasticity**
- Residuals have constant variance across all fitted values
- **Check**: Residuals vs. Fitted plot (no funnel shape)

**Data Assumptions:**

**5. No Multicollinearity**
- Predictors should not be highly correlated with each other
- **Check**: Variance Inflation Factor (VIF < 10)

**6. Sufficient Sample Size**
- Rule of thumb: At least 10-20 observations per predictor

**7. No Outliers**
- Extreme values can unduly influence results
- **Check**: Residual plots, leverage statistics

### Checking for Multicollinearity

**Variance Inflation Factor (VIF):**
```
          1
VIF = ----------
      1 - R²ⱼ

Where R²ⱼ is from regressing Xⱼ on other predictors

Interpretation:
VIF = 1    : No multicollinearity
VIF < 5    : Moderate (acceptable)
VIF > 10   : High (problematic)
```

---

## 2.5 REGRESSION TOWARDS THE MEAN

### Definition

**Regression to the Mean (RTM)** is the tendency for **extreme measurements to move closer to the average** on a subsequent measurement, due to **natural random variation** - NOT because of any real change.

### Why It Occurs

**Key Concepts:**

1. **Random Variation**
   - Any measurement contains: **True Score + Random Error**
   - Extreme scores have unusually large errors

2. **Imperfect Correlation**
   - Perfect correlation (r = 1) rarely exists
   - Most measurements have r < 1

3. **Not Causal!**
   - Does NOT mean interventions caused the change
   - Mixing RTM with causation is a common statistical error

### Historical Context

**Francis Galton (1886)**
- First described RTM while studying heights of parents and children
- Found: Tall parents have tall children - but **closer to average height** than the parents
- Coined the term "regression"

### Visualizing Regression to the Mean

```
Attempt 1 Scores vs Attempt 2 Scores

High │  ●●                    ●
     │    ●●                ●
     │      ●●            ●
     │        ●●        ●
Mean │──────────●●────●─────────
     │            ●●●
     │              ●●●
     │                ●●●
Low  │                  ●●●●
     └───────────────────────────
       Low    Mean      High
            Attempt 1

← Extreme HIGH scorers in Attempt 1 tend to score LOWER in Attempt 2
← Extreme LOW scorers in Attempt 1 tend to score HIGHER in Attempt 2
← Average scorers stay near average
← This happens purely due to random variation!
```

### The Mathematics of Regression to the Mean

**Formula:**
```
   E[Y₂ | Y₁] = μ + ρ × (Y₁ - μ)

Where:
E[Y₂ | Y₁] = Expected 2nd measurement given 1st
μ          = Population mean
ρ (rho)    = Correlation between measurements (0 to 1)
Y₁ - μ     = Deviation from mean
```

**Interpretation:**

```
μ (Population Mean)
└─ The true average of all scores
   Both extreme and average scores drift toward this

ρ (Correlation)
└─ If ρ = 1: No RTM (perfect reliability)
   If ρ = 0: Full RTM (complete randomness)
   In practice: 0 < ρ < 1

(Y₁ - μ) (Deviation from Mean)
└─ How far the first score is from the mean
   Larger deviation = more regression toward mean
```

**Key Insight:**
The **further Y₁ is from the mean** AND the **weaker the correlation**, the **stronger the regression to the mean effect**.

### Real-World Examples

**1. Sports - Sophomore Slump**

**Scenario:** A cricketer has a record-breaking debut season

**What Happens:**
- Next season is less impressive
- Was it a slump or just RTM?

**Common Mistake:**
- Analyst blames extra practice for "fixing the slump"
- But the drop and recovery were statistical, not causal

**2. Medicine - Patient Blood Pressure**

**Scenario:** Patients with dangerously high BP enrolled in study

**What Happens:**
- After 2 weeks, BP drops - even in placebo group!

**Common Mistake:**
- Doctors credit the treatment
- But patients with extreme readings tend to have more moderate readings on follow-up naturally

**3. Education - Tutoring Studies**

**Scenario:** Students who scored in bottom 10% enrolled in tutoring

**What Happens:**
- Scores improve

**Common Mistake:**
- Is it the tutoring? Maybe!
- But part of the gain is RTM
- Need a control group to isolate true tutoring effect

**4. Finance - Fund Manager Performance**

**Scenario:** Top-performing mutual funds in Year 1

**What Happens:**
- Often perform near-average in Year 2
- The "curse of the top performer"

**Common Mistake:**
- Investors assume strategy shift is needed
- But it could simply be RTM in action

### The RTM Fallacy

**Definition:** Attributing regression to the mean to an "intervention" or "treatment"

**Example:**
```
Scenario: Student scores 95% on first test
          Scores 85% on second test

Wrong Conclusion: "Tutoring made the student worse!"

Correct Understanding: The first score was unusually high
                       (luck + ability). Second score 
                       regressed toward true ability.
```

### How to Avoid RTM Mistakes

**Solutions:**

1. **Use Control Groups**
   - Compare treatment group to similar group without treatment
   - Both groups will show RTM
   - Difference shows true treatment effect

2. **Multiple Measurements**
   - Take baseline average of several measurements
   - Reduces impact of random variation

3. **Random Assignment**
   - Randomly assign subjects to groups
   - Ensures RTM affects all groups equally

4. **Understand the Phenomenon**
   - Be aware RTM exists
   - Question extreme-to-moderate changes

---

## 2.6 BASICS OF NUMPY ARRAYS

### What is a NumPy Array?

**Definition:** NumPy (Numerical Python) is the foundation of scientific Python computing.

**Key Characteristics:**
- **ndarray**: N-dimensional array object
- **Homogeneous data type** (dtype) - all elements same type
- **Fixed size** at creation time
- **Shape**: (rows, cols, ...)

**Advantages over Python Lists:**
- Faster operations
- Less memory
- Vectorized operations
- Built-in mathematical functions

### Creating NumPy Arrays

**Basic Creation:**

```python
import numpy as np

# 1D Array
a = np.array([1, 2, 3, 4, 5])
print(a)
# Output: [1 2 3 4 5]

# 2D Array
b = np.array([[1, 2, 3],
              [4, 5, 6]])
print(b)
# Output: [[1 2 3]
#          [4 5 6]]
```

**Special Arrays:**

```python
# All zeros
np.zeros((3, 3))
# Output: [[0. 0. 0.]
#          [0. 0. 0.]
#          [0. 0. 0.]]

# All ones
np.ones((2, 4))
# Output: [[1. 1. 1. 1.]
#          [1. 1. 1. 1.]]

# Range with step
np.arange(0, 10, 2)
# Output: [0 2 4 6 8]

# Evenly spaced values
np.linspace(0, 1, 5)
# Output: [0.   0.25 0.5  0.75 1.  ]

# Random 3x3 array
np.random.rand(3, 3)
# Output: Random values between 0 and 1
```

### Key Attributes

```python
arr = np.array([[1, 2, 3],
                [4, 5, 6]])

arr.shape   # (2, 3) - 2 rows, 3 columns
arr.ndim    # 2 - number of dimensions
arr.dtype   # int64 or int32 - data type
arr.size    # 6 - total number of elements
```

---

## 2.7 AGGREGATIONS

### What are Aggregations?

**Definition:** Functions that summarize data by computing a single value from an array.

### Common Aggregation Functions

```
Σ (Sum)           np.sum(a)      - Total of all elements
μ (Mean)          np.mean(a)     - Average value
σ (Std Dev)       np.std(a)      - Standard deviation
min/max           np.min/max(a)  - Minimum/Maximum value
Median            np.median(a)   - Middle value
Cumulative Sum    np.cumsum(a)   - Running total
```

### Examples

**Basic Aggregations:**

```python
import numpy as np

a = np.array([[1, 2, 3],
              [4, 5, 6]])

# Sum of all elements
np.sum(a)  # Output: 21

# Sum along axis 0 (column sums)
np.sum(a, axis=0)  # Output: [5 7 9]
# Column 0: 1+4=5
# Column 1: 2+5=7
# Column 2: 3+6=9

# Sum along axis 1 (row sums)
np.sum(a, axis=1)  # Output: [6 15]
# Row 0: 1+2+3=6
# Row 1: 4+5+6=15

# Mean
np.mean(a)  # Output: 3.5

# Standard Deviation
np.std(a)  # Output: 1.708

# Minimum and Maximum
np.min(a)  # Output: 1
np.max(a)  # Output: 6

# Median
np.median(a)  # Output: 3.5
```

**Understanding Axis:**

```
2D Array:
         Axis 1 →
       ┌───────────┐
Axis 0 │ 1   2   3 │
  ↓    │ 4   5   6 │
       └───────────┘

axis=0: Operate down columns
axis=1: Operate across rows
```

---

## 2.8 COMPUTATIONS ON ARRAYS

### Universal Functions (ufuncs)

**Definition:** Functions that operate element-wise on arrays.

**Common ufuncs:**

```python
import numpy as np

a = np.array([1, 2, 3, 4])

# Square root
np.sqrt(a)
# Output: [1.   1.41 1.73 2.  ]

# Natural logarithm
np.log(a)
# Output: [0.    0.69  1.1   1.39]

# Exponential (e^x)
np.exp(a)
# Output: [ 2.72  7.39 20.09 54.6 ]

# Trigonometric functions
np.sin(a)
np.cos(a)

# Power
np.power(a, 2)
# Output: [ 1  4  9 16]

# Absolute value
np.abs(np.array([-1, -2, 3]))
# Output: [1 2 3]
```

### Element-wise Operations

```python
a = np.array([1, 2, 3])
b = np.array([10, 20, 30])

# Addition
a + b  # Output: [11 22 33]

# Multiplication
a * b  # Output: [10 40 90]

# Subtraction
b - a  # Output: [ 9 18 27]

# Division
b / a  # Output: [10. 10. 10.]

# Power
a ** 2  # Output: [1 4 9]
```

### Broadcasting

**Definition:** Smaller arrays are automatically "stretched" to match larger array shapes for element-wise operations.

**Example 1 - Array + Scalar:**

```python
a = np.array([1, 2, 3])
a + 10
# Output: [11 12 13]
# 10 is "broadcast" to [10, 10, 10]
```

**Example 2 - 2D Array + 1D Array:**

```python
M = np.ones((3, 3))
v = np.array([1, 2, 3])

M + v
# Output: [[2. 3. 4.]
#          [2. 3. 4.]
#          [2. 3. 4.]]
# v is added to each row
```

**Broadcasting Rules:**
1. Arrays are aligned right-to-left
2. Dimensions must be equal or one must be 1
3. Smaller array is "stretched" to match

---

## 2.9 COMPARISONS, MASKS, BOOLEAN LOGIC

### Comparison Operators

```
<   Less than
>   Greater than
<=  Less than or equal
>=  Greater than or equal
==  Equal to
!=  Not equal
```

### Boolean Masks

**Definition:** Arrays of True/False values used to filter data.

**Example:**

```python
import numpy as np

a = np.array([1, 2, 3, 4, 5, 6])

# Comparison creates boolean mask
a > 3
# Output: [False False False  True  True  True]

# Use mask to filter
a[a > 3]
# Output: [4 5 6]

# Count True values
np.sum(a > 3)  # Output: 3

# Check if any True
np.any(a > 5)  # Output: True

# Check if all True
np.all(a > 0)  # Output: True
```

### Combining Conditions

**Logical Operators:**

```
&   AND
|   OR
~   NOT
```

**Example:**

```python
a = np.array([1, 2, 3, 4, 5, 6])

# AND: Values between 2 and 5
a[(a > 2) & (a < 5)]
# Output: [3 4]
# Note: Must use parentheses!

# OR: Values less than 2 OR greater than 5
a[(a < 2) | (a > 5)]
# Output: [1 6]

# NOT: Values NOT equal to 3
a[~(a == 3)]
# Output: [1 2 4 5 6]
```

### Real-World Applications

**1. Filter exam scores:**

```python
scores = np.array([45, 67, 38, 82, 55, 91])
passed = scores[scores >= 40]
# Output: [45 67 82 55 91]
```

**2. Find negative temperatures:**

```python
temps = np.array([5, -2, 8, -5, 12, -1])
below_freezing = temps[temps < 0]
# Output: [-2 -5 -1]
```

**3. Select high sales:**

```python
sales = np.array([500, 1200, 800, 1500, 300])
high_sales = sales[sales > 1000]
# Output: [1200 1500]
```

**💡 Important Tip:**
Always wrap compound conditions in parentheses:
```python
# Correct:
a[(a > 2) & (a < 5)]

# Wrong:
a[a > 2 & a < 5]  # Error!
```

---

## 2.10 FANCY INDEXING

### What is Fancy Indexing?

**Definition:** Accessing multiple elements using arrays of indices instead of single values or slices.

**Key Difference:**
- **Basic Indexing**: Returns a VIEW
- **Fancy Indexing**: Returns a COPY

### Types of Indexing

```
Basic Indexing:
  a[2]        → Single element
  a[1:4]      → Contiguous range

Boolean Mask:
  a[a > 2]    → Condition-based

Fancy Indexing:
  a[[1,3,0]]  → Any index list
```

### Examples

**1D Array Indexing:**

```python
import numpy as np

a = np.array([10, 20, 30, 40, 50])

# Integer array indexing
idx = [0, 2, 4]
a[idx]
# Output: [10 30 50]

# Direct indexing
a[[1, 3]]
# Output: [20 40]

# With repetition
a[[0, 0, 2, 2]]
# Output: [10 10 30 30]
```

**2D Fancy Indexing:**

```python
X = np.arange(12).reshape(4, 3)
# X = [[ 0  1  2]
#      [ 3  4  5]
#      [ 6  7  8]
#      [ 9 10 11]]

# Select specific elements
rows = [0, 1, 3]
cols = [2, 1, 0]

X[rows, cols]
# Output: [2 4 9]
# X[0,2] = 2
# X[1,1] = 4
# X[3,0] = 9

# Select entire rows
X[[1, 3], :]
# Output: [[ 3  4  5]
#          [ 9 10 11]]

# Select entire columns
X[:, [0, 2]]
# Output: [[ 0  2]
#          [ 3  5]
#          [ 6  8]
#          [ 9 11]]
```

**Important Note:**

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

---

## 2.11 STRUCTURED ARRAYS

### What are Structured Arrays?

**Definition:** Arrays with **named fields** of **different data types** - like a lightweight table.

**Use Cases:**
- Tabular data with mixed types
- Record arrays (like CSV rows)
- Scientific data (particle data)
- Memory-efficient vs Python dicts

### Creating Structured Arrays

**Example:**

```python
import numpy as np

# Define structure (dtype)
dt = np.dtype([
    ('name', 'U10'),   # Unicode 10 chars
    ('age', 'i4'),     # 32-bit int
    ('score', 'f8')    # 64-bit float
])

# Create array
data = np.array([
    ('Alice', 25, 92.5),
    ('Bob',   30, 85.0),
    ('Carol', 22, 97.3)
], dtype=dt)

print(data)
# Output:
# [('Alice', 25, 92.5) ('Bob', 30, 85. ) ('Carol', 22, 97.3)]
```

### Accessing Fields

```python
# Access by field name
data['name']
# Output: ['Alice' 'Bob' 'Carol']

data['score']
# Output: [92.5 85.  97.3]

# Boolean filtering
data['score'] > 90
# Output: [ True False  True]

data[data['age'] < 28]
# Output: [('Alice', 25, 92.5) ('Carol', 22, 97.3)]

# Access individual record
data[0]
# Output: ('Alice', 25, 92.5)

data[0]['name']
# Output: 'Alice'
```

**Field Type Codes:**

```
'U10'  - Unicode string, 10 characters
'i4'   - 32-bit integer
'i8'   - 64-bit integer
'f4'   - 32-bit float
'f8'   - 64-bit float
'b1'   - Boolean
```

---

## 2.12 DATA MANIPULATION WITH PANDAS

### Introduction to Pandas

**Pandas** is a powerful data manipulation and analysis library built on NumPy.

**Key Data Structures:**
1. **Series** - 1D labeled array
2. **DataFrame** - 2D table (like Excel/SQL)

### Series

```python
import pandas as pd

# Create Series
s = pd.Series([10, 20, 30], index=['a', 'b', 'c'])

print(s)
# Output:
# a    10
# b    20
# c    30
# dtype: int64

# Access by label
s['b']  # Output: 20

# Access by position
s.iloc[1]  # Output: 20
```

### DataFrame

**Creation:**

```python
# Create DataFrame
df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Carol'],
    'Age': [25, 30, 35],
    'Score': [92.5, 85.0, 88.5]
})

print(df)
# Output:
#     Name  Age  Score
# 0  Alice   25   92.5
# 1    Bob   30   85.0
# 2  Carol   35   88.5
```

**Essential DataFrame Methods:**

```python
df.head(n)        # First n rows
df.tail(n)        # Last n rows
df.info()         # Data types & nulls
df.describe()     # Summary statistics
df.shape          # (rows, columns)
df.dtypes         # Column data types
df.isnull()       # Find missing values
df.columns        # Column names
df.index          # Row indices
```

### Selecting Data

**Column Selection:**

```python
# Single column (returns Series)
df['Age']

# Multiple columns (returns DataFrame)
df[['Name', 'Score']]
```

**Row Selection:**

```python
# By label
df.loc[0]          # Row with label 0
df.loc[0:2]        # Rows 0 to 2 (inclusive)

# By position
df.iloc[1]         # Row at position 1
df.iloc[1:3]       # Rows 1 to 2 (position 3 exclusive)
```

**loc vs iloc:**

```
loc  - Label based indexing
iloc - Position based indexing (0-indexed)
```

### Filtering Data

```python
# Single condition
df[df['Age'] > 25]
# Output:
#     Name  Age  Score
# 1    Bob   30   85.0
# 2  Carol   35   88.5

# Multiple conditions
df[(df['Age'] > 25) & (df['Score'] > 85)]

# Using between()
df[df['Score'].between(85, 90)]

# Using isin()
df[df['Name'].isin(['Alice', 'Bob'])]
```

### Adding/Modifying Columns

```python
# Add new column
df['Grade'] = df['Score'].apply(
    lambda x: 'A' if x >= 90 else 'B'
)

# Output:
#     Name  Age  Score Grade
# 0  Alice   25   92.5     A
# 1    Bob   30   85.0     B
# 2  Carol   35   88.5     B

# Modify existing column
df['Age'] = df['Age'] + 1

# Drop column
df.drop('Grade', axis=1, inplace=True)
```

### Sorting

```python
# Sort by single column
df.sort_values('Score')  # Ascending
df.sort_values('Score', ascending=False)  # Descending

# Sort by multiple columns
df.sort_values(['Age', 'Score'])
```

### GroupBy Operations

**Split-Apply-Combine Pattern:**

```python
df = pd.DataFrame({
    'Dept': ['HR', 'IT', 'HR', 'IT', 'HR'],
    'Emp': ['A', 'B', 'C', 'D', 'E'],
    'Salary': [50, 80, 55, 90, 60],
    'Yrs': [2, 5, 3, 7, 4]
})

# Group by and aggregate
df.groupby('Dept')['Salary'].mean()
# Output:
# Dept
# HR    55.0
# IT    85.0
# Name: Salary, dtype: float64

# Multiple aggregations
df.groupby('Dept').agg({
    'Salary': ['mean', 'max', 'sum'],
    'Yrs': 'mean'
})

# Named aggregations (pandas >= 0.25)
df.groupby('Dept').agg(
    avg_sal=('Salary', 'mean'),
    max_sal=('Salary', 'max'),
    headcount=('Emp', 'count')
)
```

### Missing Values

```python
# Check for missing values
df.isnull()
df.isnull().sum()

# Remove missing values
df.dropna()  # Drop rows with any NaN
df.dropna(axis=1)  # Drop columns with NaN

# Fill missing values
df.fillna(0)  # Replace with 0
df.fillna(df.mean())  # Replace with mean
df.fillna(method='ffill')  # Forward fill
df.fillna(method='bfill')  # Backward fill
```

### Merging DataFrames

```python
df1 = pd.DataFrame({
    'ID': [1, 2],
    'Name': ['Alice', 'Bob']
})

df2 = pd.DataFrame({
    'ID': [2, 3],
    'Score': [90, 85]
})

# Inner join
pd.merge(df1, df2, on='ID')
# Output:
#    ID   Name  Score
# 0   2    Bob     90

# Left join
pd.merge(df1, df2, on='ID', how='left')

# Outer join
pd.merge(df1, df2, on='ID', how='outer')
```

---

# 📖 MODULE 3: DATA WRANGLING AND DATA VISUALIZATION

## 3.1 DATA INDEXING AND SELECTION

### Pandas Indexing Methods

Pandas provides multiple ways to access rows, columns, and specific data points.

### 1. .loc[] - Label-based Selection

**Purpose:** Select rows/columns by their **labels** (index names or column names).

**Syntax:**
```python
df.loc[row_label, column_label]
```

**Examples:**

```python
import pandas as pd

df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Carol'],
    'Age': [25, 30, 35],
    'Score': [88, 92, 79]
})

# Select single cell by label
df.loc[0, 'Name']
# Output: 'Alice'

# Select multiple rows
df.loc[0:1]
# Output:
#     Name  Age  Score
# 0  Alice   25     88
# 1    Bob   30     92

# Select specific rows and columns
df.loc[0:1, ['Name', 'Age']]
# Output:
#     Name  Age
# 0  Alice   25
# 1    Bob   30

# Select all rows, specific column
df.loc[:, 'Score']
# Output:
# 0    88
# 1    92
# 2    79
# Name: Score, dtype: int64

# Boolean indexing with loc
df.loc[df['Age'] > 25]
# Output:
#     Name  Age  Score
# 1    Bob   30     92
# 2  Carol   35     79
```

### 2. .iloc[] - Position-based Selection

**Purpose:** Select rows/columns by **integer position** (0-indexed).

**Syntax:**
```python
df.iloc[row_position, column_position]
```

**Examples:**

```python
# Select single cell by position
df.iloc[1, 2]
# Output: 92 (Bob's score)

# Select first 2 rows, all columns
df.iloc[:2, :]
# Output:
#     Name  Age  Score
# 0  Alice   25     88
# 1    Bob   30     92

# Select specific positions
df.iloc[[0, 2], [1, 2]]
# Output:
#    Age  Score
# 0   25     88
# 2   35     79

# Select last row
df.iloc[-1]
# Output:
# Name     Carol
# Age         35
# Score       79
# Name: 2, dtype: object
```

### 3. Boolean Masking

**Purpose:** Filter rows using True/False conditions.

**Examples:**

```python
# Single condition
df[df['Age'] > 25]
# Output: Bob and Carol

# Multiple conditions with AND
df[(df['Age'] > 25) & (df['Score'] > 80)]
# Output: Only Bob

# Multiple conditions with OR
df[(df['Age'] < 28) | (df['Score'] > 90)]
# Output: Alice and Bob

# Using isin()
df[df['Name'].isin(['Alice', 'Carol'])]
# Output: Alice and Carol
```

### 4. .at[] and .iat[] - Fast Scalar Access

**Purpose:** Fast access for **single cell** values.

**Examples:**

```python
# .at uses label
df.at[0, 'Name']
# Output: 'Alice'

# .iat uses position
df.iat[2, 1]
# Output: 35

# Faster than loc/iloc for single values
# Use for performance-critical code
```

**Comparison:**

```
.loc  - Label based, can select multiple
.iloc - Position based, can select multiple
.at   - Label based, single value only (faster)
.iat  - Position based, single value only (faster)
```

---

## 3.2 OPERATING ON DATA

### Vectorized Operations

**Definition:** Arithmetic operates **element-wise**; no loops needed.

**Examples:**

```python
import pandas as pd
import numpy as np

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

**Purpose:** Apply any function **row-wise or column-wise**.

**Examples:**

```python
# Apply to Series
df['Grade'] = df['Score'].apply(
    lambda x: 'A' if x >= 90 else 'B'
)
# Output:
# Score  Grade
#    88      B
#    92      A
#    79      B

# Apply to DataFrame
def normalize(col):
    return (col - col.mean()) / col.std()

df[['Age', 'Score']].apply(normalize)
# Returns standardized values

# Apply row-wise
df.apply(lambda row: row['Age'] + row['Score'], axis=1)
# Output: [113, 122, 114]
```

### map() and applymap()

**map() - Element-wise on Series:**

```python
# Transform Series
df['Name'] = df['Name'].map(str.upper)
# Output: ['ALICE', 'BOB', 'CAROL']

# Using dictionary mapping
grade_map = {'A': 4, 'B': 3, 'C': 2}
df['Grade_Point'] = df['Grade'].map(grade_map)
```

**applymap() - Element-wise on DataFrame:**

```python
# Round all values
df[['Age', 'Score']].applymap(lambda x: round(x, 2))

# Note: applymap() deprecated in newer pandas
# Use DataFrame.map() instead
```

### NumPy ufuncs on DataFrames

**Universal functions work directly:**

```python
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

## 3.3 MISSING DATA

### Detecting Missing Data

**Methods:**

```python
import numpy as np

df = pd.DataFrame({
    'A': [1, np.nan, 3],
    'B': [np.nan, 5, 6],
    'C': [7, 8, np.nan]
})

# Boolean mask
df.isnull()
# Output:
#        A      B      C
# 0  False   True  False
# 1   True  False  False
# 2  False  False   True

# Count missing per column
df.isnull().sum()
# Output:
# A    1
# B    1
# C    1
# dtype: int64

# Check if any missing
df.isnull().any().any()  # True

# Check if all values present
df.notnull().all().all()  # False

# Total missing
df.isnull().sum().sum()  # 3
```

### Removing Missing Data

**dropna() Method:**

```python
# Drop rows with ANY NaN
df.dropna()
# Output: Empty DataFrame (all rows have NaN)

# Drop columns with ANY NaN
df.dropna(axis=1)
# Output: Empty DataFrame

# Drop rows with ALL NaN
df.dropna(how='all')
# Output: Original df (no row has all NaN)

# Keep rows with ≥2 valid values
df.dropna(thresh=2)
# Output: All rows (each has 2 valid values)

# Drop only specific columns
df.dropna(subset=['A', 'B'])
```

### Filling Missing Data

**fillna() Method:**

```python
# Replace with scalar
df.fillna(0)
# Output: All NaN replaced with 0

# Replace with mean
df['A'].fillna(df['A'].mean())
# Output: NaN replaced with mean of A

# Replace with different values per column
df.fillna({'A': 0, 'B': 1, 'C': 2})

# Forward fill (use previous value)
df.fillna(method='ffill')
# Output:
#      A    B    C
# 0  1.0  NaN  7.0
# 1  1.0  5.0  8.0
# 2  3.0  6.0  8.0

# Backward fill (use next value)
df.fillna(method='bfill')
# Output:
#      A    B    C
# 0  1.0  5.0  7.0
# 1  3.0  5.0  8.0
# 2  3.0  6.0  8.0

# Limit filling
df.fillna(method='ffill', limit=1)
```

### Interpolation

**For numerical series:**

```python
# Linear interpolation
df['B'].interpolate()
# Output: [NaN, 5.0, 6.0]
# NaN at start remains

# Full interpolation
df.interpolate()
# Output:
#      A    B    C
# 0  1.0  NaN  7.0
# 1  2.0  5.0  8.0
# 2  3.0  6.0  8.0

# Different methods
df.interpolate(method='linear')
df.interpolate(method='polynomial', order=2)
df.interpolate(method='time')
```

---

## 3.4 HIERARCHICAL INDEXING (MULTIINDEX)

### What is MultiIndex?

**Definition:** A MultiIndex allows you to have **multiple levels** in a row or column index, enabling storage and manipulation of higher-dimensional data in a 2D DataFrame.

**Why Use It:**
- Represent panel/grouped data naturally
- Perform partial indexing on any level
- Enable cross-section selection with .xs()
- Reshape data easily

### Creating MultiIndex

**Method 1: From Tuples:**

```python
import pandas as pd

index = pd.MultiIndex.from_tuples([
    ('2023', 'Q1'),
    ('2023', 'Q2'),
    ('2024', 'Q1'),
    ('2024', 'Q2')
], names=['Year', 'Quarter'])

df = pd.DataFrame({
    'Sales': [100, 120, 130, 150],
    'Profit': [20, 25, 28, 35]
}, index=index)

print(df)
# Output:
#               Sales  Profit
# Year Quarter               
# 2023 Q1          100      20
#      Q2          120      25
# 2024 Q1          130      28
#      Q2          150      35
```

**Method 2: From Arrays:**

```python
index = pd.MultiIndex.from_arrays([
    ['A', 'A', 'B', 'B'],
    [1, 2, 1, 2]
], names=['Group', 'Num'])
```

**Method 3: From DataFrame:**

```python
df2 = pd.DataFrame({
    'Year': [2023, 2023, 2024, 2024],
    'Quarter': ['Q1', 'Q2', 'Q1', 'Q2'],
    'Sales': [100, 120, 130, 150]
})

df2.set_index(['Year', 'Quarter'])
```

### Partial Indexing

**Select by first level:**

```python
# All 2023 rows
df.loc['2023']
# Output:
#         Sales  Profit
# Quarter              
# Q1          100      20
# Q2          120      25
```

**Select by multiple levels:**

```python
# Specific year and quarter
df.loc[('2023', 'Q1')]
# Output:
# Sales     100
# Profit     20
# Name: (2023, Q1), dtype: int64
```

### Cross-Section Selection

**Using .xs() method:**

```python
# All Q1 rows (across all years)
df.xs('Q1', level='Quarter')
# Output:
#       Sales  Profit
# Year               
# 2023    100      20
# 2024    130      28

# By level number
df.xs('Q1', level=1)
```

### Reset and Set Index

```python
# Flatten MultiIndex to columns
df.reset_index()
# Output:
#    Year Quarter  Sales  Profit
# 0  2023      Q1    100      20
# 1  2023      Q2    120      25
# 2  2024      Q1    130      28
# 3  2024      Q2    150      35

# Set columns as index
df2.set_index(['Year', 'Quarter'])
```

### Stack and Unstack

**stack() - Move column level to row level:**

```python
df_stacked = df.stack()
# Moves columns to index
```

**unstack() - Move row level to column level:**

```python
# Unstack Quarter level
df.unstack('Quarter')
# Output:
#       Sales      Profit     
# Quarter    Q1   Q2       Q1  Q2
# Year                          
# 2023      100  120       20  25
# 2024      130  150       28  35

# Unstack by level number
df.unstack(level=1)
```

---

## 3.5 COMBINING DATASETS

### Three Ways to Unite DataFrames

```
1. concat()  - Stack vertically or side-by-side
2. merge()   - SQL-style joins on key columns
3. join()    - Index-based joining
```

### 1. pd.concat()

**Purpose:** Stack DataFrames **vertically** (axis=0) or **side-by-side** (axis=1).

**Examples:**

```python
df1 = pd.DataFrame({
    'ID': [1, 2],
    'Name': ['Alice', 'Bob']
})

df2 = pd.DataFrame({
    'ID': [2, 3],
    'Score': [90, 85]
})

df3 = pd.DataFrame({
    'X': [10, 20]
}, index=[1, 2])

# Vertical stack (default)
pd.concat([df1, df2])
# Output:
#    ID   Name  Score
# 0   1  Alice    NaN
# 1   2    Bob    NaN
# 0   2    NaN   90.0
# 1   3    NaN   85.0

# Side-by-side (axis=1)
pd.concat([df1, df3], axis=1)
# Output:
#    ID   Name     X
# 0   1  Alice  10.0
# 1   2    Bob  20.0

# Reset index
pd.concat([df1, df2], ignore_index=True)
# Output: Index becomes 0,1,2,3

# Add keys for identification
pd.concat([df1, df2], keys=['First', 'Second'])
```

**Parameters:**
- `axis`: 0 (rows) or 1 (columns)
- `ignore_index`: Reset index
- `keys`: Add hierarchical index
- `join`: 'outer' (default) or 'inner'

### 2. pd.merge()

**Purpose:** SQL-style joins on key columns.

**Types of Joins:**

```python
df1 = pd.DataFrame({
    'ID': [1, 2, 3],
    'Name': ['Alice', 'Bob', 'Carol']
})

df2 = pd.DataFrame({
    'ID': [2, 3, 4],
    'Score': [90, 85, 95]
})

# Inner Join (default)
# Only matching keys
pd.merge(df1, df2, on='ID')
# Output:
#    ID   Name  Score
# 0   2    Bob     90
# 1   3  Carol     85

# Left Join
# All from left, matching from right
pd.merge(df1, df2, on='ID', how='left')
# Output:
#    ID   Name  Score
# 0   1  Alice    NaN
# 1   2    Bob   90.0
# 2   3  Carol   85.0

# Right Join
# All from right, matching from left
pd.merge(df1, df2, on='ID', how='right')
# Output:
#    ID   Name  Score
# 0   2    Bob     90
# 1   3  Carol     85
# 2   4    NaN     95

# Outer Join
# All from both
pd.merge(df1, df2, on='ID', how='outer')
# Output:
#    ID   Name  Score
# 0   1  Alice    NaN
# 1   2    Bob   90.0
# 2   3  Carol   85.0
# 3   4    NaN   95.0

# Different column names
df3 = pd.DataFrame({
    'EmpID': [2, 3],
    'Score': [90, 85]
})

pd.merge(df1, df3, left_on='ID', right_on='EmpID')
```

**Parameters:**
- `on`: Column name to join on
- `left_on`, `right_on`: Different column names
- `how`: 'inner', 'left', 'right', 'outer'
- `suffixes`: For duplicate column names

### 3. df.join()

**Purpose:** Join on **index** (default) or column.

**Examples:**

```python
df1 = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Carol']
}, index=[1, 2, 3])

df2 = pd.DataFrame({
    'Score': [90, 85, 95]
}, index=[2, 3, 4])

# Join on index (default)
df1.join(df2)
# Output:
#     Name  Score
# 1  Alice    NaN
# 2    Bob   90.0
# 3  Carol   85.0

# Left join (default)
df1.join(df2, how='left')

# Inner join
df1.join(df2, how='inner')
# Output: Only indices 2, 3

# Outer join
df1.join(df2, how='outer')
# Output: All indices 1, 2, 3, 4

# Add suffixes for duplicate columns
df1.join(df2, lsuffix='_left', rsuffix='_right')
```

**Comparison:**

```
merge()  - More flexible, SQL-like, join on columns
join()   - Simpler, index-based, shorthand for merge
concat() - Stacking, not relational joining
```

---

## 3.6 AGGREGATION AND GROUPING

### The GroupBy Pattern

**Split-Apply-Combine:**

```
1. SPLIT:   Group rows by key
2. APPLY:   Aggregate/Transform each group
3. COMBINE: Merge results back
```

### Basic GroupBy

```python
df = pd.DataFrame({
    'Dept': ['HR', 'IT', 'HR', 'IT', 'HR'],
    'Emp': ['A', 'B', 'C', 'D', 'E'],
    'Salary': [50, 80, 55, 90, 60],
    'Yrs': [2, 5, 3, 7, 4]
})

# Group by single column
df.groupby('Dept')

# Aggregate single column
df.groupby('Dept')['Salary'].mean()
# Output:
# Dept
# HR    55.0
# IT    85.0
# Name: Salary, dtype: float64

# Multiple aggregations
df.groupby('Dept')['Salary'].agg(['mean', 'max', 'sum'])
# Output:
#       mean  max  sum
# Dept                
# HR    55.0   60  165
# IT    85.0   90  170
```

### Multiple Aggregations

**Different functions per column:**

```python
df.groupby('Dept').agg({
    'Salary': ['mean', 'max', 'sum'],
    'Yrs': 'mean'
})
# Output:
#       Salary            Yrs
#         mean max sum  mean
# Dept                      
# HR      55.0  60 165   3.0
# IT      85.0  90 170   6.0
```

**Named aggregations (pandas >= 0.25):**

```python
df.groupby('Dept').agg(
    avg_sal=('Salary', 'mean'),
    max_sal=('Salary', ' 'max'),
    min_sal=('Salary', 'min'),
    total_sal=('Salary', 'sum'),
    headcount=('Emp', 'count'),
    avg_yrs=('Yrs', 'mean')
)
# Output:
#       avg_sal  max_sal  min_sal  total_sal  headcount  avg_yrs
# Dept                                                          
# HR       55.0       60       50        165          3      3.0
# IT       85.0       90       80        170          2      6.0
```

### GroupBy with Multiple Keys

```python
df2 = pd.DataFrame({
    'Region': ['North', 'North', 'South', 'South'],
    'Year': [2023, 2024, 2023, 2024],
    'Sales': [100, 120, 80, 90]
})

# Group by multiple columns
df2.groupby(['Region', 'Year'])['Sales'].sum()
# Output:
# Region  Year
# North   2023    100
#         2024    120
# South   2023     80
#         2024     90
# Name: Sales, dtype: int64
```

### Transform and Filter

**transform() - Return same shape:**

```python
# Add group mean to each row
df['Dept_Avg_Salary'] = df.groupby('Dept')['Salary'].transform('mean')
# Output:
#     Name  Salary  Dept_Avg_Salary
# 0  Alice      50             55.0
# 1    Bob      80             85.0
# ...

# Standardize within groups
df['Salary_Z'] = df.groupby('Dept')['Salary'].transform(
    lambda x: (x - x.mean()) / x.std()
)
```

**filter() - Keep/drop groups:**

```python
# Keep groups with more than 2 employees
df.groupby('Dept').filter(lambda x: len(x) > 2)

# Keep groups with average salary > 60
df.groupby('Dept').filter(lambda x: x['Salary'].mean() > 60)
```

### Iterating Over Groups

```python
for name, group in df.groupby('Dept'):
    print(f"Department: {name}")
    print(group)
    print()
# Output:
# Department: HR
#   Dept Emp  Salary  Yrs
# 0   HR   A      50    2
# 2   HR   C      55    3
# 4   HR   E      60    4
#
# Department: IT
#   Dept Emp  Salary  Yrs
# 1   IT   B      80    5
# 3   IT   D      90    7
```

---

## 3.7 PIVOT TABLES

### What are Pivot Tables?

**Definition:** Reshape and summarize data like Excel pivot tables.

**Two Main Functions:**
1. `pd.pivot_table()` - With aggregation
2. `df.pivot()` - Without aggregation

### pd.pivot_table()

**Basic Syntax:**
```python
pd.pivot_table(df, 
               values='column_to_summarize',
               index='row_grouping',
               columns='column_grouping',
               aggfunc='aggregation_function')
```

**Example:**

```python
df = pd.DataFrame({
    'Region': ['East', 'East', 'West', 'West', 'East'],
    'Product': ['A', 'B', 'A', 'B', 'A'],
    'Quarter': ['Q1', 'Q1', 'Q1', 'Q1', 'Q2'],
    'Sales': [100, 200, 150, 250, 120]
})

# Basic pivot table
pd.pivot_table(df,
               values='Sales',
               index='Region',
               columns='Product',
               aggfunc='sum')
# Output:
# Product    A    B
# Region           
# East     220  200
# West     150  250
```

**With Totals (Margins):**

```python
pd.pivot_table(df,
               values='Sales',
               index='Region',
               columns='Product',
               aggfunc='sum',
               fill_value=0,
               margins=True,
               margins_name='Total')
# Output:
# Product    A    B  Total
# Region                  
# East     220  200    420
# West     150  250    400
# Total    370  450    820
```

**Multiple Aggregations:**

```python
pd.pivot_table(df,
               values='Sales',
               index=['Region', 'Quarter'],
               columns='Product',
               aggfunc=['mean', 'sum'])
# Output: Multi-level columns
#        mean       sum      
# Product   A    B    A    B
# Region Quarter            
# East   Q1   100  200  100  200
#        Q2   120    0  120    0
# West   Q1   150  250  150  250
```

**Multiple Values:**

```python
pd.pivot_table(df,
               values=['Sales', 'Quantity'],
               index='Region',
               columns='Product',
               aggfunc='sum')
```

**Custom Aggregation:**

```python
pd.pivot_table(df,
               values='Sales',
               index='Region',
               aggfunc=lambda x: x.max() - x.min())
```

### df.pivot()

**Purpose:** Simple reshape **without aggregation**.

**Requirements:**
- Unique index-column combinations
- Raises error on duplicates

**Example:**

```python
df.pivot(index='Region',
         columns='Product',
         values='Sales')
# Output:
# Product    A      B
# Region             
# East     100  200.0
# West     150  250.0
```

**Error with duplicates:**

```python
# If East-A appears twice, this fails:
# ValueError: Index contains duplicate entries
# Use pivot_table instead!
```

### Pivot Table Parameters

```
values     - Column(s) to aggregate
index      - Row grouping
columns    - Column grouping
aggfunc    - Aggregation function(s)
           - 'mean', 'sum', 'count', 'min', 'max'
           - List: ['mean', 'sum']
           - Dict: {'Sales': 'sum', 'Qty': 'mean'}
fill_value - Replace NaN with value
margins    - Add row/column totals (True/False)
margins_name - Label for totals ('All', 'Total')
```

---

## 3.8 IMPORTING MATPLOTLIB

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

# Available styles
print(plt.style.available)
```

**Basic Plot Structure:**

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

**Figure and Axes:**

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

## 3.9 LINE PLOTS

### What is a Line Plot?

**Definition:** A line plot connects data points with straight lines.

**Best For:**
- Showing trends over time
- Continuous variables
- Time series data

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
'o'   - Circle
's'   - Square
'^'   - Triangle up
'v'   - Triangle down
'D'   - Diamond
'*'   - Star
'+'   - Plus
'x'   - X
```

### Multiple Lines

```python
x = np.linspace(0, 4*np.pi, 200)

plt.figure(figsize=(8, 4))

# Plot multiple lines
plt.plot(x, np.sin(x),
         color='blue',
         linestyle='-',
         linewidth=2,
         label='sin(x)')

plt.plot(x, np.cos(x),
         color='red',
         linestyle='--',
         linewidth=2,
         label='cos(x)')

plt.plot(x, np.sin(x)*np.exp(-x/10),
         color='green',
         linewidth=2,
         linestyle=':',
         label='damped sin')

# Add labels and legend
plt.title('Line Plot Example')
plt.xlabel('x')
plt.ylabel('y')
plt.legend()
plt.grid(True, alpha=0.4)
plt.tight_layout()
plt.show()
```

### Customizing Appearance

```python
# Set figure size
plt.figure(figsize=(10, 6))

# Plot with custom style
plt.plot(x, y,
         color='#2563EB',     # Hex color
         linestyle='-',
         linewidth=2.5,
         marker='o',
         markersize=6,
         markerfacecolor='red',
         markeredgecolor='black',
         markeredgewidth=1,
         alpha=0.8)           # Transparency

# Customize grid
plt.grid(True,
         linestyle='--',
         alpha=0.5)

# Tight layout
plt.tight_layout()
```

---

## 3.10 SCATTER PLOTS

### What is a Scatter Plot?

**Definition:** Shows correlation between two numerical variables.

**Characteristics:**
- Each point = one observation
- X-axis = Independent variable
- Y-axis = Dependent variable
- Reveals relationships, clusters, outliers

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
               alpha=0.75,
               s=50,
               color=col,
               label=grp,
               edgecolors='white',
               lw=0.5)

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
            c=colors,
            s=sizes,
            alpha=0.5,
            cmap='viridis')

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

## 3.11 VISUALIZING ERRORS

### Why Show Errors?

**Purpose:** Display uncertainty in measurements or predictions.

**Common Uses:**
- Experimental error bars
- Confidence intervals
- Standard deviation
- Standard error

### plt.errorbar()

**Basic Usage:**

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

### fill_between()

**Purpose:** Shade region between two y-curves.

**Perfect for:**
- Confidence intervals
- Prediction bands
- Uncertainty regions

**Example:**

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

### Multiple Bands

```python
x = np.linspace(0, 10, 100)
y = np.exp(-x/10) * np.sin(x)

plt.plot(x, y, 'k-', linewidth=2)

# 68% confidence
plt.fill_between(x, y-0.1, y+0.1,
                 alpha=0.3, color='blue',
                 label='68% CI')

# 95% confidence
plt.fill_between(x, y-0.2, y+0.2,
                 alpha=0.2, color='blue',
                 label='95% CI')

plt.legend()
plt.show()
```

---

## 3.12 DENSITY AND CONTOUR PLOTS

### Kernel Density Estimation (KDE)

**Definition:** Smoothed probability density estimate.

**Purpose:**
- Show distribution shape
- Better than histogram for continuous data
- No binning artifacts

**Example:**

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
plt.hist(data,
         bins=25,
         density=True,
         alpha=0.4,
         label='Histogram')

plt.plot(x, kde(x),
         lw=2.5,
         label='KDE')

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

**Types:**
- `contour()` - Line-only contours
- `contourf()` - Filled contours

**Example:**

```python
# Create grid
xx = yy = np.linspace(-3, 3, 80)
X, Y = np.meshgrid(xx, yy)
Z = np.exp(-(X**2 + Y**2)/2)

# Line contour
plt.contour(X, Y, Z, levels=14)
plt.title('Contour Plot')
plt.show()

# Filled contour
plt.contourf(X, Y, Z,
             levels=14,
             cmap='viridis')
plt.colorbar()
plt.title('Filled Contour')
plt.show()
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

### 2D Density Plot

```python
# Generate correlated data
x = np.random.randn(1000)
y = x * 0.5 + np.random.randn(1000) * 0.5

# Create 2D histogram
plt.hist2d(x, y,
           bins=30,
           cmap='Blues')
plt.colorbar()
plt.title('2D Density')
plt.show()
```

---

## 3.13 HISTOGRAMS

### What is a Histogram?

**Definition:** Shows frequency distribution of a single variable.

**Characteristics:**
- Contiguous (touching) bars
- X-axis = Value ranges (bins)
- Y-axis = Frequency or density

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
         bins=20,
         alpha=0.65,
         color='blue',
         label='Class A',
         edgecolor='white')

plt.hist(scores_B,
         bins=20,
         alpha=0.65,
         color='red',
         label='Class B',
         edgecolor='white')

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

plt.hist2d(x, y,
           bins=30,
           cmap='Blues')

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

plt.hist(data,
         bins=bins,
         edgecolor='black')

plt.xticks(bins)
plt.show()
```

### Normalized Histogram

```python
plt.hist(data,
         bins=20,
         density=True,    # Area = 1
         alpha=0.6)

# Overlay normal distribution
from scipy.stats import norm
x = np.linspace(min(data), max(data), 100)
plt.plot(x, norm.pdf(x, np.mean(data), np.std(data)),
         'r-', linewidth=2)
```

---

## 3.14 LEGENDS

### What are Legends?

**Purpose:** Identify different elements in a plot.

### Basic Legend

```python
plt.plot(x, y1, label='Line 1')
plt.plot(x, y2, label='Line 2')
plt.legend()
plt.show()
```

### Legend Parameters

```python
plt.legend(loc='best',        # Location
           fontsize=12,       # Font size
           framealpha=0.9,    # Frame transparency
           fancybox=True,     # Rounded corners
           shadow=True,       # Shadow
           title='Legend',    # Title
           ncol=2,           # Number of columns
           frameon=True)     # Show frame
```

### Location Options

```
'best'          - 0 (automatic)
'upper right'   - 1
'upper left'    - 2
'lower left'    - 3
'lower right'   - 4
'right'         - 5
'center left'   - 6
'center right'  - 7
'lower center'  - 8
'upper center'  - 9
'center'        - 10
```

### Custom Legend

```python
import matplotlib.patches as mpatches

# Create custom patches
patch1 = mpatches.Patch(color='blue', label='Category A')
patch2 = mpatches.Patch(color='red', label='Category B')
patch3 = mpatches.Patch(color='green', label='Category C')

plt.legend(handles=[patch1, patch2, patch3],
           loc='upper right',
           fancybox=True,
           shadow=True)
```

### Legend Outside Plot

```python
plt.plot(x, y, label='Data')

# Place legend outside
plt.legend(bbox_to_anchor=(1.05, 1),
           loc='upper left',
           borderaxespad=0)

plt.tight_layout()
plt.show()
```

### Multiple Legends

```python
line1, = plt.plot(x, y1, 'b-', label='Line 1')
line2, = plt.plot(x, y2, 'r-', label='Line 2')

# First legend
leg1 = plt.legend([line1, line2],
                  ['Line 1', 'Line 2'],
                  loc='upper left')

# Add second legend
plt.gca().add_artist(leg1)

plt.legend([line1], ['Special'], loc='lower right')
```

---

## 3.15 COLORS

### Color Specifications

**Named Colors:**

```python
plt.plot(x, y, color='red')
plt.plot(x, y, color='blue')
plt.plot(x, y, color='green')
plt.plot(x, y, color='orange')
plt.plot(x, y, color='purple')
```

**Common Color Names:**
```
'red', 'blue', 'green', 'yellow', 'orange', 'purple'
'pink', 'brown', 'black', 'white', 'gray', 'cyan'
'magenta', 'lime', 'navy', 'maroon', 'olive', 'teal'
```

**Hex Colors:**

```python
plt.plot(x, y, color='#2563EB')   # Blue
plt.plot(x, y, color='#DC2626')   # Red
plt.plot(x, y, color='#059669')   # Green
```

**RGB/RGBA:**

```python
# RGB (0-1)
plt.plot(x, y, color=(0.3, 0.6, 0.9))

# RGBA (with alpha)
plt.plot(x, y, color=(0.3, 0.6, 0.9, 0.7))
```

### Colormaps

**Sequential (light to dark):**

```python
'viridis'    - Default, perceptually uniform
'plasma'     - Purple to yellow
'inferno'    - Black to yellow
'magma'      - Black to pink
'Blues'      - White to blue
'Greens'     - White to green
'Reds'       - White to red
```

**Diverging (two colors):**

```python
'coolwarm'   - Blue to red
'Seismic'    - Blue to red (earthquake)
'RdBu'       - Red to blue
'PiYG'       - Pink to green
```

**Qualitative (distinct):**

```python
'Set1'       - 9 distinct colors
'Set2'       - 8 distinct colors
'Set3'       - 12 distinct colors
'tab10'      - 10 colors
'tab20'      - 20 colors
```

### Using Colormaps

```python
# Scatter plot with colormap
plt.scatter(x, y,
            c=values,
            cmap='viridis')

plt.colorbar(label='Value')

# Heatmap
plt.imshow(data,
           cmap='plasma',
           aspect='auto')

plt.colorbar()
```

### Custom Color Cycle

```python
# Set custom colors for all plots
plt.rcParams['axes.prop_cycle'] = plt.cycler(
    color=['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728']
)
```

---

## 3.16 SUBPLOTS

### What are Subplots?

**Purpose:** Multiple plots in one figure.

### Basic Subplots

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

### Parameters

```python
plt.subplots(nrows=2,
             ncols=2,
             figsize=(10, 6),
             sharex=True,      # Share x-axis
             sharey=True,      # Share y-axis
             squeeze=False)    # Keep 2D array
```

### Sharing Axes

```python
# Share x-axis
fig, axes = plt.subplots(2, 1, sharex=True)

axes[0].plot(x, y1)
axes[1].plot(x, y2)
# Both have same x-range
```

### GridSpec - Flexible Layouts

```python
from matplotlib.gridspec import GridSpec

fig = plt.figure(figsize=(10, 6))

# Create gridspec
gs = GridSpec(2, 3, figure=fig,
              hspace=0.4,
              wspace=0.3)

# Add subplots with different sizes
ax1 = fig.add_subplot(gs[0, :2])  # Wide plot
ax2 = fig.add_subplot(gs[0, 2])   # Narrow
ax3 = fig.add_subplot(gs[1, :])   # Full width

ax1.plot(x, y)
ax2.scatter(x, y)
ax3.hist(data)

plt.show()
```

### Complex Layout

```python
fig = plt.figure(figsize=(12, 8))
gs = fig.add_gridspec(3, 3, hspace=0.3, wspace=0.3)

# Large plot on left
ax_main = fig.add_subplot(gs[:, 0:2])

# Small plots on right
ax_top = fig.add_subplot(gs[0, 2])
ax_mid = fig.add_subplot(gs[1, 2])
ax_bot = fig.add_subplot(gs[2, 2])

ax_main.plot(x, y)
ax_top.hist(data1)
ax_mid.hist(data2)
ax_bot.scatter(x, y)
```

---

## 3.17 TEXT AND ANNOTATION

### Adding Text

**ax.text() - Place text at coordinates:**

```python
fig, ax = plt.subplots()
ax.plot(x, y)

# Add text
ax.text(0.2, -0.9,
        'sin(x) function',
        fontsize=9,
        style='italic',
        bbox=dict(boxstyle='round',
                  facecolor='lightyellow'))

plt.show()
```

### Parameters

```python
ax.text(x, y,
        'Text content',
        fontsize=12,
        fontweight='bold',
        color='red',
        ha='center',      # Horizontal alignment
        va='center',      # Vertical alignment
        rotation=45,      # Rotation degrees
        bbox=dict(        # Text box
            boxstyle='round',
            facecolor='wheat',
            alpha=0.5))
```

### ax.annotate() - Text with Arrow

```python
fig, ax = plt.subplots()
ax.plot(x, np.sin(x))

# Find maximum
idx = np.argmax(np.sin(x))

# Annotate
ax.annotate('Maximum',
            xy=(x[idx], np.sin(x[idx])),    # Point to annotate
            xytext=(x[idx]+0.8, 0.6),       # Text position
            arrowprops=dict(                # Arrow style
                facecolor='black',
                shrink=0.05,
                width=2,
                headwidth=8))

plt.show()
```

### Arrow Styles

```python
arrowprops=dict(
    arrowstyle='->',        # Arrow type
    connectionstyle='arc3', # Connection style
    color='red',
    lw=2)
```

**Arrow Styles:**
```
'-'   - Simple line
'->'  - Simple arrow
'-['  - Bracket
'-|>' - Filled arrow
'fancy' - Fancy arrow
```

### Multiple Annotations

```python
fig, ax = plt.subplots()
ax.plot(x, y)

# Add multiple annotations
annotations = [
    (x[10], y[10], 'Point A'),
    (x[50], y[50], 'Point B'),
    (x[90], y[90], 'Point C')
]

for x_val, y_val, label in annotations:
    ax.annotate(label,
                xy=(x_val, y_val),
                xytext=(x_val+0.5, y_val+0.1),
                arrowprops=dict(arrowstyle='->'))
```

---

## 3.18 CUSTOMIZATION

### plt.style

**Predefined Styles:**

```python
plt.style.use('seaborn-v0_8')
plt.style.use('ggplot')
plt.style.use('fivethirtyeight')
plt.style.use('dark_background')
plt.style.use('classic')

# View available styles
print(plt.style.available)
```

### rcParams - Global Settings

```python
import matplotlib as mpl

# Set global parameters
plt.rcParams['font.size'] = 14
plt.rcParams['axes.facecolor'] = 'white'
plt.rcParams['figure.figsize'] = (10, 6)
plt.rcParams['lines.linewidth'] = 2
plt.rcParams['axes.grid'] = True
plt.rcParams['legend.fontsize'] = 12

# Save settings
mpl.rcParams.update(mpl.rcParamsDefault)  # Reset
```

### Spines Customization

```python
fig, ax = plt.subplots()
ax.plot(x, y)

# Remove top and right spines
ax.spines['top'].set_visible(False)
ax.spines['right'].set_visible(False)

# Move bottom and left to center
ax.spines['bottom'].set_position('zero')
ax.spines['left'].set_position('zero')

# Change color
ax.spines['left'].set_color('gray')
ax.spines['bottom'].set_color('gray')
```

### Ticks Customization

```python
# Set tick locations
plt.xticks([0, 2, 4, 6, 8, 10])
plt.yticks([-1, -0.5, 0, 0.5, 1])

# Set tick labels
plt.xticks([0, 1, 2], ['A', 'B', 'C'])

# Customize appearance
ax.tick_params(labelsize=12,
               length=6,
               width=2,
               color='red',
               labelcolor='blue')

# Rotate labels
plt.xticks(rotation=45, ha='right')
```

### Figure Customization

```python
fig, ax = plt.subplots()

# Set figure properties
fig.patch.set_facecolor('lightgray')
fig.patch.set_alpha(0.5)

# Set axes properties
ax.set_facecolor('white')
ax.set_xlim(0, 10)
ax.set_ylim(-1, 1)
ax.set_aspect('equal')  # Equal scaling
```

---

## 3.19 THREE-DIMENSIONAL PLOTTING

### Introduction to 3D Plots

**Module:**

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

### 3D Wireframe

```python
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

ax.plot_wireframe(X, Y, Z,
                  rstride=2,
                  cstride=2,
                  color='blue',
                  linewidth=0.5)

plt.show()
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
           c=colors,
           cmap='viridis',
           marker='o',
           s=50,
           alpha=0.6)

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

### Multiple 3D Plots

```python
fig = plt.figure(figsize=(12, 4))

# Plot 1
ax1 = fig.add_subplot(131, projection='3d')
ax1.plot_surface(X, Y, Z, cmap='viridis')

# Plot 2
ax2 = fig.add_subplot(132, projection='3d')
ax2.plot_wireframe(X, Y, Z, color='red')

# Plot 3
ax3 = fig.add_subplot(133, projection='3d')
ax3.scatter(xs, ys, zs, c=zs, cmap='plasma')

plt.tight_layout()
```

---

## 3.20 GEOGRAPHIC DATA WITH BASEMAP

### Introduction to Basemap

**Note:** Basemap is deprecated. Use Cartopy for new projects.

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
            llcrnrlat=-60,
            urcrnrlat=80,
            llcrnrlon=-180,
            urcrnrlon=180)

# Draw features
m.drawcoastlines(linewidth=0.8)
m.drawcountries(linewidth=0.5)
m.fillcontinents(color='lightgreen',
                 lake_color='lightblue')
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

### Filled Continents

```python
m.fillcontinents(color='coral',
                 lake_color='aqua',
                 resolution='h')  # 'c', 'l', 'i', 'h', 'f'
```

---

## 3.21 VISUALIZATION WITH SEABORN

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

### Violin Plot

**Purpose:** Shows full distribution shape (combines box plot + KDE).

```python
# Load dataset
tips = sns.load_dataset('tips')

# Basic violin plot
sns.violinplot(data=tips,
               x='day',
               y='total_bill',
               palette='Set2')

plt.title('Total Bill by Day')
plt.show()
```

### Box Plot

**Purpose:** Shows IQR, median, outliers.

```python
# Basic box plot
sns.boxplot(data=tips,
            x='smoker',
            y='total_bill',
            hue='time',
            palette='coolwarm')

plt.title('Bill by Smoker and Time')
plt.show()
```

### Regplot (Regression Plot)

**Purpose:** Scatter plot + regression line.

```python
sns.regplot(data=tips,
            x='total_bill',
            y='tip',
            ci=95,           # Confidence interval
            scatter_kws={'alpha': 0.5},
            line_kws={'color': 'red'})

plt.title('Tip vs Total Bill')
plt.show()
```

### Heatmap

**Purpose:** Great for correlation matrices.

```python
# Calculate correlation
corr = tips[['total_bill', 'tip', 'size']].corr()

# Create heatmap
sns.heatmap(corr,
            annot=True,      # Show values
            cmap='Blues',
            fmt='.2f',       # Decimal places
            linewidths=0.5,
            square=True)

plt.title('Correlation Matrix')
plt.show()
```

### Count Plot

**Purpose:** Bar chart for categorical data.

```python
sns.countplot(data=tips,
              x='day',
              hue='sex',
              palette='pastel')

plt.title('Count by Day and Sex')
plt.show()
```

### Pairplot

**Purpose:** Scatter matrix - all pairwise relationships.

```python
# Basic pairplot
sns.pairplot(tips)
plt.show()

# With hue
sns.pairplot(tips,
             hue='sex',
             palette='viridis',
             markers=['o', 's'])

plt.show()

# Specific variables
sns.pairplot(tips,
             vars=['total_bill', 'tip', 'size'],
             hue='smoker')
```

### Distribution Plot

```python
# Histogram + KDE
sns.histplot(data=tips,
             x='total_bill',
             kde=True,
             bins=20)

plt.show()

# Multiple distributions
sns.histplot(data=tips,
             x='total_bill',
             hue='time',
             kde=True,
             element='step')
```

### Styling

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

## PANDAS

**Indexing:**
```
df.loc[r,c]      - Label based
df.iloc[r,c]     - Position based
df[mask]         - Boolean filtering
df.at/i          - Fast scalar access
```

**Operations:**
```
df * scalar      - Vectorized ops
.apply(fn)       - Apply function
.map()           - Element-wise Series
.applymap()      - Element-wise DataFrame
np.ufunc(df)     - NumPy functions
```

**Missing Data:**
```
.isnull()        - Boolean mask
.dropna()        - Remove NaN
.fillna()        - Fill NaN
.interpolate()   - Interpolate
```

**MultiIndex:**
```
pd.MultiIndex.from_tuples()
.xs()            - Cross-section
.stack()         - Column to row
.unstack()       - Row to column
```

**Combining:**
```
pd.concat()      - Stack DataFrames
pd.merge(how=...) - SQL joins
df.join()        - Index join
```

**Grouping:**
```
.groupby(key).agg({})
.transform()
.filter()
```

**Pivot:**
```
pd.pivot_table(values, index, columns, aggfunc)
margins=True     - Add totals
```

## NUMPY

**Arrays:**
```
np.array()       - Create array
np.zeros()       - Zeros array
np.ones()        - Ones array
np.arange()      - Range array
np.linspace()    - Evenly spaced
np.random.rand() - Random array
```

**Aggregations:**
```
np.sum()         - Sum
np.mean()        - Mean
np.std()         - Standard deviation
np.min/max()     - Min/Max
np.median()      - Median
```

**Operations:**
```
a + b            - Element-wise add
a * b            - Element-wise multiply
np.sqrt(a)       - Square root
np.exp(a)        - Exponential
```

**Indexing:**
```
a[a > 5]         - Boolean mask
a[[1,3,5]]       - Fancy indexing
a[rows, cols]    - 2D indexing
```

## MATPLOTLIB

**Basic Plots:**
```
plt.plot()       - Line plot
plt.scatter()    - Scatter plot
plt.hist()       - Histogram
plt.bar()        - Bar chart
plt.errorbar()   - Error bars
```

**Customization:**
```
plt.figure(figsize=(w,h))
plt.xlabel/ylabel/title()
plt.legend(loc=...)
plt.grid(True)
plt.style.use('style')
```

**Subplots:**
```
plt.subplots(r,c)
fig.add_subplot()
GridSpec()
```

**3D:**
```
from mpl_toolkits.mplot3d import Axes3D
ax.plot_surface(X,Y,Z)
ax.scatter(xs,ys,zs)
```

## SEABORN

**Statistical Plots:**
```
sns.violinplot()
sns.boxplot()
sns.regplot()
sns.heatmap()
sns.pairplot()
sns.countplot()
sns.histplot()
```

**Styling:**
```
sns.set_style()
sns.set_context()
sns.set_palette()
```

---

## 📖 FORMULAS QUICK REFERENCE

### Statistics

**Mean:**
```
      Σx
μ = -----
       n
```

**Variance:**
```
       Σ(x - μ)²
σ² = -----------
          n
```

**Standard Deviation:**
```
σ = √σ²
```

**Z-Score:**
```
      X - μ
Z = --------
       σ
```

**Correlation:**
```
        n(Σxy) - (Σx)(Σy)
r = ----------------------------
    √[nΣx² - (Σx)²][nΣy² - (Σy)²]
```

**Regression:**
```
Ŷ = a + bX

        n(ΣXY) - (ΣX)(ΣY)
b = -----------------------
        nΣX² - (ΣX)²

a = ȳ - b(x̄)
```

**Coefficient of Determination:**
```
R² = r²
```

**Standard Error:**
```
         Σ(Y - Ŷ)²
SEE = √-----------
           n - 2
```

---


---

*This comprehensive guide covers all concepts from your course materials with detailed explanations, step-by-step examples, and practical code. Master these topics and you're on your way to scoring 100/100!*
