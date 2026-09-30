<div align="center">

# MATH 153 · Data Wrangling and Data Engineering

**Howard University · Department of Mathematics · Fall 2026**

Instructor: Moussa Doumbia, Ph.D.

![Python](https://img.shields.io/badge/Python-3.10%2B-003A63?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-notebooks-E51937?logo=jupyter&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-data%20wrangling-003A63?logo=pandas&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-querying-E51937)

</div>

---

Real data rarely arrives ready to analyze. This course is a comprehensive introduction to data wrangling and data engineering: how to **collect, clean, transform, and prepare** data for analysis and machine learning. It covers data formats, integration, quality assessment, and building data pipelines, with an emphasis on practical work in **Python, SQL, and data engineering frameworks**.

| | |
|---|---|
| **Meets** | Monday, Wednesday, Friday · 2:00–3:30 pm · Locke Hall, Room 208 |
| **Office hours** | Monday, Wednesday, Friday · 1:00–2:00 pm |
| **Credits** | 3 · CRN 83974 |
| **Prerequisites** | MATH 014 (Introduction to Data Science) and CSCI 135 |
| **Full syllabus** | On Canvas (contact information, policies, university services) |

## Contents

- [Learning outcomes](#learning-outcomes)
- [Weekly schedule](#weekly-schedule)
- [Repository layout](#repository-layout)
- [Getting started](#getting-started)
- [Grading](#grading)
- [Textbooks](#textbooks)
- [Submitting work](#submitting-work)
- [Questions and support](#questions-and-support)

---

## Learning outcomes

By the end of the course you will be able to:

1. **Collect** data from files, web pages, and APIs, and **integrate** data from multiple sources.
2. **Clean** data: detect and handle outliers, fix inconsistencies, and measure data quality.
3. **Reshape and transform** data, and **engineer features** for analysis and machine learning.
4. **Query** relational data with SQL, from basic queries to joins and subqueries.
5. **Validate** data and **build pipelines** with Python, SQL, and frameworks such as Airflow.
6. Work with **large-scale and complex data** (Spark, nested JSON).

---

## Weekly schedule

| Week | Topic | Materials |
|:---:|---|---|
| 1 | Introduction to data wrangling and data engineering | |
| 2 | Data manipulation libraries (pandas, NumPy) | |
| 3 | Data sources and retrieval: formats, web scraping, APIs | |
| 4 | Data integration: merging CSV and JSON | |
| 5 | **Data quality and outliers** | [📂 Lecture](lectures/week05_outliers/) · [📝 Homework](homework/week05_outliers/) |
| 6 | **Data transformation and feature engineering** | [📂 Lecture](lectures/week06_reshaping_features/) |
| 7 | Introduction to SQL | |
| 8 | Advanced SQL: joins, subqueries | |
| 9 | Data quality profiling and assessment | |
| 10 | Data validation and testing | |
| 11 | Introduction to data pipelines (ETL) | |
| 12 | Data engineering frameworks (Airflow, Luigi) | |
| 13 | Big data processing (Hadoop, Spark) | |
| 14 | Advanced data wrangling: nested JSON, performance | |
| 15 | Final projects and presentations | |

**Homework:** [📝 All assignments](homework/) · **Labs:** [🧪 Lab 4 · Regular Expressions](labs/lab04_regex/)

Materials are added as the semester goes on. Each folder has its own README listing its files.

---

## Repository layout

```
fall_26_data_wrang/
├── README.md                          ← you are here
├── requirements.txt                   ← Python packages for the notebooks
├── lectures/
│   ├── week05_outliers/
│   │   ├── README.md
│   │   ├── week05_outliers_slides.pdf
│   │   ├── week05_outliers_slides_with_notes.pdf
│   │   ├── week05_outliers_lecture_notes.pdf
│   │   ├── week05_outliers_lecture_notes.ipynb
│   │   └── week05_outliers_companion.ipynb
│   └── week06_reshaping_features/
│       ├── README.md
│       ├── week06_reshaping_slides.pdf
│       └── week06_flights_wide_long.ipynb
├── homework/
│   ├── README.md                      ← all assignments and due dates
│   └── week05_outliers/
│       ├── README.md
│       └── week05_outliers_homework.pdf
└── labs/
    └── lab04_regex/
        ├── README.md
        └── lab04_regex_directions.pdf
```

**Naming convention:** `weekNN_topic_type` for lecture and homework files and `labNN_topic` for labs, so files stay sorted and are recognizable after download.

---

## Getting started

You need **Python 3.10+** and **Jupyter**.

**Option 1 · Anaconda (recommended).** Install [Anaconda](https://www.anaconda.com/download); everything is included.

**Option 2 · pip.**

```bash
pip install -r requirements.txt
```

**Get the materials:**

```bash
git clone https://github.com/mdoumbia1/fall_26_data_wrang.git
cd fall_26_data_wrang
jupyter notebook
```

To pick up new materials later, run `git pull` inside the folder.

**Working with the notebooks**

- Run cells **top to bottom** (Kernel → Restart & Run All). Later cells depend on earlier ones.
- Before reading a result, **predict it**.
- Change the numbers and re-run. Breaking an example is the fastest way to understand it.
- To keep your own notes, **make a copy** of a notebook first, so `git pull` never conflicts with your changes.

---

## Grading

| Component | Weight |
|---|:---:|
| Class participation | 5% |
| Assessments | 40% |
| Group project | 30% |
| Final individual project | 25% |

| A | B | C | D | F |
|:---:|:---:|:---:|:---:|:---:|
| 90–100% | 80–89% | 70–79% | 60–69% | below 60% |

- Every activity is graded 0–100. **Work not submitted receives 0.**
- **Late work is not accepted.**
- To receive credit for the course, you need a **C or higher** on the weighted average.

---

## Textbooks

- Wes McKinney, *Python for Data Analysis* (O'Reilly). Free online edition: [wesmckinney.com/book](https://wesmckinney.com/book/)
- *Data Wrangling with Python* (online resource)
- Additional readings are posted on Canvas.

---

## Submitting work

Unless an assignment says otherwise:

- Submit **`lastname_labNN.ipynb`**, run top to bottom with no errors, **plus a PDF export**.
- Upload to **Canvas** by the posted deadline.
- Discuss ideas with classmates, but write your own code and answers. The Howard University Academic Code of Conduct applies.

---

## Questions and support

- **Course questions:** post on the Canvas discussion board, or come to office hours.
- **Accommodations:** register with the Office of Student Services (oss.disabilityservices@howard.edu). Accommodations must be requested each semester.
- **Technical help:** ETS Help Desk · 202-806-2020 · huhelpdesk@howard.edu
- **Found a mistake in these materials?** Open an [issue](https://github.com/mdoumbia1/fall_26_data_wrang/issues).
