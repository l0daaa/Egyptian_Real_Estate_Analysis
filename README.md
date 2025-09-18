# 🏡 Egypt Real Estate Market Analysis  

## 📌 Project Overview  
This project analyzes the **Egypt Real Estate Listings Dataset (2025)** to uncover key insights about property prices, sizes, payment methods, and geographic trends.  
The goal is to understand the drivers of property values and provide **data-driven recommendations** for real estate stakeholders.  

---

## 📂 Dataset  
- **Source:** Egypt Real Estate Listings (CSV file)  
- **Size:** ~50,000+ property records  
- **Key Fields:**
  - `price`: Property price (EGP)  
  - `size`: Property size (sqm)  
  - `bedrooms`, `bathrooms`, `maid_room`  
  - `type`: Apartment, Villa, Chalet, etc.  
  - `payment_method`: Cash or Installments  
  - `location`: Governorate, City, Compound  

---

## ⚙️ Data Preparation  
- Cleaned and transformed raw data (removed irrelevant fields, fixed types, dropped errors).  
- Split **location** into `governorate`, `city`, and `compound` for better granularity.  
- Created new features:
  - `price_per_sqm` (price efficiency metric).  
  - `size_bin` (grouped property sizes).  
  - `maid_room` (binary indicator).  
- Handled missing values using **grouped imputation with global fallback**.  
- Optimized memory by converting categorical/text fields to efficient datatypes.  

---

## 📊 Exploratory Data Analysis (EDA)  
### 🔹 Univariate Analysis  
- **Size, Bedrooms, Bathrooms, Price** distributions.  
- Identified outliers → treated carefully as they represent luxury segments.  

📌 *Figures: Histograms, Boxplots*  

### 🔹 Categorical Variables  
- Property types (Apartments dominate).  
- Payment methods (Cash > Installments).  
- Geographic distribution (Cairo, North Coast, Giza lead).  

📌 *Figures: Countplots*  

### 🔹 Bivariate Analysis  
- **Price vs Size, Bedrooms, Bathrooms** (scatterplots with trend lines).  
- **Price vs Payment Method** (boxplots).  
- **Price vs Governorate & Type** (barplots).  

📌 *Figures: Scatterplots, Boxplots, Barplots*  

### 🔹 Multivariate Analysis  
- Median price comparisons by **Governorate & Property Type**.  

📌 *Figure: Grouped Barplot*  

### 🔹 Price per sqm Analysis  
- Governorates with highest efficiency.  
- Top 15 cities and compounds by median price per sqm.  

📌 *Figures: Barplots for Governorates, Cities, Compounds*  

### 🔹 Correlation Analysis  
- Strongest correlations:  
  - **Price & Size (0.62)**  
  - **Bedrooms & Bathrooms (0.81)**  
- Weak link: Maid room with price.  

📌 *Figure: Correlation Heatmap*  

---

## 💡 Key Insights  
- **Location is the biggest driver** of property value.  
- **Compounds define exclusivity** → Marassi, Mountain View, Mangroovy top the market.  
- **Cash dominates luxury purchases**, installments are more common in mid-market.  
- **Apartments dominate supply**, while **Villas/Chalets dominate luxury demand**.  
- Outliers (very high prices) are **valid signals of luxury properties**, not errors.  

---

## 🎯 Recommendations  
1. Focus on **Cairo, North Coast, and Red Sea** for high-value opportunities.  
2. Expand **installment financing** for mid-market apartments.  
3. Invest in **compound branding & exclusivity** to capture premium buyers.  
4. Use **price per sqm** benchmarks for pricing strategies.  
5. Segment market into **apartments (mass), villas/chalets (luxury), compounds (premium/exclusive)**.  

---

## 📑 Report  
A detailed **PDF report** is included in the repository:  
- Data preparation  
- Exploratory data analysis  
- Key insights & visualizations  
- Recommendations for real estate stakeholders  

---

## 🛠️ Tools & Libraries  
- **Python**: Pandas, NumPy, Matplotlib, Seaborn, Missingno  
- **Jupyter Notebook** for analysis  
- **PDF Report** for stakeholders  

---

## 🚀 Next Steps  
- Build predictive models for property price estimation.  
- Add geospatial visualizations (maps of prices by region).  
- Perform buyer segmentation (if demographic data is available).  
- Incorporate time-series data for forecasting.  

---

## 📌 Author  
👤 **Khaled Youssef**  
Passionate about **data science, data analysis, and real estate analytics**.  
