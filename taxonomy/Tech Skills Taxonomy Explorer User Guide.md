# Tech Skills Taxonomy Explorer User Guide

## Overview

The Tech Skills Taxonomy Explorer is an interactive tool that helps you explore and analyze technology skills data. The visualization displays skills as points on a map, where similar skills are positioned closer together. This guide explains the key metrics, features, and information available in the visualization, enabling you to gain actionable insights from complex job market and skill datasets.

---

## Interface Elements

### Main Visualization

- **Points:** Each point represents a specific skill or technology.

- **Clusters:** Groups of related skills are shown in proximity.

- **Colors:** Different colors indicate different categories of skills.

- **Point Size:** Larger points indicate higher average salary ranges, providing a visual cue for compensation levels.

### Interactive Features

- **Zoom:** Use the mouse wheel or pinch gestures to zoom in and out.

- **Pan:** Click and drag to move around the visualization.

- **Selection:**

   - **Left-click** individual points to select them.

   - **Right-click** to select all points within a cluster.

   - **Shift-click-drag** to select multiple points at once via the **lasso tool**.

- **Search:** Utilize the search box to quickly find specific skills or technologies.

---

## Understanding the Data

### Hover Information

When you hover over a point, a tooltip appears with detailed information. The displayed data includes:

#### Salary Information

- **Est. Salary Range:** Shows the minimum, median, and maximum salary range.

- **Cluster Salary Statistics:**

   - **Median and Mean Salary:** Indicates the typical compensation within the cluster.

   - **Salary Rank:** For example, "Rank 5 of 150" shows how the cluster compares to others.

   - **Salary Percentile:** For example, "95.2 percentile" indicates the relative salary standing.

#### Temporal Metrics

- **Growth Rate:** A value between -1.0 and 1.0 that indicates the skill's demand trend.  

   - *Positive values* signal increasing demand.  

   - *Negative values* indicate decreasing demand.

- **Temporal Pattern:** Classifies the skill based on its activity over time:

   - **New:** Recently emerged skills.

   - **Trending:** Skills showing significant growth.

   - **Concentrated:** Skills with high demand during specific periods.

   - **Seasonal:** Skills with recurring demand patterns.

   - **Stable:** Skills with consistent demand.

- **Age Metrics (measured in quarters):**

   - **Average Age:** Mean duration that the skill has been present.

   - **Median Age:** The middle value in the age distribution.

   - **Newest Entry:** The most recent appearance of the skill.

#### Volume and Distribution

- **Sample Size:** The number of job postings mentioning the skill.

- **Size Classification:**

   - **Small:** Fewer than 50 mentions.

   - **Medium:** Between 50 and 200 mentions.

   - **Large:** More than 200 mentions.

- **Monthly Distribution:** Shows posting frequency by month, helping to reveal seasonal or periodic trends.

---

## Color Schemes

The visualization offers multiple color schemes to highlight different aspects of the data:

- **Posting Month:** Colors reflect the time when skills were posted.

- **Salary Range:** A gradient that shows salary distributions.

- **Job Specialization:** Distinct colors for various job specialties.

- **Salary Distribution:** A log-scaled visualization of salary data.

- **Age-Based Views:** Options to display:

   - Individual skill age.

   - Cluster average age.

   - Newest entries in the cluster.

- **Additional Layers:** Such as anomaly values, trends, and salary rank percentiles to further emphasize unique data patterns.

---

## Analyzing the Data

### Cluster Analysis

Clusters are formed based on several factors:

- **Semantic Similarity:** Grouping skills that are conceptually related.

- **Co-occurrence in Job Postings:** Skills that frequently appear together.

- **Related Technology Stacks:** Similar technical ecosystems.

- **Similar Salary Ranges:** Clustering by compensation metrics.

### Temporal Analysis

The visualization helps you identify:

- **Emerging Technologies:** Skills that are rapidly gaining traction.

- **Declining Skills:** Technologies that are losing prominence.

- **Seasonal Patterns:** Variations in demand over different months.

- **Industry Shifts:** Broad trends in technology adoption and job market evolution.

### Salary Analysis

Salary data is normalized and analyzed to reveal:

- **Market Value of Skills:** Understand compensation trends across clusters.

- **Salary Trends Within Clusters:** Compare median and mean salaries.

- **Compensation Patterns:** Insights across different job specializations.

- **Regional Variations:** Where available, highlighting geographic differences in salary.

---

## Tips for Effective Use

### Exploration

- **Start with the Default View:** Begin by exploring the default category to gain an overall understanding.

- **Switch Color Schemes:** Experiment with different color schemes to focus on specific aspects, such as posting month or salary distribution.

- **Zoom and Pan:** Use zoom and pan features to navigate dense clusters and investigate individual points.

