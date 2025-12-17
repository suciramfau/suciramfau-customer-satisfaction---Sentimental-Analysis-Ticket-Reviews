# Customer Satisfaction & Sentiment Analysis  
**Ticket System Review Analysis**

##  Project Overview
This project analyzes customer satisfaction and sentiment from **ticket system reviews** to evaluate service quality, user experience, and customer loyalty.  
Key performance indicators such as **CSAT, CES, and NPS** are combined with **text-based sentiment analysis** to generate actionable business insights.

The analysis is supported by an interactive **Power BI dashboard** and a reproducible **Python notebook**.

---

##  Business Objectives
- Measure overall customer satisfaction and ease of use
- Identify strengths and weaknesses across ticket systems
- Detect recurring issues from negative customer feedback
- Provide strategic recommendations to improve service quality and NPS

---

##  Dataset
- **Source**: Ticket system reviews (Oct–Dec 2024)
- **Total records**: 1,462 tickets
- **Survey response rate**:  
  - Responded: 787 (54%)  
  - Not responded: 675 (46%)

### Key Features
- `id_survey`
- `date_of_survey`
- `ticket_system`
- `overall_rating`
- `customer_service`
- `features`
- `value_for_money`
- `ease_of_use`
- `likelihood_to_recommend`
- `overall_text` (review text)

---

## 🧮 Metrics & Formulas
- **CSAT (%)**  
  \[
  \text{CSAT} = \frac{\sum rating}{(\text{count of respondents} \times 5)} \times 100
  \]

- **CES (%)**  
  \[
  \text{CES} = \frac{\text{average ease\_of\_use}}{5} \times 100
  \]

- **NPS**  
  \[
  \text{NPS} = \%Promoters (9–10) - \%Detractors (0–6)
  \]

- **Sentiment Analysis**  
  Lexicon-based sentiment classification (positive vs negative), with potential extension to:
  - TF-IDF + Logistic Regression
  - Transformer-based models

---

## 🛠️ Tools & Technologies
- **Python** (Google Colab)
  - pandas, numpy
  - matplotlib, seaborn
  - nltk / VADER (sentiment)
- **Power BI**
  - KPI dashboard (CSAT, CES, NPS)
  - Vendor comparison
  - Time-series trend analysis

---

## 🔍 Analysis Workflow
1. **Data Cleaning & Preprocessing**
   - Filter valid survey responses
   - Handle missing values
   - Normalize rating scales
   - Standardize ticket system categories

2. **KPI Calculation**
   - CSAT, CES, NPS at overall and vendor level
   - Time-based trend analysis

3. **Sentiment Analysis**
   - Text preprocessing (lowercase, stopwords, lemmatization)
   - Positive vs negative word frequency
   - Word cloud visualization

4. **Visualization**
   - Interactive Power BI dashboard
   - Summary insights for stakeholders

---

## Key Insights
- Overall satisfaction is **very high** (CSAT 91.2%, CES 89.5%)
- **Customer Service** scores lowest (67.3%) → primary improvement area
- NPS (12%) indicates a moderate number of detractors
- Positive reviews emphasize *ease of use* and *support*
- Negative reviews frequently mention *service speed*, *reporting*, and *UX friction*

---

## Strategic Recommendations
- Improve customer service response time and resolution quality
- Optimize ticket workflow and self-service features
- Implement close-the-loop program for detractors
- Monitor KPIs continuously via operational dashboards
- Apply A/B testing to UX and process improvements

---

## Repository Structure



---

## Deliverables
- Python notebook (.ipynb)
- Power BI dashboard
- Presentation slides (optional)
- Project summary (Notion)

---
