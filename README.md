# AI & ML Internship Task 7

## Title
Exploratory Data Analysis (EDA)

---

## Objective

The objective of this task is to perform Exploratory Data Analysis (EDA) on the Automobile Dataset and discover meaningful patterns, trends, relationships, and insights using statistical analysis and visualizations.

This task focuses on:
- Univariate Analysis
- Bivariate Analysis
- Multivariate Analysis
- Correlation Analysis
- Outlier Detection
- Data Visualization
- Insight Generation

---

## Tools & Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- GitHub

---

## Dataset Used

### Automobile Dataset

The dataset contains information related to different automobile models including:

- Company
- Price
- Horsepower
- Engine Size
- Fuel Type
- Length
- Width
- Height
- Wheel Base
- Mileage

Dataset File:

```text
Automobile_data.csv
```

---

## Libraries Used

### Pandas
Used for:
- Loading data
- Data analysis
- Data exploration

### NumPy
Used for numerical calculations.

### Matplotlib
Used for:
- Histograms
- Visual analysis

### Seaborn
Used for:
- Boxplots
- Heatmaps
- Pairplots
- Scatterplots
- Barplots

---

## Tasks Performed

### 1. Loaded Dataset

Loaded the Automobile Dataset using Pandas.

```python
df = pd.read_csv('Automobile_data.csv')
```

---

### 2. Explored Dataset Structure

Used:

```python
df.head()
df.info()
df.shape
df.describe()
```

to understand:

- Number of rows
- Number of columns
- Data types
- Statistical summary

---

### 3. Checked Missing Values

Used:

```python
df.isnull().sum()
```

to identify missing values.

---

## Univariate Analysis

### Histogram

Used Histogram to analyze the distribution of automobile prices.

```python
plt.hist(df['price'])
```

Purpose:
- Understand data distribution
- Detect skewness
- Identify concentration of values

---

### Boxplot

Used Boxplot to identify outliers in automobile prices.

```python
sns.boxplot(x=df['price'])
```

Purpose:
- Detect extreme values
- Understand spread of data

---

## Bivariate Analysis

### Horsepower vs Price

Used Scatterplot to study the relationship between:

- Horsepower
- Price

```python
sns.scatterplot(
    x='horsepower',
    y='price'
)
```

Purpose:
- Understand feature relationships
- Identify trends

---

### Company vs Price

Used Barplot to compare automobile prices across companies.

```python
sns.barplot(
    x='company',
    y='price'
)
```

Purpose:
- Compare average prices
- Identify premium automobile brands

---

## Correlation Analysis

Generated Correlation Matrix using:

```python
df.corr()
```

Purpose:
- Measure relationships among numerical features

Correlation Values:

```text
+1  = Strong Positive Correlation
 0  = No Correlation
-1  = Strong Negative Correlation
```

---

## Heatmap Visualization

Used Heatmap to visualize correlations.

```python
sns.heatmap()
```

Purpose:
- Easily identify strongly related variables
- Understand feature dependencies

---

## Multivariate Analysis

Used Scatterplot with additional grouping variable.

Analyzed:

- Horsepower
- Price
- Fuel Type

```python
sns.scatterplot(
    x='horsepower',
    y='price',
    hue='fuel-type'
)
```

Purpose:
- Analyze relationships among multiple variables simultaneously

---

## Pairplot Analysis

Used:

```python
sns.pairplot()
```

Purpose:
- Observe relationships among numerical variables
- Detect trends and clusters
- Compare multiple features simultaneously

---

## Visualizations Used

- Histogram
- Boxplot
- Scatterplot
- Barplot
- Correlation Heatmap
- Pairplot

---

## Top 5 Insights

### Insight 1
Higher horsepower vehicles generally have higher prices.

### Insight 2
Some vehicles are significantly more expensive than others and appear as outliers.

### Insight 3
Certain automobile companies consistently manufacture premium-priced vehicles.

### Insight 4
Engine-related features show a positive relationship with vehicle price.

### Insight 5
Fuel type influences both vehicle performance and pricing.

---

## Concepts Learned

### Exploratory Data Analysis (EDA)
Process of understanding and analyzing data before building machine learning models.

### Univariate Analysis
Analysis of a single variable.

Example:
- Histogram
- Boxplot

### Bivariate Analysis
Analysis of relationships between two variables.

Example:
- Scatterplot

### Multivariate Analysis
Analysis involving three or more variables.

Example:
- Scatterplot with hue parameter

### Correlation
Measures strength and direction of relationship between variables.

### Outlier Detection
Identifying unusual observations that differ significantly from the majority of data.

---

## Outcome

Successfully performed Exploratory Data Analysis on the Automobile Dataset.

The analysis helped identify:
- Patterns
- Relationships
- Outliers
- Trends
- Feature correlations

The generated visualizations provided meaningful business and analytical insights from the dataset.

---

## Files Included

```text
Automobile_EDA.ipynb
Automobile_data.csv
README.md
```

---

## Repository Name

```text
AI-ML-Internship-Task-7
```

---

## Author

**Arya Chighare**  
Artificial Intelligence & Data Science  
YCCE, Nagpur