- **Search:** Use the search functionality to quickly locate specific skills or technologies.

### Analysis

- **Compare Related Clusters:** Look for similarities and differences in salary and temporal metrics.

- **Examine Temporal Patterns:** Identify emerging trends or seasonal fluctuations.

- **Review Salary Distributions:** Benchmark market values and compare across clusters.

- **Consider Skill Relationships:** Analyze how different skills relate to one another based on their cluster grouping.

### Selection

- **Multi-Select Options:** Use multi-select (via lasso tool or right-click) for comparing groups of skills.

- **Right-Click for Cluster Selection:** Quickly select all points in a cluster for a comprehensive analysis.

- **Custom Selections:** Tailor your analysis by creating custom selections to focus on subsets of data.

---

## Data Quality Notes

- **Outlier Detection:** Outliers are automatically detected and filtered to ensure reliable metrics.

- **Missing Data Imputation:** Missing salary values are imputed using cluster medians.

- **Growth Rate Calculation:** Growth rates are calculated using a 90-day window.

- **Temporal Pattern Reliability:** Temporal metrics require a minimum sample size for accuracy.

---

## Additional Features

### Search and Filtering

- **Full-Text Search:** Quickly search across all skills.

- **Category Filtering:** Filter results by categories, subcategories, or clusters.

- **Date Range Filtering:** Focus on data from specific time periods.

- **Salary Range Filtering:** Narrow down results based on compensation levels.

---

## High-Level Methodology

### Dimensionality Reduction and Clustering

The tool uses advanced techniques to reduce high-dimensional data (such as skill descriptions and job titles) into a two-dimensional map while preserving relationships between data points. Similar skills are positioned closer together, and clustering algorithms then group these points based on semantic similarity, co-occurrence in job postings, technology stack relationships, and similar salary ranges.

### Salary and Temporal Analysis

- **Salary Metrics:** The system computes median and mean salary values for each cluster, using outlier detection to filter anomalous data.

- **Temporal Metrics:** Growth rates, age metrics (average, median, newest entry), and monthly distributions are calculated to highlight trends and seasonal variations.

### Taxonomy Data Integration

Data is loaded from a curated taxonomy where infrequent or overly generic skills are filtered out based on preset frequency thresholds. This ensures that the visualization focuses on high-quality, relevant data.

---

## Interactive Features

### Hover Tooltips

Hovering over a point reveals a tooltip that displays:

- **Salary Information:** Including salary ranges, median/mean salary, salary rank, and percentile.

- **Temporal Metrics:** Such as growth rate, temporal pattern, and age metrics.

- **Volume Metrics:** Like sample size and monthly distribution.

### Selection and Filtering

Interactive selection tools allow you to:

- **Click or Lasso-Select:** Pick individual or groups of points.

- **Right-Click:** Select an entire cluster.

- **Dynamic Filtering:** Refine your selection to focus on subsets of data.

### Search Functionality

A built-in search feature makes it easy to locate specific skills or clusters, streamlining the exploration process.

---

## How to Interpret the Data

- **Growth Rate:** Indicates the momentum of a skill’s demand; high positive values suggest rapid growth, while negative values imply decline.

- **Cluster Ages:** Help differentiate between established skills and emerging trends by showing average, median, and newest entry ages.

- **Anomaly Score & Trending Status:** Identify clusters that deviate from typical patterns or are experiencing significant changes.

- **Salary Metrics:** Enable benchmarking of median and mean salaries across clusters.

- **Volume and Distribution:** Provide context on sample size and seasonal posting patterns, which help assess data reliability.

---

## Practical Applications

- **Identifying Emerging Trends:** Spot rapidly growing or declining technologies using growth rate and temporal metrics.

- **Benchmarking Salaries:** Compare salary data across clusters to understand market value.

- **Market Analysis:** Use clustering and temporal data to gauge industry shifts and technology adoption.

- **Strategic Planning:** Inform decisions in talent management, recruitment, and skill development based on comprehensive data insights.

---

## How to Use the Visualization

1. **Exploration:**

   - Hover over points to view detailed metrics.

   - Use zoom and pan to navigate the map.

   - Use the search box to quickly locate specific skills.

2. **Interaction:**

   - **Left-click** to select individual points.

   - **Right-click** to select all points within a cluster.

   - Use the **lasso tool** for custom multi-point selections.

3. **Analysis:**

   - Compare clusters based on salary and temporal metrics.

   - Examine growth rates and age metrics to identify emerging trends.

   - Review monthly distributions to understand seasonal variations.

---

This comprehensive guide integrates advanced data processing methodologies with an intuitive, interactive interface. Whether you are exploring market trends, benchmarking salaries, or planning strategic initiatives, the Tech Skills Taxonomy Explorer provides the insights you need to make informed decisions.


