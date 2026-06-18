# hotel-booking-demand-analytics
A data analytics project focused on preprocessing, exploratory analysis (EDA), and statistical hypothesis testing for hotel booking patterns and operational optimization.



# Comprehensive Hospitality Analytics & Hotel Booking Optimization

This repository contains the complete end-to-end data pipeline, data cleaning, advanced exploratory data analysis (EDA), and dual statistical hypothesis testing for optimizing hotel operations. I have independently built the entire code infrastructure to analyze booking patterns, mitigate cancellation risks, and forecast seasonal hospitality demand.

---

## 🚀 Data Pipeline & Project Workflow

The repository is executed sequentially across the following structural phases:

### 📥 Phase 1: Data Importation & Metadata Inspection
* **Cell 1:** Initial configuration where we import all required statistical and visualization libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`, and `scipy.stats`) and load the core file data.

### 🧹 Phase 2: Comprehensive Data Cleaning & Initial Auditing
* **By Cell 3:** Automated handling and tracking of missing fields across segments (such as missing operational location identities, agent indexes, and company classifications) to prepare the data for baseline exploratory testing.

### 📉 Phase 3: Outlier Profiling & Data Preprocessing
* Execution of **multiple Box Plots** to explicitly track down statistical anomalies and extreme variance behaviors. Outliers across variables like pricing metrics and reservation horizons are strategically isolated and handled to secure robust analytical outputs.

---

## 🏨 The 4 Core Business Scopes

The structural foundation of this project resolves the primary business pillars of the project documentation:
1. **Seasonal Trends:** Spotting reservation changes across month cycles to guide staff scheduling.
2. **Occupancy Rates:** Isolating actual realized check-ins to evaluate accurate property capacity utilization.
3. **Cancellation Behavior:** Matrix checking of payment rules and deposit structures to lower revenue leakage.
4. **Market Segments:** Processing mathematical modeling onto booking streams to optimize dynamic room yield limits.

To completely answer these 4 foundational pillars, I executed a massive multi-level exploratory data analysis containing multiple detailed charts for every individual question.

---

## 📈 Detailed Exploratory Data Analysis (EDA)

### 📊 1. Univariate Analysis (Single-Variable Distributions)
1. **Bar Chart of Hotel Types:** Visualizing the absolute volume split between City Hotels and Resort Hotels.
2. **Cancellation Rate Distribution:** A clear count plot detailing the baseline proportion of checked-in vs. canceled bookings.
3. **Market Segment Distribution:** Evaluating the frequency share of incoming traffic (Online TA, Direct, Corporate, Groups, etc.).
4. **Deposit Type Distribution:** Visualizing the share of contract structures (No Deposit, Non-Refundable, Refundable).
5. **Lead Time Distribution:** A distribution plot tracking the overall advanced scheduling horizon of reservation books.
6. **ADR (Average Daily Rate) Histogram:** Pinpointing the frequency distribution of average room prices per day.
7. **Total Stay Nights Distribution:** Analyzing the common concentration of actual duration lengths spent by travelers.
8. **Descriptive Statistics Table:** Generating comprehensive data tables containing mean, median, standard deviation, and variance parameters for every single numerical feature.

### 🔀 2. Bivariate Analysis (Two-Variable Relationships)
1. **Volume Fluctuations by Month/Season:** Comparative tracking of monthly reservation peaks and valleys across City Hotels versus Resort environments.
2. **Cancellation Rates by Market Segment:** Determining exactly which transaction avenue (Online Travel Agencies, Direct, Offline Agents, or Corporate) carries the greatest dropout frequency.
3. **Deposit Strategy Impacts:** Evaluating if strict Non-Refundable policies reduce structural booking cancellations when contrasted with No Deposit terms.
4. **Family Composition vs. Hotel Preferences:** Cross-tabulating guest demographics (families with children) against target property type choices.
5. **Lead Time for Canceled vs. Non-Canceled:** Side-by-side **Box Plots** evaluating whether reservations locked in far in advance exhibit a higher probability of cancellation than short-horizon bookings.
6. **Monthly Occupancy Profile:** Extracting the true percentage distribution of realized bookings across months to locate the single highest capacity peak of the calendar year.
7. **Lead Time Horizons by Segment:** Calculating precise average reservation horizons to classify which market routes plan furthest in advance.
8. **ADR Variations by Hotel Type:** Directly contrasting operational daily rates to pinpoint which hotel format yields premium pricing models.
9. **Lead Time vs. ADR Link (Scatter Plot):** Testing for a potential correlation or pricing curve mapping booking horizons against target transaction values.

### 🗺️ 3. Multivariate Analysis (Complex Cross-Variable Connections)
1. **Cancellation Heatmap (Month vs. Hotel Type):** A custom color-coded matrix displaying months on one axis and property types on the other, with the hue mapped to cancellation rates to instantly isolate operational risk red zones.
2. **Feature Correlation Matrix:** A full correlation map evaluating directional trends among core numeric variables: `lead_time`, `adr`, `total_nights`, `total_of_special_requests`, `previous_cancellations`, and `is_canceled`.
3. **Longitudinal Cancellation Trends:** Grouping data slices by arrival years and calendar months to build a clear line timeline tracking whether cancellation issues are increasing, decreasing, or flattening over time.
4. **Pair Plot Integration:** Building global matrix grid visualizations across selected features to instantly map joint distributions and multi-variable shapes.

---

## 🧪 Statistical Inferential Hypothesis Testing

To back up visual findings with pure mathematical certainty, I formulated and executed two distinct advanced hypothesis validation tests:

### 🔬 Hypothesis Test 1: Deposit Type vs. Cancellation Proportions
* **Business Question:** Does requiring a Non-Refundable deposit effectively reduce cancellation rates compared to a No Deposit arrangement?
* **Null Hypothesis ($H_0$):** There is no association between deposit type and reservation cancellation status. The cancellation rate is mathematically identical across all deposit categories.
* **Alternative Hypothesis ($H_1$):** There is a statistically significant association between deposit type and cancellation status. Specifically, Non-Refundable deposits showcase lower cancellation volumes than No Deposit entries.
* **Test Selection & Rationale:** Both parameters are categorical variables. Deposit type contains three factors (*No Deposit*, *Non-Refundable*, *Refundable*), and Cancellation status contains two factors (*canceled*, *not canceled*). A **Chi-Square Test of Independence** was selected to mathematically establish dependency.
* **Significance Level ($\alpha$):** 0.05

### 🔬 Hypothesis Test 2: Booking Horizons Across Reservation Vectors
* **Business Question:** Do Online Travel Agency (OTA) bookings feature significantly different advanced lead time parameters compared to customers booking Direct?
* **Null Hypothesis ($H_0$):** There is zero difference in mean booking lead times between Online Travel Agency (OTA) paths and Direct consumers. ($\mu_{OTA} = \mu_{Direct}$)
* **Alternative Hypothesis ($H_1$):** There is a statistically significant difference in mean booking lead times between Online Travel Agency (OTA) paths and Direct consumers. ($\mu_{OTA} \neq \mu_{Direct}$)
* **Test Selection & Rationale:** This evaluates continuous numerical distributions across two distinct independent categorical populations. A **Two-Sample Independent T-Test (Welch's T-Test)** was applied to process variations without assuming equal group variances.
* **Significance Level ($\alpha$):** 0.05

---

## 🛠️ Tech Stack & Dependencies
* **Development Language:** Python 3
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, SciPy (Stats Module)
* **Code Standard:** Fully modernized code block styling — all legacy warning outputs have been handled (such as resolving index chained assignments to make the pipeline 100% compatible with Pandas 3.0 processing behavior).
