# Social Media and Mental Health Analysis

This repository contains two related DAT 301 projects examining associations between daily social media screen time and mental health outcomes. The analyses focus on anxiety measured by GAD-7 and depression measured by PHQ-9, with additional comparisons by gender and social media activity type.

## Research questions

- How is daily screen time associated with GAD-7 anxiety scores?
- How is daily screen time associated with PHQ-9 depression scores?
- Do these relationships differ by gender or by active versus passive social media use?
- Does screen time remain associated with mental health scores after accounting for age, gender, and activity type?

## Dataset

The analysis uses a Kaggle social media and mental health dataset with 8,000 observations and 15 original variables. Variables include demographics, social media behavior, sleep duration, and mental health measures.

The primary variables used in the projects are:

| Variable | Description |
| --- | --- |
| Age | Participant age |
| Gender | Self-reported gender |
| Daily Screen Time | Average daily social media use in hours |
| Activity Type | Active use, such as posting, or passive use, such as scrolling |
| GAD-7 Score | Generalized anxiety score from 0 to 21 |
| PHQ-9 Score | Depression score from 0 to 27 |

## Project 1: R analysis

Project 1 uses R for data cleaning, exploratory analysis, correlation analysis, and visualization. It examines screen time in relation to GAD-7 and PHQ-9 scores and compares correlations by gender and activity type.

Tools and packages:

- R and R Markdown
- `dplyr`
- `ggplot2`
- `plotly`
- `knitr`, `kableExtra`, and `DT`

Files:

- [`Project1_Jiyoo_Lee.Rmd`](project%201/Project1_Jiyoo_Lee.Rmd) — source analysis and presentation
- [`Project1_Jiyoo_Lee.html`](project%201/Project1_Jiyoo_Lee.html) — rendered presentation
- [`social_media_mental_health.csv`](project%201/social_media_mental_health.csv) — dataset used in Project 1

## Project 2: Python extension

Project 2 reproduces and extends the analysis in Python. In addition to correlations and visualizations, it fits separate multiple linear regression models for GAD-7 and PHQ-9 scores using screen time, age, gender, and activity type as predictors.

Tools and packages:

- Python and Jupyter Notebook
- pandas and NumPy
- Matplotlib and seaborn
- SciPy
- statsmodels

Files:

- [`Jiyoo Lee_Project 2.ipynb`](project%202/Jiyoo%20Lee_Project%202.ipynb) — Python analysis notebook
- [`Jiyoo Lee_Project 2.html`](project%202/Jiyoo%20Lee_Project%202.html) — rendered notebook
- [`Jiyoo Lee_Project 2.pdf`](project%202/Jiyoo%20Lee_Project%202.pdf) — final PDF report
- [`social_media_mental_health.csv`](project%202/social_media_mental_health.csv) — dataset used in Project 2

## Main findings

- Daily screen time has a positive association with both anxiety and depression scores.
- Screen time and GAD-7 scores have a correlation of approximately `r = 0.63`.
- Screen time and PHQ-9 scores have a correlation of approximately `r = 0.59`.
- Differences by gender are minimal, while the relationship is stronger among active users than passive users.
- The multiple regression model explains approximately 46% of the variation in GAD-7 scores and 35% of the variation in PHQ-9 scores.
- Screen time remains positively associated with both outcomes after accounting for age, gender, and activity type.

These results describe associations, not causal effects.

## Running the analyses

### Project 1

Open `project 1/Project1_Jiyoo_Lee.Rmd` in RStudio. Install the required R packages if needed:

```r
install.packages(c("dplyr", "ggplot2", "plotly", "knitr", "kableExtra", "DT"))
```

Render the R Markdown file from within the `project 1` directory so that its relative dataset path resolves correctly.

### Project 2

Install the Python dependencies:

```bash
python3 -m pip install pandas numpy matplotlib seaborn scipy statsmodels jupyter
```

Launch the notebook from the `project 2` directory:

```bash
jupyter notebook "Jiyoo Lee_Project 2.ipynb"
```

## Limitations

- The dataset is observational, so the analysis cannot establish causation.
- Screen time and mental health scores are self-reported.
- The participant age range is narrow, mostly 18 to 22 years old.
- Active and passive use are broad categories that may not capture the complexity of social media behavior.
- Other relevant factors, such as prior mental health conditions and offline social support, are not included in the models.

## Author

Jiyoo Lee  
DAT 301 Projects 1 and 2
