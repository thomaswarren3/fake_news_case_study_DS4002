# Fake News Detection — Case Study

A case study for 2nd year UVA Data Science students exploring how 
machine learning can be used to classify news articles as fake or real.

## Overview
Can a machine tell the difference between fake and real news? In this 
case study you will explore a large dataset of news articles, uncover 
patterns through EDA and clustering, and build classifiers to 
automatically detect misinformation.

## Dataset
**WELFake** is a dataset of 72,134 news articles (35,028 real, 37,106 fake) 
sourced from four popular datasets — Kaggle, McIntire, Reuters, and 
BuzzFeed Political — merged to improve generalization and reduce overfitting.

| Column | Description |
|--------|-------------|
| index  | Row identifier |
| title  | Article headline |
| text   | Full article body |
| label  | 0 = Real, 1 = Fake |

The dataset is stored in this repo via Git LFS. You will need 
Git LFS installed to download it:
```bash
git lfs install
git lfs pull
```

## Repo Structure

```
fake_news_case_study/
├── DATA/
│   ├── WELFake_Dataset.csv   # Full dataset
│   └── Data Appendix.pdf     # Dataset documentation
├── SCRIPTS/
│   ├── EDA.ipynb             # Exploratory data analysis
│   └── Modeling.ipynb        # Clustering and classification
├── OUTPUT/                   # Generated visualizations
├── hook/                     # Hook document (PDF)
├── rubric/                   # Rubric (PDF)
├── references/               # Reference materials
├── requirements.txt          # Python dependencies
└── README.md
```

## Setup Instructions

**1. Clone the repo**
```bash
git clone https://github.com/thomaswarren3/fake_news_case_study.git
cd fake_news_case_study
```

**2. Pull the dataset via Git LFS**
```bash
git lfs install
git lfs pull
```

**3. Create and activate a virtual environment**
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac/Linux
python -m venv venv
source venv/bin/activate
```

**4. Install dependencies**
```bash
pip install -r requirements.txt
```

**5. Run the notebooks**

Open `SCRIPTS/EDA.ipynb` first, then `SCRIPTS/Modeling.ipynb` in 
Jupyter or VS Code. Run all cells top to bottom.

## Case Study Materials
- See `hook/hook.pdf` to understand the mission
- See `rubric/rubric.pdf` for the full deliverable specifications
- See `references/` for suggested reading before you begin

## Original Dataset
WELFake on Kaggle: https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification