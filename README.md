# College Admission Dataset India – Full Data Analysis & Power BI Dashboard

This comprehensive analysis explores the factors affecting student admissions in Indian colleges by leveraging Excel for data preparation and Power BI for interactive visualizations. The goal is to ensure high-quality data and deliver actionable insights through robust dashboards.

---

## 1. Data Preparation and Cleaning (Excel)

### Importing and Cleaning
The college admissions dataset was imported into Excel for initial processing. Key cleaning steps included removing duplicate entries in power query, especially in the **ID_Student** column, to maintain data integrity.

### Data Validation Rules
Specific validation rules were applied to each column to ensure consistent and accurate data:

| Column                   | Validation Applied                                |
|-------------------------|----------------------------------------------------|
| ID_Student              | Prevent duplicates                                 |
| Age                     | Dropdown: 17, 18, 19, 20                           |
| Gender                  | Dropdown: Male, Female, Other                      |
| Category                | Dropdown: General, OBC, SC, ST, EWS                |
| State                   | Standardized dropdown list                         |
| Preferred Stream        | Dependent dropdown based on Entrance Exam          |
| Entrance Exam           | Validation based on selected stream                |
| Entrance Score          | Between 0 and 700                                  |
| Board Percentage        | Between 0 and 100%                                 |
| Extracurricular Score   | Between 0 and 10                                   |
| Admission Probability   | Between 0 and 1                                    |

### Importance of Data Validation
These validation rules ensure that the dataset contains:
- no duplicates,
- no invalid values,
- standardized categorical fields,
- and a high level of consistency.

This creates a reliable foundation for further analysis in Power BI.

---

## 2. Preparing the Dataset for Power BI

### Calculated Columns
New columns were created to classify academic metrics, such as:
- **Board Percentage Category** (High, Medium, Low)
- **Extracurricular Score Category**(High,Medium,Low)

### DAX Measures
Key metrics were calculated using DAX, including:
- Total Students  
- Total Admitted  
- Total Rejected  
- Admission Rate  
- Rejection Rate  

### Dataset Import
After cleaning and validation, the dataset was imported into Power BI, where a four-page interactive dashboard was developed.

---

## 3. Power BI Dashboards

### **Page 1 — Student Demographics**
This page contains KPIs and visualizations such as:
- Gender distribution (donut chart)
- Age distribution (pie chart)
- Category distribution (donut chart)
- Student distribution by state (treemap)
- KPI Total student

Slicers include age, gender, category, and state.

**Insight:**  
The student population is highly balanced across gender, age, category, and state.

---

### **Page 2 — Student Academics**
This page highlights key academic indicators:
- Entrance exam participation
- SRA Curricula Score Category
- Preferred stream
- Board Percentage Category

**Key insights:**
- 45.20% of students did not sit for any entrance exam  
- Most students have high or medium board percentages  
- **Extracurricular performance influences admission likelihood**  
- Curricula scores are moderately distributed  

---

### **Page 3 — Admission Drivers Analysis**
This page focuses on the primary factors influencing admission decisions, including KPIs for:
- Total admitted
- Total rejected
- Admission rate
- Rejection rate

Visualizations include:
- Decision tree (Board %, Extracurricular Score)
- Admission rate by stream
- Admission rate by board percentage category
- Admission rate by extracurricular score category

**Key findings:**
- Medical stream shows the highest admission rate (**12.44%**)  
- Engineering stream follows (**9.88%**)  
- High board percentages and strong extracurricular scores significantly increase admission probability  

---

### **Page 4 — Admission by Demographics**
This page analyzes admissions across demographic variables:
- Admission by state
- Admission by age
- Admission by gender
- Admission by category

**Conclusion:**  
Admissions are **equitable across all demographic groups**, with a stable average admission rate of **32.51%**.

---

## 4. Summary of Key Insights

- **Student Demographics:** Highly balanced population with no demographic bias.  
- **Student Academics:**  
  - Board percentage is the strongest predictor of admission.  
  - Entrance exams are less influential.  
  - **Extracurricular scores have a moderate impact.**  
- **Admission Drivers:**  
  - Medical and engineering streams show the highest admission rates.  
  - High board percentages and extracurricular scores are the strongest drivers of admission.  
- **Admission by Demographics:**  
  - Admissions remain equitable across age, gender, state, and category.

---

## 5. Key Notes

- Excel validations ensure clean and reliable data.  
- Power BI provides dynamic and interactive insights.  
- The dashboard highlights equity and key academic drivers of admission.  
- The dataset is ready for future analysis or machine learning models.



