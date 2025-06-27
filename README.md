# Personalized Study Plan Recommender 🎓📊

This machine learning project predicts which subjects a student should focus on next, based on their performance in past courses and assessments. It uses an XGBoost model to rank subject recommendations tailored to individual learning progress.

Ideal for adaptive learning platforms, academic advising systems, or self-paced study assistants.

---

## 🧠 Project Goals

- Analyze historical academic performance
- Recommend subjects with the highest impact on mastery
- Personalize study paths based on student-level data

---

## 🧾 Key Features

- 🔢 **Inputs:** Prior grades, quiz results, and assessment scores
- 📈 **Ranking Model:** Uses XGBoost with ranking objective (`rank:pairwise`)
- 🧮 **Predictive Output:** Ranked list of subjects to study next
- 🔁 **Adaptivity:** Can be re-evaluated after each new assessment

---

## 📂 Files Included

| File Name                    | Description                                      |
|-----------------------------|--------------------------------------------------|
| `Study Plan XGboost.ipynb`   | Full pipeline including preprocessing, training, evaluation, and testing |

---

## ⚙️ Technologies Used

- Python
- XGBoost
- Pandas, NumPy
- Scikit-learn
- Jupyter Notebook
- (Optional) Firebase / GCP integration

---

## 🚀 How It Works

1. Input student performance data (e.g., CSV or Firestore)
2. Transform the dataset into (student, subject) pairs with features like:
   - Previous grade in prerequisites
   - Mastery level or quiz score
   - Subject popularity (optional)
3. Train XGBoost model on ranking objective
4. Generate ranked list of subjects per student

---

## 📌 Example Use Case

> A student has completed “Math I” and “Intro to Programming.” Based on their performance, the model recommends focusing next on “Data Structures” and “Discrete Math” before attempting “Algorithms.”

---

## 🧪 Evaluation

- Metrics used: NDCG, MAP, and manual verification
- Supports cross-validation for stable training
- Easily extendable to include time-series or text features

---

## ✅ Future Enhancements

- Integration with live student dashboard (via Firebase or MAUI)
- Real-time updates after each assessment submission
- Add feedback loop to learn from student outcomes

---

## 📜 License

MIT License — free to use with attribution.

---

## 🤝 Contact

Created by [Ali Gaber](https://linkedin.com/in/ali-gaber-277663316).  
For questions or feedback, feel free to [open an issue](https://github.com/Aligaber24/study-code-ai/issues) or reach out.

