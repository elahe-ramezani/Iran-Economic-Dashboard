# Iran Economic Dashboard | Power BI

An interactive Power BI dashboard analyzing Iran's economic position relative to neighboring countries from 2020 to 2024.

---

## 📊 Project Overview

This project analyzes Iran's economic position relative to neighboring countries using Nominal GDP (Current USD) as the primary economic size indicator.

The dashboard combines GDP data with selected macroeconomic indicators, including:

- GDP Growth
- Inflation
- GDP per Capita
- GDP Ranking
- Regional GDP Share
- GDP Gap Analysis
- Economic Volatility

The objective is to transform economic data into an interactive analytical story that explains Iran's relative position, economic performance, regional competitiveness, and key economic challenges.

---

## 🎯 Key Questions

This dashboard answers the following questions:

- What is Iran's economic position relative to neighboring countries?
- How has Iran's regional GDP ranking changed over time?
- How large is the GDP gap between Iran and the regional leader?
- Is the GDP gap widening or narrowing?
- How volatile are GDP growth and inflation?
- How does Iran compare with neighboring economies geographically?
- What are Iran's main economic strengths and challenges?

---

## 📈 Dashboard Structure

The dashboard follows a progressive analytical story:

**Relative Position → Ranking Dynamics → Gap Analysis → Volatility → Geographic Comparison → Executive Summary**

---

## 🖼️ Dashboard Preview

### 1. Relative Economic Position

Overview of Iran's economic position compared with neighboring countries.

![Relative Economic Position](Screenshots/01-relative-position.JPG)

---

### 2. Ranking Dynamics

Analysis of Iran's GDP ranking and economic performance trends over time.

![Ranking Dynamics](Screenshots/02-ranking-dynamics.JPG)

---

### 3. Gap Analysis

Analysis of Iran's GDP gap relative to the regional leader and regional median.

![Gap Analysis](Screenshots/03-gap-analysis.JPG)

---

### 4. Volatility & Fluctuation

Analysis of GDP growth volatility and inflation volatility across the selected period.

![Volatility & Fluctuation](Screenshots/04-volatility-fluctuation.JPG)

---

### 5. Map & Relative Strength

Geographic comparison of economic size and relative economic strength across neighboring countries.

![Map & Relative Strength](Screenshots/05-map-relative-strength.JPG)

---

### 6. Executive Economic Summary

Final comparison of key economic indicators and regional economic composition.

![Executive Economic Summary](Screenshots/06-executive-summary.JPG)

---

## 🔍 Key Findings

- Iran remained among the largest economies in the analyzed regional comparison.
- Iran maintained the second position in the selected regional GDP ranking during the analyzed period.
- Iran's GDP remained significantly below the regional leader.
- The GDP gap with the regional leader widened during the later years of the analysis period.
- Inflation volatility exceeded GDP growth volatility.
- Iran remained one of the region's major economic powers based on nominal GDP.

---

## 📊 Main Analytical Perspectives

### Relative Economic Position

Evaluates Iran's current position based on:

- GDP Rank
- Regional GDP Share
- GDP Gap to Regional Leader
- GDP Gap to Regional Median

### Ranking Dynamics

Analyzes:

- GDP ranking trends
- Rank stability
- GDP growth trends
- Comparative regional performance

### Gap Analysis

Measures:

- GDP distance from the regional leader
- GDP distance from the regional median
- Year-over-year gap changes
- Gap direction and convergence/divergence

### Volatility & Fluctuation

Evaluates:

- GDP growth standard deviation
- Inflation volatility
- Economic volatility
- GDP growth and inflation trends

### Map & Relative Strength

Provides a geographic view of:

- Regional GDP distribution
- Economic strength
- Relative position of Iran
- Stronger and weaker neighboring economies

---

## 🧮 Data Model

The project uses a dimensional data model designed for analytical reporting.

### Main Tables

#### FactEconomy

Contains economic observations by country and year, including:

- GDP
- GDP Growth
- Inflation
- GDP per Capita
- Exports
- Imports
- Other economic indicators

#### DimCountry

Contains country-level attributes, including:

- Country Name
- Country Code
- Region
- Income Group
- Oil Exporter Classification

#### DimDate

Contains the time dimension used for:

- Year filtering
- Time-based analysis
- Year-over-year comparisons
- Historical trends

---

## 📐 Key DAX Measures

Examples of the main analytical measures used in the project:

```DAX
Total GDP =
SUM(FactEconomy[GDP])
