Of course! Based on your new dashboard design and the provided example, here is a new README file tailored for your **Financial Risk Dashboard**.

---

# Financial Risk Analytics Dashboard

---

## 📋 Table of Contents

- [📊 Project Overview](#-project-overview)
- [🎯 Key Metrics & KPIs](#-key-metrics--kpis)
- [🚀 Dashboard Features](#-dashboard-features)
- [📈 Trends Analysis](#-trends-analysis)
- [🔧 Technical Details](#-technical-details)
  - [📊 Data Sources](#-data-sources)
  - [🗃️ Data Model](#-data-model)
- [🎮 How to Use This Dashboard](#-how-to-use-this-dashboard)
- [💡 Key Insights & Recommendations](#-key-insights--recommendations)
- [📁 Project Structure](#-project-structure)
- [🛠️ Project Development](#-project-development)
- [📞 Contact](#-contact)

---

## 📊 Project Overview

This Financial Risk Dashboard offers a comprehensive analytical view of a loan application portfolio. Designed for risk managers, credit analysts, and financial stakeholders, it provides crucial insights into applicant profiles, risk distribution, and portfolio health. The dashboard enables data-driven decision-making to optimize underwriting processes, manage portfolio risk, and ensure sustainable lending practices.

### Project Goals:

-   Monitor the overall risk level of the loan application portfolio in real-time.
-   Identify and analyze high-risk segments based on various client attributes.
-   Track key risk indicators like DTI, LTI, and Credit Score.
-   Analyze trends in application volume and client risk profiles over time.
-   Provide actionable insights to refine credit policies and mitigate potential losses.

### Key Features:

-   High-level summary of critical risk and volume KPIs.
-   Interactive filtering by Year, Month, Payment History, Loan Purpose, and Risk Rating.
-   Detailed analysis of risk based on employment status and credit score.
-   Time-series visualization to track application trends and seasonality.

---

## 🎯 Key Metrics & KPIs

### Primary Risk KPIs

-   **Total Applications:** 15K applications in the portfolio.
-   **Risk Rate (%):** 10% of applications are classified as high risk.
-   **Average Debt-to-Income (DTI):** 0.35, indicating the average portion of income used for debt payments.
-   **Average Loan-to-Income (LTI):** 0.39, showing the average loan size relative to client income.
-   **Average Credit Score:** 699.11, a key indicator of historical creditworthiness.

---

## 🚀 Dashboard Features

### Dynamic Slicers and Filters

-   **Temporal Filters:** Year and Month selection for time-series and point-in-time analysis.
-   **Attribute Filters:** Drill down into specific segments by Payment History, Loan Purpose, and assigned Risk Rating.
-   **Instant Updates:** All visuals on the dashboard update in real-time based on filter selections.

### Advanced Visualizations

-   **KPI Cards:** At-a-glance view of the most critical portfolio metrics.
-   **Time Series Line Chart:** Tracks total, maximum, and minimum application volumes by month to identify trends and seasonal patterns.
-   **Pie Chart:** Displays the overall distribution of clients across High, Medium, and Low risk ratings.
-   **Stacked Bar Chart:** Breaks down the risk profile for different employment statuses, allowing for direct comparison.
-   **Combo Chart:** Correlates application volume with credit score brackets while showing the trend of the average credit score.

---

## 📈 Trends Analysis

### Application Volume Patterns

-   **Monthly Trends:** Application volume shows seasonality, peaking in March (1.54K) and hitting a low in September (0.94K).
-   **Year-over-Year:** The 'Year' filter allows for comparison of application trends across different years.

### Risk Distribution Insights

-   **Overall Risk:** The majority of clients (60%) are categorized as Low Risk, with 10% being High Risk.
-   **Employment Status:** Risk profiles are remarkably consistent across Employed, Self-employed, and Unemployed segments, with each showing a ~33% high-risk component. This suggests employment status is not a primary driver of risk in this portfolio.
-   **Credit Score Impact:** The largest volume of applications originates from clients in the 600-649 credit score bracket. The trendline clearly shows that higher credit score brackets correlate with better average scores.

---

## 🔧 Technical Details

### 📊 Data Sources

#### Core Systems:

-   Loan Origination System (LOS)
-   Core Banking Platform
-   Client Relationship Management (CRM) System

#### Data Specifications:

-   **Volume:** 15K+ loan application records.
-   **Data Fields:** Includes client demographics, financial details, credit history, and loan specifics.
-   **Update Frequency:** Designed for daily or weekly data refreshes to ensure timely insights.

### 🗃️ Data Model

#### Core Tables:

-   **Applications:** Contains all transactional data for each loan application (`ApplicationID`, `ClientID`, `LoanAmount`, `ApplicationDate`, `LoanPurpose`, `Status`).
-   **Clients:** Stores demographic and financial data for each client (`ClientID`, `EmploymentStatus`, `ClientIncome`, `CreditScore`).
-   **Risk:** Holds the calculated risk metrics for each application (`ApplicationID`, `DTI`, `LTI`, `RiskRating`).

---

## 🎮 How to Use This Dashboard

1.  **Get a High-Level View:** Start with the top KPI cards to understand the overall health of the portfolio.
2.  **Analyze Trends:** Use the "Client Trends by Month" chart to identify any unusual spikes or dips in application volume. Use the 'Year' and 'Month' filters to narrow down the period.
3.  **Drill Down into Risk:** Use the filters on the top right (`Payment History`, `Loan Purpose`, `Risk Rating`) to isolate specific segments. For example, filter for "High" `Risk Rating` and "Debt Consolidation" `Loan Purpose` to see if that combination poses a significant problem.
4.  **Investigate Segments:** Analyze the "Risk Profile by Employment Status" and "Credit Score Distribution" charts to understand the drivers behind the risk in your filtered segment.

---

## 💡 Key Insights & Recommendations

### Major Discoveries

-   **Low Credit Score Volume:** The highest number of applications comes from the 600-649 credit score range, which typically carries higher risk.
-   **Employment Parity:** The risk distribution is nearly identical across all employment types, indicating that the current risk model does not heavily differentiate based on this attribute. This may be an area for model refinement.
-   **Majority Low Risk:** A strong base of 60% of clients is rated as low risk, which is a positive indicator for portfolio health.

### Strategic Recommendations

#### Risk Policy & Underwriting:

1.  **Review Low Credit Score Segment:** Given the high volume of applications from the 600-649 credit score bracket, review underwriting standards and pricing for this group to ensure risk is adequately compensated.
2.  **Enhance Risk Model:** Since employment status does not appear to be a strong risk differentiator, consider incorporating alternative data or refining model weightings to better capture risk variations between these groups.
3.  **Promote to Medium Risk Clients:** Target marketing or pre-approval campaigns towards the 30% of clients in the "Medium" risk category to help them transition to lower-risk products over time.

---

## 📁 Project Structure

#### Financial_Risk_Dashboard_PowerBI/

|--- README.md # Project documentation
|--- Financial_Risk_Dashboard.pbix # Main Power BI dashboard file
|--- Screenshot/ # Dashboard visual
|   └── financial risk dashboard.png # Dashboard preview image
|--- Data/ # Data sources folder
    |--- loan_applications.csv # Primary data source
    
---

## 🛠️ Project Development

-   **Tool Used:** Power BI Desktop
-   **Dataset:** Sample Financial Data *(anonymized/synthetic)*
-   **Development Time:** Personal project

### 🚧 Key Development Challenges

-   **Metric Definition:** Creating accurate and robust DAX calculations for KPIs like LTI and DTI.
-   **Data Modeling:** Structuring the data model to allow for efficient filtering and cross-analysis between client attributes and loan details.
-   **Visual Clarity:** Designing visuals (e.g., color schemes, chart types) that are intuitive and do not misrepresent risk (e.g., avoiding red for positive trends).

### 🚀 Future Enhancements

-   **Predictive Analytics:** Incorporate a machine learning model to predict the probability of default for new applications.
-   **What-If Analysis:** Add parameters to allow users to simulate how changes in underwriting criteria (e.g., lowering acceptable DTI) would impact the portfolio's risk rate and volume.
-   **Automated Alert System:** Create alerts for when key risk metrics breach predefined thresholds.

---

## 📞 Contact

-   **Email:** ekaterine.mashchenko.1@btu.edu.ge
-   **LinkedIn:** https://www.linkedin.com/in/ekaterine-mashchenko-b497a5235/
-   **GitHub:** https://github.com/Katherinam4
