# Amazon Review Sentiment Analysis

## Overview
Temporal analysis of Amazon Electronics reviews across four time points (2008, 2013, 2018, 2023), examining shifts in sentiment, rating distribution, and review length over 15 years.

## Key Findings
- 5-star reviews increased from ~53% (2008) to ~62% (2023)
- 1-star reviews rose from ~11% to ~15% — indicating stronger polarization
- Review length remained relatively stable across years

## Methodology
- Loaded 500M+ reviews from [McAuley-Lab/Amazon-Reviews-2023](https://huggingface.co/datasets/McAuley-Lab/Amazon-Reviews-2023) via Hugging Face
- Applied **reservoir sampling** to create a balanced dataset of 100,000 reviews per year
- Analyzed sentiment polarity using **VADER**
- Visualized rating distributions and review length trends with Matplotlib and seaborn

## Tech Stack
- Python
- `vaderSentiment`, `datasets`, `pandas`, `matplotlib`, `seaborn`

## How to Run
1. Clone the repository
   ```bash
   git clone https://github.com/xiaoxuanzhang1/Amazon-Review-Sentiment-Analysis.git
   ```
2. Install dependencies
   ```bash
   pip install datasets vaderSentiment pandas matplotlib seaborn
   ```
3. Open and run the notebook
   ```bash
   jupyter notebook Project.ipynb
   ```

## Data
Data sourced from [Amazon Reviews 2023](https://huggingface.co/datasets/McAuley-Lab/Amazon-Reviews-2023). Raw data not included due to size.
