## 2025 MinneMUDAC 1st place Winner - Match Length Prediction & Sentiment Trends in Mentoring Programs
### Predictive Modeling, Topic Modeling, NLP Analysis, LLM Modeling, Survival Analysis

Our team acts as consultant for a US nonprofit mentoring organization in this project. Our analysis goal is to help the organization **utilize sentiment analysis through NLP and LLM to better understand match dynamics, identify potential risks early, and enhance the longevity and quality of mentoring relationships**. Our work received interest from the CEO of the organization, and he expressed interest in applying our findings and exploring further collaboration. If implemented, **this monitoring dashboard has the potential to strengthen mentor-mentee bonds and ultimately promote the well-being and long-term development of the children served.**\
This project predicts the **duration of mentoring matches** and the **closure reason** using features extracted from match call notes with LLMs. By combining **natural language processing**, **machine learning**, and **survival analysis**, we aim to enable real-time monitoring and early intervention in mentoring programs.

---

### Project Highlights

- **LLM-powered feature engineering** using OpenAI to extract features that fall in these 3 categories:
  - **Risk & Conflict** – Detect signs of interpersonal challenges or tension between mentors and mentees
  - **Engagement** – Tracks match support involvement between the organization and mentors/ mentees
  - **Relationship Quality** - Measures depth & positivity of the relationship between mentors and mentees
- **Supervised learning models** - (LightGBM, Random Forest) to predict match length (numeric prediction) and closure reason (multi-class classification)
- **Survival analysis** (Cox Proportional Hazards Model) to understand the magnitude and direction of how features affect closure risk
- **Real-time risk monitoring** - dashboard design for early intervention support

---

### Tools & Technologies

- Python (pandas, scikit-learn, LightGBM, Random Forest, lifelines)
- OpenAI API for embedding and semantic feature extraction
- Feature Importance for model interpretability

---

### Project Structure
```
match-length-prediction/
├── notebooks/            # Development notebooks for analysis & modeling
├── scripts/              # Python scripts for preprocessing, modeling
├── results/              # Visualizations, metrics, and outputs
└── README.md             # Project overview
```

### Key Results

- Match length prediction model achieved strong performance with an **average RMSE of 6.77 months**. (vs. baseline 19 months)
- CLosure reason classification model achieved up to **AUC 0.8** in classifying critical categories, such as safety concerns and incompatibility.
- The project lays the groundwork for a real-time **intervention monitoring system** that enables the organization to increase the number of success matches.

---

### Data & Privacy

Due to confidentiality concerns, original mentoring call transcripts are not shared

---

### Future Work

- Integrate real-time call monitoring with streaming NLP models
- Deploy risk scoring dashboard for program coordinators

---

### Authors

**Anshu Mehta, Chen Ju Wang, Olivia Boe, Pin-Shiuan Liang, Ya Chin Hsu**  
MS in Business Analytics Graduate Student | Carlson School of Management | University of Minnesota

