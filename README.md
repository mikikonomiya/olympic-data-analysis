# Olympic Performance Trends: A Tri-Pillar Statistical Analysis

This repository contains a comprehensive data analysis of the Modern Olympic Games (1896–2016), investigating the evolution of the event through **Economic**, **Social**, and **Biological** lenses. 

The project moves beyond descriptive statistics to apply rigorous hypothesis testing, exploring how global progress is reflected in the world's premier sporting event.

---

## 📊 The Three Pillars

### 1. Economic Pillar: Persistent Financial Links
* **Objective:** To determine the correlation between a nation's GDP and its Olympic success.
* **Methodology:** Correlation analysis and visualization of medal counts against economic indicators.
* **Key Finding:** Strong, persistent links remain between national wealth and the ability to produce podium-level athletic talent.

### 2. Social Pillar: Converging Gender Participation
* **Objective:** To analyze the trajectory toward gender parity in the Games.
* **Methodology:** **Pearson’s Chi-Squared Test** applied to gender proportions across eras.
* **Technical Note:** Data from 1896 was excluded to satisfy the statistical assumption of **Expected Frequencies** ($N > 5$), ensuring a mathematically valid p-value.
* **Finding:** A significant shift from a "thin sliver" of participation to near 50% parity in the modern era.

### 3. Biological Pillar: Enhanced Athlete Longevity
* **Objective:** To test if modern sports medicine has extended the "performance window" of elite athletes.
* **Methodology:** A **Welch Two-Sample t-test** comparing two 16-year windows: 1960–1976 vs. 2000–2016.
* **Statistical Rigor:** * Leveraged the **Central Limit Theorem (CLT)** to ensure the normality of the sampling distribution of the mean despite right-skewed raw age data.
    * Utilized **Welch’s t-test** ($df \approx 103,224$) to account for unequal variances and unequal group sizes.
* **Result:** A statistically significant rightward shift of **1.36 years** in the biological peak of athletes ($p < 2.2e-16$).

---

## 🛠️ Tech Stack & Tools
* **Language:** R, Python
* **Environment:** Google Colab

## 📂 Repository Structure
* `notebooks/`: Separate Google Colab notebooks for each research question.
* `data/`: Contains the cleaned and filtered subsets used for the analysis.
* `presentation/`: Full project summary and slides (PDF).

## 💾 Data Sources
The raw data was sourced from the **Kaggle "120 years of Olympic history: athletes and results"** and the **World GDP by Country: 1960-2022**. Custom subsets and cleaning scripts were used to generate the era-specific data for the comparative analysis.

## ⚖️ License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.