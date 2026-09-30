# MATH 153 · Data Wrangling and Data Engineering

**Howard University · Department of Mathematics · Fall 2026**
Instructor: Moussa Doumbia, Ph.D.

Course materials for MATH 153: lecture slides, lecture notes, companion Jupyter notebooks, and lab directions. Real data rarely arrives ready to analyze. This course teaches you to get it there: to find and fix what is wrong, and to reshape and transform it so your question can be answered, in code you can re-run.

---

## Contents

### Outliers, Inconsistencies, and Data Quality

| File | What it is |
|---|---|
| [`outliers_beamer.pdf`](outliers_beamer.pdf) | Lecture slides |
| [`outliers_beamer_notes.pdf`](outliers_beamer_notes.pdf) | The same slides with instructor notes |
| [`outliers_simple_notes_1.pdf`](outliers_simple_notes_1.pdf) | Lecture notes with practice problems, solutions, and glossary |
| [`outliers_simple_notes_1.ipynb`](outliers_simple_notes_1.ipynb) | Runnable version of the lecture notes |
| [`outliers_data_wrangling.ipynb`](outliers_data_wrangling.ipynb) | Companion notebook: three worked cases (the Bison Half-Marathon, the \$1 Apartment, the Ice Cream Truck) |

**Topics:** kinds of outliers (error, contamination, genuine extreme) · z-score, IQR rule, modified z-score · masking and breakdown point · right-skewed data and log scales · multivariate outliers · the four kinds of inconsistency (representation, units, format, contradiction) · handling flagged values · measuring data quality.

### Reshaping, Feature Engineering, and Transformations

| File | What it is |
|---|---|
| [`Reshaping_5.pdf`](Reshaping_5.pdf) | Lecture slides |
| [`FILIGTHS.ipynb`](FILIGTHS.ipynb) | Wide vs. long with seaborn's `flights` dataset (`pivot`, `pivot_table`) |

**Topics:** wide vs. long (tidy) data · `pivot`, `pivot_table`, `melt` · building new features · scaling and log transformations.

### Labs

| File | What it is |
|---|---|
| [`MATH153_Lab01_RegEx_Directions.pdf`](MATH153_Lab01_RegEx_Directions.pdf) | Lab 4: Regular Expressions, parsing a server log and a product catalogue |

---

## Getting started

You need Python 3.10 or newer and Jupyter. The notebooks use:

```
numpy  pandas  matplotlib  seaborn
```

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

Unless a lab or homework says otherwise:

- Submit **`lastname_labXX.ipynb`**, run top to bottom with no errors, **plus a PDF export**.
- Upload to **Canvas** by the posted deadline.
- Discuss ideas with classmates, but write your own code and answers.

---

## Questions

Post on the Canvas discussion board or come to office hours. If you find a mistake in these materials, please open an [issue](https://github.com/mdoumbia1/fall_26_data_wrang/issues).

