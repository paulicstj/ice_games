# 🎮 Ice Games – Video Game Sales Analysis

## 🧊 Project Overview
**Ice** is an online store that sells video games globally. The company wants to identify patterns that determine whether a game is successful or not. This information will support strategic decisions like identifying promising projects and planning targeted advertising campaigns.

In this project, we explore historical sales data, user and expert reviews, game genres, platforms, and ESRB ratings to discover trends and build regional user profiles. We'll also use statistical hypothesis testing to validate observed differences across platforms and genres.

---

## 📁 Dataset Description

The dataset includes information such as:

- `Name`, `Platform`, `Year_of_Release`, `Genre`
- `NA_sales`, `EU_sales`, `JP_sales`, `Other_sales`
- `Critic_Score`, `User_Score`, `Rating`

---

## 🧪 Project Steps

### 🔍 1. Data Exploration & Preparation
- Loaded and examined dataset structure and quality.
- Renamed columns, handled missing values, and converted data types.
- Focused the analysis on the **most recent six years (2011–2016)** to ensure relevance for a 2017 marketing campaign.

---

### 📊 2. Descriptive Analysis
- **Sales by Year**: Sales patterns reveal generational cycles in consoles (e.g., PS3, PS4, Xbox 360). Most platforms have a lifespan of 5–7 years.
- **Platform Trends**:  
  - PS3, PS4, and Xbox 360 were dominant between 2011 and 2016.
  - PS4 and Xbox One are rising; older platforms (e.g., Wii, DS, PSP) are in decline.
- **Genre Analysis**: Action and Shooter games lead global sales, while RPGs dominate in Japan.
- **Global Sales Distribution**: Boxplots show high variance across platforms; median sales vary significantly.
- **Regional Profiles**:  
  - **NA**: Strong Xbox presence; focus on Action/Shooter.  
  - **EU**: PlayStation dominates; similar genre preference to NA.  
  - **JP**: Nintendo handhelds and RPGs are most popular.

---

### 📐 3. Hypothesis Testing

#### 📌 Hypothesis 1:
**H₀**: Average user ratings for Xbox One and PC games are the same.  
**H₁**: The averages differ.  
- **Test**: Levene's test for equal variances → Two-sample t-test  
- **Result**: Failed to reject the null — no significant difference in average ratings between Xbox One and PC.

#### 📌 Hypothesis 2:
**H₀**: Average user ratings for Action and Sports genres are the same.  
**H₁**: The averages differ.  
- **Test**: Levene's test → Two-sample t-test  
- **Result**: Rejected the null — significant difference between Action and Sports game ratings.

---

## ✅ Conclusions & Recommendations

- **PS4 and Xbox One** show the most growth potential. Campaigns should prioritize these platforms for 2017.
- **PC** provides steady but modest sales and can complement console campaigns.
- **NA** marketing should leverage Xbox loyalty and push PS4 upgrades.
- **EU** should maintain PlayStation dominance while promoting new PS4 titles.
- **JP** campaigns should target handheld consoles and genres like RPGs and family games.
- **Genre Focus**:
  - **NA & EU**: Emphasize Action and Shooter titles.
  - **JP**: Promote RPGs.
- **Age Ratings**:
  - **Teen and Mature** games dominate in NA/EU.
  - **Family-friendly** content is better received in Japan.

By tailoring campaigns to **platform life cycles**, **regional genre preferences**, and **cultural differences in ratings**, Ice can improve the accuracy and effectiveness of its marketing strategies for upcoming game releases.
