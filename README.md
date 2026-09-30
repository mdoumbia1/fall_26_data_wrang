# MATH 153 · Data Wrangling and Data Engineering

**Howard University · Department of Mathematics · Fall 2026**
Instructor: Moussa Doumbia, Ph.D. · 3 credit hours · CRN 83974

| | |
|---|---|
| **Meets** | Monday, Wednesday, Friday · 2:00–3:30 pm · Locke Hall, Room 208 |
| **Office hours** | Monday, Wednesday, Friday · 1:00–2:00 pm |
| **Prerequisites** | MATH 014 (Introduction to Data Science) and CSCI 135 |
| **Full syllabus** | On Canvas (contact information, policies, university services) |

---

## About the course

Real data rarely arrives ready to analyze. This course is a comprehensive introduction to data wrangling and data engineering: how to **collect, clean, transform, and prepare** data for analysis and machine learning. It covers data formats, integration, quality assessment, and building data pipelines, with an emphasis on practical work in **Python, SQL, and data engineering frameworks**.

### By the end of the course you will be able to

- Collect data from files, web pages, and APIs, and combine data from multiple sources.
- Clean data: detect and handle outliers, fix inconsistencies, and measure data quality.
- Reshape and transform data, and engineer features for analysis and machine learning.
- Query and transform relational data with SQL, from basic queries to joins and subqueries.
- Validate and test data, and build data pipelines with Python, SQL, and frameworks such as Airflow.
- Work with large-scale and complex data (Spark, nested JSON).

---

## Weekly schedule

| Week | Topic | In class | Materials in this repo |
|---|---|---|---|
| 1 | Introduction to data wrangling and data engineering | Examples of messy data | |
| 2 | Data manipulation libraries (pandas, NumPy) | Hands-on pandas for data cleaning | |
| 3 | Data sources and retrieval (formats, web scraping, APIs) | Retrieve and parse data from an API | |
| 4 | Data integration | Merge CSV and JSON datasets | |
| 5 | **Data quality and outliers** | Detect and handle outliers | [Slides](outliers_beamer.pdf) · [Slides with notes](outliers_beamer_notes.pdf) · [Lecture notes](outliers_simple_notes_1.pdf) ([notebook](outliers_simple_notes_1.ipynb)) · [Companion notebook](outliers_data_wrangling.ipynb) |
| 6 | **Data transformation and feature engineering** | Create new features from existing data | [Slides](Reshaping_5.pdf) · [Flights notebook](FILIGTHS.ipynb) |
| 7 | Introduction to SQL | Simple queries on sample databases | |
| 8 | Advanced SQL (joins, subqueries) | Joins and nested subqueries | |
| 9 | Data quality profiling and assessment | Profile a dataset's quality | |
| 10 | Data validation and testing | Build validation checks for incoming data | |
| 11 | Introduction to data pipelines (ETL) | Build a basic pipeline in Python or SQL | |
| 12 | Data engineering frameworks (Airflow, Luigi) | Design a pipeline with a framework | |
| 13 | Big data processing (Hadoop, Spark) | Process a large dataset with Spark | |
| 14 | Advanced data wrangling | Nested JSON; performance optimization | |
| 15 | Final projects and presentations | Present final projects | |

Materials are added as the semester goes on.

### Labs

| File | What it is |
|---|---|
| [`MATH153_Lab01_RegEx_Directions.pdf`](MATH153_Lab01_RegEx_Directions.pdf) | Lab 4: Regular Expressions, parsing a server log and a product catalogue |

---

## Grading

| Component | Weight |
|---|---|
| Class participation | 5% |
| Assessments | 40% |
| Group project | 30% |
| Final individual project | 25% |

| A | B | C | D | F |
|---|---|---|---|---|
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

## Getting started

You need Python 3.10 or newer and Jupyter. The notebooks use `numpy`, `pandas`, `matplotlib`, and `seaborn`.

**Option 1: Anaconda (recommended).** Install [Anaconda](https://www.anaconda.com/download); everything above is included.

**Option 2: pip.**

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

**Get the materials:**

```bash
git clone https://github.com/mdoumbia1/fall_26_data_wrang.git
cd fall_26_data_wrang
jupyter notebook
```

To pick up new materials later, run `git pull` inside the folder.

### Running the notebooks

- Run cells **top to bottom** (Kernel → Restart & Run All). Later cells depend on earlier ones.
- Before reading a result, **predict it**. The notebooks are built around "what will this print?" moments.
- Change the numbers and re-run. Breaking an example is the fastest way to understand it.

---

## Submitting work

Unless a lab or assignment says otherwise:

- Submit **`lastname_labXX.ipynb`**, run top to bottom with no errors, **plus a PDF export**.
- Upload to **Canvas** by the posted deadline.
- Discuss ideas with classmates, but write your own code and answers. The Howard University Academic Code of Conduct applies.

---

## Questions and support

- **Course questions:** post on the Canvas discussion board, or come to office hours.
- **Accommodations:** register with the Office of Student Services (oss.disabilityservices@howard.edu). Accommodations must be requested each semester.
- **Technical help:** ETS Help Desk, 202-806-2020, huhelpdesk@howard.edu.
- **Found a mistake in these materials?** Open an [issue](https://github.com/mdoumbia1/fall_26_data_wrang/issues).
