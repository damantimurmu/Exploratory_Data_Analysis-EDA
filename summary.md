# **Observations**

### **Univariate Analysis**
1. **Age**:
   - The age distribution appears fairly uniform, with slightly higher counts in the younger and older age brackets.

2. **Fever**:
   - Three distinct peaks suggest grouped classification: Mild, Moderate, and High fever.

3. **Gender**:
   - Balanced distribution of Male and Female participants.

4. **Chest Pain, Night Sweats, Blood in Sputum, Previous TB History**:
   - Binary responses show nearly equal counts, indicating these symptoms are common in both TB and non-TB cases.

5. **Cough Severity & Breathlessness**:
   - Severity is spread across a range (0–9 for cough, 0–4 for breathlessness), indicating varying degrees in patients.

6. **Sputum Production & Smoking History**:
   - Balanced distribution across categories (e.g., low, medium, high; never, former, current).

7. **Class**:
   - Imbalanced dataset: Majority are labeled “Normal”, fewer are “Tuberculosis”.

---

### **Bivariate Analysis**
1. **Pairplot**:
   - Minor visual separation between TB and non-TB for features like Fever and Weight Loss.
   - Class 1 (Tuberculosis) points show slight clustering toward higher fatigue, fever, and weight loss.

2. **Violin/Box Plots**:
   - **Fever, Fatigue, Weight Loss**: TB patients generally have higher values.
   - **Age**: TB can occur at any age, but slight increase in younger to middle-aged patients.

3. **Correlation Heatmap**:
   - Very weak correlation between numerical features (values close to 0).
   - Fatigue and Weight Loss have a small positive correlation.

---

# **Summary of Findings**
- **Symptoms like Fever, Fatigue, and Weight Loss** show **stronger presence in TB-positive cases**.
- Dataset has **class imbalance**, with many more normal cases than TB, which needs attention during modeling (e.g., using SMOTE or class weights).
- Cough Severity and Breathlessness are **diverse**, which may help model granularity in symptoms.
- No strong linear correlations among features — suggesting **non-linear modeling approaches** like decision trees, random forests, or boosting might be suitable.
- **Categorical features** (e.g., Chest Pain, Previous TB History) may serve as **important binary indicators**.

---

Would you like these insights as part of a PDF or PPT report, or integrated directly into a Jupyter markdown cell?
