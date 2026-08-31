The Wizard of Viz: Evaluating a Playful Approach to Learn How to
Construct Charts and Recognize Misleading Visualizations
================================================================================

This archive contains the evaluation data, analysis scripts, and survey
materials accompanying the paper.

--------------------------------------------------------------------------------
GAME
--------------------------------------------------------------------------------
The Wizard of Viz source code and deployable builds (iPad/Android) are
available at:
https://github.com/MagdalenaKejstova/VisGame_Constructing

--------------------------------------------------------------------------------
FOLDER STRUCTURE
--------------------------------------------------------------------------------

```
README.md
Mentimeter/
├── [ClassCode].pdf              Raw Mentimeter responses per class
├── MentimeterAnalysis.html      Full Likert-scale and free-text analysis
└── MisleadingVisualizations.docx  Charts used in the post-game activity
GameLogAnalysis/
├── FirstIteration/
│   ├── Accuracy per activity-Table 1.csv
│   ├── Level - Best score-Table 1.csv
│   ├── Level - First full attempt-Table 1.csv
│   ├── Level - All attempts-Table 1.csv
│   ├── Level - Badge distribution-Table 1.csv
│   ├── Level - Improving final score.csv
│   ├── Level - Gaps == Explanations-Table 1.csv
│   └── FirstIteration.ipynb     Analysis notebook (N=31)
└── SecondIteration/
    ├── ActivityFulltable.csv    Per-activity log data (N=72)
    ├── Level_summary.csv        Per-level summary data (N=72)
    └── SecondIteration.ipynb    Analysis notebook (N=72)
```
--------------------------------------------------------------------------------
DATA DESCRIPTION
--------------------------------------------------------------------------------

FIRST ITERATION (N=31, 2 schools: BORGK, BFI)

  Accuracy per activity-Table 1.csv
    Per-participant, per-level accuracy with activity counts and correct counts.

  Level - Best score-Table 1.csv
    Best score achieved per participant per level (as percentages).

  Level - First full attempt-Table 1.csv
    Time spent on the first complete attempt per participant per level.

  Level - All attempts-Table 1.csv
    Total time spent across all attempts per participant per level.

  Level - Badge distribution-Table 1.csv
    Distribution of Gold/Silver/Bronze badges per level.

  Level - Improving final score (-Improving score.csv
    Binary indicator of whether each participant improved from first to best.

  Level - Gaps == Explanations ti-Table 1.csv
    Time spent in explanation chapters between levels.

SECOND ITERATION (N=72, 3 schools: IRN, RAM1, RAM2, BRG9)

  ActivityFulltable.csv
    Detailed per-activity log: participant, level, activity name, score,
    max score, correct/error counts, time spent, returns to explanation,
    and qualitative behavior notes. Used for Table 2 (time metrics),
    Table 3 (performance metrics), and error analysis.

  Level_summary.csv
    Per-participant, per-level summary: time spent, error count,
    explanation time, score, best/first percentages, skip/read behavior,
    and restart flags.

MENTIMETER SURVEY (N=87)

  [ClassCode].pdf
    Raw exported responses per school class, including Likert-scale
    ratings (14 questions) and free-text responses (3 questions).
    Note: The survey was administered in German. English translations
    of all questions are provided in Table 6 of the paper.

  MentimeterAnalysis.html
    Statistical analysis of Likert-scale responses: descriptive statistics,
    Kruskal-Wallis tests, Dunn's post hoc comparisons, Mann-Whitney U
    tests, and Spearman correlations with age.

  MisleadingVisualizations.docx
    Charts used in the post-game misleading visualizations group
    activity.

--------------------------------------------------------------------------------
ANALYSIS NOTEBOOKS
--------------------------------------------------------------------------------

FirstIteration.ipynb
  Computes: mean best scores per level, error counts from
  raw activity logs 

SecondIteration.ipynb
  Computes: Table 2 (time-related metrics per level, replays, replayer
  times), Table 3 (first vs. best attempt scores with paired t-tests,
  Bonferroni correction, and Cohen's d), explanation time, best score
  distribution (Figure 2), and student archetype clustering (Table 5,
  Figure 3).

Notebooks can be viewed using Jupyter Notebook, JupyterLab, VS Code,
or any compatible environment.

--------------------------------------------------------------------------------
REQUIREMENTS
--------------------------------------------------------------------------------
Python 3.10+
pandas, numpy, scipy, statsmodels, matplotlib (for notebooks)

--------------------------------------------------------------------------------
CONTACT
--------------------------------------------------------------------------------
For questions about the data or analysis, please contact:
Magdaléna Kejstová — makej@mail.muni.cz
Magdalena Boucher — magdalena.boucher@ustp.at
