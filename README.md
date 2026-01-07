# GenAI Policy Co-Pilot for Cognitive Cities

**Status:** Early-stage research project, under active development (January 2026).

## Overview

LLM-powered decision-support system that combines air-quality forecasting with policy document retrieval to help urban policymakers evaluate environmental policy impacts.

**Use case:** A policymaker asks *"What if we expand the odd-even traffic rule to 7 days/week?"* → System forecasts PM10 impact, estimates congestion/fuel costs, and cites relevant regulations.

## Motivation

DKI Jakarta (10M+ residents) faces serious air pollution: PM2.5 peaks at 40–80 µg/m³ during dry seasons (WRI Indonesia, 2019–2021). Yet policymakers lack integrated tools to evaluate policy trade-offs. This project combines **forecasting** (hybrid RF–ARIMA) with **GenAI** (LLM + RAG) for transparent policy analysis.

## Project Architecture

- **Module 1:** Air-quality forecasting (PM10/PM2.5) using hybrid Random Forest–ARIMA with SHAP explainability
- **Module 2:** Urban mobility & economic impact estimator (traffic, congestion, fuel consumption)
- **Module 3:** LLM-based Q&A interface against policy documents (RAG pattern)

## Development Plan (2-Week Prototype)

| Week | Focus |
|------|-------|
| Week 1 (Jan 7–13) | Data pipeline setup, EDA notebooks, baseline ARIMA + RF models |
| Week 2 (Jan 14–20) | Hybrid RF–ARIMA integration, SHAP explainability, initial results |

**Future work:** LLM integration (RAG), policy documents, UI prototype (post-KAUST application)

## Tech Stack

- **ML:** Python, scikit-learn, statsmodels, SHAP
- **LLM:** OpenAI API / LangChain (RAG)
- **Data:** Pandas, NumPy
- **UI:** Streamlit (prototype)

## Repository Structure

```
├── README.md
├── LICENSE (MIT)
├── requirements.txt
├── notebooks/              # Jupyter experiments
├── src/                    # Core modules
│   ├── data_pipeline.py
│   ├── forecasting.py
│   ├── llm_interface.py
│   └── utils.py
├── data/                   # Raw & processed data
└── docs/                   # Architecture, methodology
```

## Quick Start

```bash
# Clone & install
git clone https://github.com/rafidhiyaulh/genai-policy-copilot-cognitive-cities.git
cd genai-policy-copilot-cognitive-cities
pip install -r requirements.txt

# Run notebooks for experiments
jupyter notebook notebooks/01_exploratory_data_analysis.ipynb
```

## License

MIT License – free to use, modify, and distribute for academic & commercial purposes.

## Contact

**Muhammad Rafi Dhiyaulhaq**  
Email: rafidhiyaulh@gmail.com | LinkedIn: [linkedin.com/in/rafidhiyaulh](https://linkedin.com/in/rafidhiyaulh) | GitHub: [github.com/rafidhiyaulh](https://github.com/rafidhiyaulh)
