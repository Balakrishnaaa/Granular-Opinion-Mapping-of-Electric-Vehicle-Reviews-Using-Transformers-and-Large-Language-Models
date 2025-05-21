# Granular Opinion Mapping of Electric Vehicle Reviews

## Project Overview

This project, completed as part of the DATA 606 Capstone in Data Science, aims to analyze electric vehicle (EV) reviews to extract public sentiment towards specific aspects such as battery life, charging, comfort, price, and performance. Using large language models (LLMs) and transformer-based sentiment analysis, we developed a pipeline to generate, process, and visualize insights from EV-related review data.

## Team Members
- Satvik Reddy Singi Reddy  
- Bala Krishna Reddy Chinna  
- Manasa Jagati

## Objectives

- Understand public sentiment about various aspects of electric vehicles.
- Automatically extract and classify review aspects (e.g., battery, range, price).
- Generate actionable insights to assist EV manufacturers and policymakers.
- Present results through interactive data visualizations and a user-friendly dashboard.

## Dataset

Due to the absence of a comprehensive publicly available dataset, we used **synthetically generated EV reviews** via OpenAI’s GPT-4 model. Reviews were crafted using domain-specific prompts to simulate realistic and balanced customer feedback.

### Data Generation

- **Model Used:** GPT-4 (via LangChain)
- **Design:** Custom prompts ensuring coverage of key EV features.
- **Balance:** Reviews include a mix of positive, negative, and neutral sentiments.

## Methodology

1. **Aspect Extraction** – Key features were identified from each review using transformer models.
2. **Sentiment Classification** – Each aspect was classified using `distilbert-base-uncased-finetuned-sst-2-english` from Hugging Face.
3. **Explanation Generation** – Summaries were generated per review to describe sentiment findings.
4. **Visualization** – Streamlit dashboard integrated with Altair and Plotly for interactive charts.

## Tools & Technologies

- **Language Models:** OpenAI GPT-4, Hugging Face Transformers
- **Sentiment Model:** DistilBERT (SST-2 fine-tuned)
- **Data Pipeline:** LangChain
- **Visualization:** Streamlit, Altair, Plotly

## Results

- **Battery Life** and **Comfort** showed predominantly positive sentiments.
- **Charging Infrastructure** and **Range** received mixed reviews.
- **Price** was polarizing — both praised and criticized.
- Trends indicated fluctuating customer sentiment depending on aspect.

## Challenges

- No static, publicly available EV review dataset.
- Maintaining authenticity in synthetic reviews.
- Sentiment misclassification in nuanced or ambiguous contexts.

## Future Work

- Fine-tune sentiment analysis models for better handling of mixed sentiments.
- Incorporate real-world reviews from multiple platforms.
- Develop "EV Insight Pro" – a product offering real-time sentiment dashboards for industry use.

## Conclusion

Aspect-based sentiment analysis using LLMs offers a powerful approach for extracting deep insights from unstructured customer feedback. This project demonstrates how modern NLP tools can support data-driven decision-making in the EV industry.

---

