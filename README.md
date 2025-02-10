# **Final-Project-Statistical-Modelling-with-Python**

## **Project Goals**
The main goals of this project were:
- Correctly load data using **GET calls** from our API.
- Convert API responses into **dataframes** and save them as **CSV files**.
- **Join the correct CSVs** and **dataframes** to create a unified dataset.
- Build a **database** with the newly combined data.
- Use **visualizations** to explore relationships in the data.
- Develop a **regression model** to understand patterns in bike station capacity.

---

## **Process**
### **Step 1: Data Collection & Storage**
- Used **GET calls** to fetch data from the API.
- Converted responses into **structured Pandas dataframes**.
- Saved the data into **CSV files**.

### **Step 2: Data Merging & Database Creation**
- Combined relevant CSVs and **joined dataframes**.
- Built an **SQLite database** to store the processed data.

### **Step 3: Data Exploration & Visualization**
- Created **visuals** to better understand relationships in the dataset.

### **Step 4: Regression Model**
- Developed a **regression model** to examine how bar characteristics relate to bike station capacity.

---

## **Results**
The regression model showed:
- **R-squared = 0.007** → The model explains **only 0.7% of the variance** in `Total_Slots`, meaning it has **low predictive power**.
- **P-values (<0.05) for `Reviews` & `Yelp_Rating`** → These variables are statistically significant but have a **small negative effect** on bike station capacity.
- **Conclusion**: The model is statistically valid but does **not effectively predict** `Total_Slots`. Additional features or a different modeling approach is needed.

---

## **Challenges**
- **Forgetting `Total_Slots` initially** and having to redo the **GET requests** and **re-run scripts**.
- **Updating the database** correctly while ensuring data integrity.
- **Rebuilding the regression model** after realizing **incorrect values were included** from Foursquare results (e.g., including non-bar categories).

---

## **Future Goals**
- Explore **more features** that may better predict `Total_Slots`.
- Improve **data filtering** to remove any remaining irrelevant records.
- Test **alternative machine learning models** (e.g., Random Forest, Decision Trees) for stronger predictive power.
- Conduct **deeper statistical analysis** to find meaningful patterns.

---
