# Mental Health in the Tech Industry

An SQL and pandas analysis of the OSMI mental health surveys of tech workers (2014 and 2016–2019): who takes part,
how common mental health conditions and treatment are, and how openly mental health is discussed at work.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pboric/tech-mental-health-analysis/blob/main/Mental_Health_in_the_Tech_Industry_v2.ipynb)

## Key findings

- Participants are mostly men, but women in the survey report mental health conditions more often.
- 57 % of participants have sought treatment from a mental health professional.
- People working at large companies report diagnosed conditions somewhat more often, but the correlation analysis
  finds no significant relationship between company type and diagnoses.
- Many answers needed cleaning first (free-text gender and age values, inconsistent categories), which limits how
  precise the results can be.

## What the notebook covers

1. Loading the survey database with SQL queries (survey, question and answer tables)
2. Participation by year and country, and the age and gender of participants, after cleaning
3. Family history, diagnoses and treatment
4. Workplace questions: mental health benefits, resources, and comfort discussing mental health with coworkers,
   supervisors and in job interviews
5. Interactive charts with Plotly

## Repository

| File | Content |
|---|---|
| [`Mental_Health_in_the_Tech_Industry_v2.ipynb`](Mental_Health_in_the_Tech_Industry_v2.ipynb) | The full analysis (the interactive Plotly charts show on Colab or locally, not in GitHub's preview) |
| `mental_health.sqlite` | The survey database |

## Run it

```bash
pip install -r requirements.txt
jupyter notebook Mental_Health_in_the_Tech_Industry_v2.ipynb
```

Or open it in Colab with the badge above and upload `mental_health.sqlite`.

## Data

[Mental Health in the Tech Industry](https://www.kaggle.com/datasets/anth7310/mental-health-in-the-tech-industry) on
Kaggle, based on the [Open Sourcing Mental Health (OSMI)](https://osmihelp.org/research) surveys.

## License

MIT
