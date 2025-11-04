# A/B Testing for Landing Page Optimization 

This project analyzes the impact of a new landing page design on user engagement and conversion rate for an online news subscription platform. The company aims to determine if the new design improves key business metrics and whether user behavior varies across preferred languages.

---

##  Problem Statement

The company randomly selects 100 users and splits them equally into:

- **Control Group**: shown the **old landing page**
- **Treatment Group**: shown the **new landing page**

The goal is to answer:
1. Do users spend more time on the new landing page?
2. Is the conversion rate higher for the new page?
3. Does preferred language influence conversion behavior?
4. Is time spent affected by language on the new page?

---

##  Dataset Overview

The dataset `abtest.csv` includes:

| Column Name             | Description                                         |
|------------------------|-----------------------------------------------------|
| `user_id`              | Unique identifier for each user                     |
| `group`                | Control or Treatment                                |
| `landing_page`         | Old or New landing page                             |
| `time_spent_on_the_page` | Time (in minutes) spent on the page               |
| `converted`            | Whether the user subscribed ("yes"/"no")            |
| `language_preferred`   | User’s preferred language (English/French/Spanish)  |

---

## 🧪 Methods Used

- Exploratory Data Analysis (EDA)
- A/B Testing (Control vs Treatment)
- Hypothesis Testing
  - Independent t-test for time spent
  - Chi-Square test for conversion rate
- Group-wise analysis across languages

---

##  Key Insights

- **Users spent more time** on the new landing page (avg. higher).
- **Conversion rate improved**:  
  - Old page: **42%**  
  - New page: **66%**
-  **Language matters**:
  - French users showed **75% higher conversion** on the new page.
  - Spanish users showed **36% higher conversion**.
  - English users showed slight preference for the old page.

---

##  Tools & Technologies

- Python (Pandas, NumPy, Seaborn, Matplotlib, SciPy)
- Jupyter Notebook
- Statistical Testing

---
## Conclusion

This analysis provided actionable recommendations:
- Roll out the **new landing page**, especially for **French and Spanish users**
- Further A/B test targeting **English users** with personalized tweaks
- Monitor time-on-page and conversion metrics post-deployment

---
