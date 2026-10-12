# HR Analytics Dashboard – Employee Attrition (Tableau)

An interactive Tableau dashboard that analyses employee attrition for a company of 1,470 employees. It helps HR understand **who is leaving, from where, and why**, so retention efforts can be targeted.

**Tools:** Excel (data source) · Tableau Public / Desktop (calculated fields, worksheets, dashboard)

---

## 1. Business Problem

High attrition is costly: recruitment, training and lost productivity. HR leadership wants answers to:

1. What is the overall attrition rate and how many employees are active?
2. Which departments, education fields and age groups lose the most people?
3. Does attrition differ by gender, and how does that change with age?
4. How satisfied are employees with their jobs?

---

## 2. Dataset

| Item | Detail |
|---|---|
| File | `HR_Data.xlsx` (sheet: `HR data`) |
| Size | 1,470 employees × 39 columns |
| Missing values / duplicates | None found |

**Key columns:** Attrition (Yes/No), Age, CF_age band, Gender, Department, Job Role, Education Field, Marital Status, Business Travel, Over Time, Monthly Income, Job Satisfaction, Work Life Balance, Years At Company, Years Since Last Promotion, and more.

---

## 3. Project Steps

### Step 1 – Connect the data
Connected Tableau to `HR_Data.xlsx` and checked that every field has the right data type (dimensions vs measures).

### Step 2 – Prepare the data
- Verified there are no nulls or duplicate employees.
- Used the helper fields in the data (e.g. age bands and attrition labels such as "Ex-Employees" / current employee flag) to simplify filtering.

### Step 3 – Create calculated fields
| Field | Purpose |
|---|---|
| Attrition Count | Number of employees who left |
| Active Employees | Number of current employees |
| Attrition Rate | Attrition Count ÷ total employees |
| Age (bin) / Bin Size | Age groups for the age analysis |

### Step 4 – Build the worksheets
| # | Worksheet | Question answered |
|---|---|---|
| 1 | KPI | Headline numbers: total employees, attrition count, attrition rate, active employees |
| 2 | Attrition by Gender | Do men or women leave more? |
| 3 | Department wise Attrition | Which departments lose the most people? |
| 4 | Education Field wise Attrition | Which education backgrounds leave most? |
| 5 | No of Employee by Age Group | What does the age profile look like? |
| 6 | Attrition Rate by Gender for different Age groups | How does attrition vary by age and gender together? |
| 7 | Job Satisfaction Rating | How satisfied are employees? |

### Step 5 – Design the dashboard
Combined the worksheets into **HR ANALYTICS DASHBOARD1** with a custom background image, KPI tiles at the top and the charts arranged below for a single-page view of attrition.

### Step 6 – Interpret and share
Drew the insights below and packaged the workbook as a `.twbx` so it can be opened with the data included.

---

## 4. Key Insights

- **Overall attrition is 16.1%** (237 of 1,470 employees have left).
- **Sales has the highest department attrition (~20.6%)**, followed by HR (~19%); R&D is lowest (~13.8%).
- **Age matters:** employees **under 25 leave at ~39%**, and the 25–34 group at ~20%. Attrition falls to about 10% for ages 35–54.
- **Gender:** men leave slightly more than women (~17% vs ~15%).
- **Education field:** Human Resources (~26%), Technical Degree (~24%) and Marketing (~22%) backgrounds show the highest attrition.
- **Other drivers visible in the data:** employees who work overtime leave at ~30.5% vs ~10.4% for those who don't; single employees leave at ~25.5%; frequent travellers at ~25%.
- **Pay and satisfaction:** leavers earn less on average (average monthly income of about 4,787 vs 6,833) and report lower job satisfaction (about 2.5 vs 2.8 out of 4).

---

## 5. Recommendations

1. **Focus retention in Sales and HR**, especially Sales Representatives (~40% attrition).
2. **Support young employees** with mentoring, career paths and onboarding, since under-25s are the biggest flight risk.
3. **Review overtime and travel load**, which are linked to much higher attrition.
4. **Review pay for lower-income roles** and tie increases to retention goals.
5. **Run regular satisfaction surveys** and act on low-scoring areas early.

---

## 6. How to Open

1. Download `HR Analytics dashboard Tableau project 1.twbx` and open it in Tableau Public or Tableau Desktop.
2. Open the **HR ANALYSTICS DASHBOARD1** tab to explore the dashboard, or any worksheet tab to see a single chart.

## 7. Repository Structure

```
├── HR Analytics dashboard Tableau project 1.twbx   # Tableau workbook + dashboard
├── HR_Data.xlsx                                    # Source data
└── README.md
```

## 8. Skills Demonstrated

Tableau calculated fields · KPI design · Dashboard layout · Attrition analysis · Business storytelling

---

**Author:** Astha Kumari Jha
**GitHub:** [github.com/Asthajha4275](https://github.com/Asthajha4275)
