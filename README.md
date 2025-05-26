#  Netflix Dataset Cleaning Project

This project is all about cleaning and preparing a Netflix dataset for analysis. The raw data had missing values, messy date formats, and inconsistent column entries — so I rolled up my sleeves and gave it a proper cleanup!

---

## 📌 What’s Inside

- `netflix_cleaned.csv` – The cleaned and processed dataset.
- `netflix_cleaning.py` – Python script I used to clean the data step by step.
- `screenshots/` – A few screenshots showing the original file, cleaned version, and GitHub upload process.

---

## 🧽 What I Did (Cleaning Steps)

Here’s a quick overview of how I cleaned the data:

### ✅ 1. Renamed Columns
Made column names easier to read and work with in Python (like changing `listed_in` to `genre` and `type` to `content_type`).

### ✅ 2. Filled Missing Data
Some columns had missing info like:
- `country`, `director`, and `cast` → filled with `"Unknown"`
- `rating` → replaced with `"Not Rated"`
- `date_added` → filled with the most frequent date
- `duration` → filled with `"Unknown"`

### ✅ 3. Cleaned Dates
- Converted the `date_added` column into proper date format
- Pulled out the **year** and **month** a title was added to Netflix

### ✅ 4. Fixed Duration Info
- Split the `duration` into two new columns:
  - `duration_num` → the number (like 90)
  - `duration_type` → the unit (like `min` or `Season`)
- Made sure it's ready for analysis

### ✅ 5. Organized the Data
- Sorted everything by `country` (A to Z)
- Then by `content_type` (Movies before TV Shows)

### ✅ 6. Saved the Results
- Exported the final cleaned version into a new file: `netflix_cleaned.csv`
