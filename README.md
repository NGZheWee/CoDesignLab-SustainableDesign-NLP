# NLP-Driven Sustainable Design

This repository contains my research artifacts for **NLP-driven sustainable design** work conducted through the **Berkeley Engineering Design Scholars Program** and the **Co-Design Lab** at UC Berkeley. The project studies how customer reviews, product certifications, and natural-language processing can reveal design opportunities for more sustainable consumer products.

The work contributed to the ASME IDETC-CIE 2025 paper **"Data-Driven Sustainable Design Opportunities from Automated User Insights"**. Official project context is available through my [Design Scholars cohort profile](https://jacobsinstitute.berkeley.edu/news/meet-the-2024-berkeley-engineering-design-scholars/), my [Co-Design Lab profile](https://codesign.berkeley.edu/team/derrick-ng/), and the [Co-Design Lab paper page](https://codesign.berkeley.edu/papers/goridkov-reviews-idetc/).

## Contents

- **Summer 2024 (Engineering Design Scholar Program)**: Initial Amazon product and review scraping pipelines, early ABSA experiments, VADER/BERT sentiment analysis, topic modeling, sustainability keyword dictionaries, and the final program poster.
- **Fall 2024**: Expanded data-processing workflows, product-feature and affordance extraction, GPT-assisted sentiment and topic modeling, merged product-review datasets, and intermediate analysis outputs.
- **Spring 2025**: IDETC-focused analysis scripts, certification/product/affordance correlation workflows, ABSA trend plots, and final mini-database generation scripts.

## Research Scope

- Built a review-analysis pipeline for **23,000+ Amazon customer reviews** across **290 sustainability-certified products**.
- Studied consumer perception of sustainability certifications, product affordances, product features, and sustainability-related review language.
- Connected customer-review signals with sustainable-design opportunity generation using ABSA, topic modeling, correlation analysis, and LLM-assisted synthesis.

## Methods and Tools

- **Data collection**: DrissionPage, Selenium, BeautifulSoup, selector-based scraping, and structured CSV workflows.
- **Text processing**: Cleaning, tokenization, keyword dictionaries, review filtering, and product/category normalization.
- **Sentiment analysis**: VADER, BERT-based sentiment classification, and GPT-assisted sentiment scoring.
- **Topic modeling**: LDA, NMF, BERTopic, and GPT-assisted topic summarization.
- **Design synthesis**: Product-feature extraction, affordance extraction, certification mapping, correlation matrices, and trend visualization.

## Key Outputs

- A structured dataset linking sustainability certifications, product metadata, product reviews, sentiment scores, affordance labels, and topic-modeling outputs.
- Comparative analyses of customer-facing sustainability concerns such as packaging, durability, material perception, quality, and energy use.
- Publication materials for **ASME IDETC-CIE 2025**, including the paper:

  Goridkov, N., Ng, Z. W., & Goucher-Lambert, K. (2025). *Data-Driven Sustainable Design Opportunities from Automated User Insights*. Proceedings of the ASME 2025 International Design Engineering Technical Conferences and Computers and Information in Engineering Conference, IDETC2025-169019.

## How to Navigate

- Start with `Summer 2024 (Engineering Design Scholar Program)/` for the original research pipeline and poster.
- Use `Fall 2024/Programs/` for the expanded scraping, filtering, GPT analysis, ABSA, product-description analysis, and topic-modeling scripts.
- Use `Fall 2024/Databases/` for intermediate and final structured datasets from the Fall 2024 phase.
- Use `Spring 2025/Programs_IDETC/` for the final IDETC-focused scripts and trend analyses.

## Reproducibility Notes

This repository preserves the research workflow and intermediate artifacts, but it is not a one-command production package. Many scripts were developed as research notebooks or local pipeline stages and may require path updates before rerunning.

To rerun GPT-assisted steps, create local environment variables instead of placing keys in source files:

```powershell
$env:OPENAI_API_KEY = "your-key"
$env:OPENAI_ORG_ID = "optional-org-id"
$env:OPENAI_PROJECT_ID = "optional-project-id"
```

Install the approximate Python dependencies with:

```powershell
pip install -r requirements.txt
```

## Data and Ethics Note

The repository contains research artifacts derived from public product and review data. Use the data responsibly, respect source-platform terms, and avoid treating automated sentiment or LLM outputs as ground truth without validation.

## Academic Integrity Note

This repository contains my own research code, data-processing artifacts, and publication-related materials, shared for portfolio and research transparency. Do not copy this work for active or future coursework, and follow your institution's academic integrity policies.
