# HealthCare Analysis with Python

# 🏥 No-Show Appointments Analysis (Healthcare Data)

## 📌 Project Overview

This project analyzes a real-world healthcare dataset of over 100,000 medical appointments to understand patient behavior and identify factors that influence **no-shows**. Using Python, the analysis focuses on how variables like age, gender, medical conditions, and scheduling affect whether a patient attends their appointment.

---

## 🧾 Dataset Description

Each row in the dataset represents a medical appointment with the following columns:

| Column           | Description |
|------------------|-------------|
| `patientid`      | Unique identifier for a patient |
| `appointmentid`  | Unique identifier for an appointment |
| `gender`         | Male or Female |
| `scheduledday`   | Date the appointment was scheduled |
| `appointmentday` | Actual appointment date |
| `age`            | Patient's age |
| `neighbourhood`  | Location of the clinic |
| `scholarship`    | 1 if the patient is enrolled in a welfare program |
| `hipertension`   | 1 if the patient has hypertension |
| `diabetes`       | 1 if the patient has diabetes |
| `alcoholism`     | 1 if the patient has a history of alcoholism |
| `handcap`        | Disability count (0–4) |
| `sms_received`   | 1 if the patient received a reminder SMS |
| `no_show`        | 'Yes' if the patient missed the appointment |
| `sch_weekday`    | Day of the week the appointment was scheduled |

---

## 🧹 Data Cleaning & Preprocessing

- Converted date columns to datetime format
- Standardized column names and values (e.g., fixed typos like "hipertension")
- Removed rows with invalid ages (e.g., negative values)
- Created new features such as waiting time between scheduled and appointment dates


---

## 📊 Exploratory Data Analysis (EDA)

### Key Questions Explored:

1. **What percentage of patients miss their appointments?**
   - ~20% of all scheduled patients do not show up.

2. **Does age affect attendance?**
   - Younger patients, especially under 25, are more likely to miss appointments.

3. **Does receiving an SMS reminder help?**
   - Slight improvement in show rates was observed for patients who received SMS.

4. **Are certain neighborhoods more prone to no-shows?**
   - High no-show rates were found in specific neighborhoods with low income levels.

5. **Do chronic conditions affect attendance?**
   - Patients with hypertension or diabetes tend to attend more consistently.

---

## 📈 Visualizations

- Barplot for age, gender, sms received and disease indicators
- Barh chart for neigborhoods
- Histogram for age and waiting time
- Heatmap for correlation matrix

---

## ✅ Conclusion

The analysis found that **age, waiting time, and SMS reminders** are strong indicators of appointment attendance. Socioeconomic status (scholarship enrollment) and chronic conditions also play a role in predicting no-shows.

---

## 🛠 Tools Used

- Python (Pandas, NumPy)
- Seaborn & Matplotlib
- Jupyter Notebook

---



