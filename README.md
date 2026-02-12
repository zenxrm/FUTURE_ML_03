# FUTURE_ML_03  
## Resume Screening & Job Matching System (NLP Based)

## Internship Task – Machine Learning Track

This project was completed as part of Machine Learning Internship (Task 03).

The objective was to build a Resume / Job Screening system that:

- Matches job descriptions with relevant roles
- Computes similarity scores
- Ranks candidates/jobs
- Identifies missing skills
- Provides explainable decision support

This simulates how real HR-tech recruitment platforms operate.

---

#  Problem Statement

Recruiters receive thousands of applications for job openings.  
Manual screening is:

- Time consuming
- Inconsistent
- Error prone

This system automates role matching using Natural Language Processing (NLP).

---

#  Dataset Information

Dataset Used: Job Descriptions Dataset (Kaggle)
dataset link:  https://www.kaggle.com/datasets/ravindrasinghrana/job-description-dataset

Total Records Used (after cleaning & sampling): ~50,000

Columns Used:

- Job Title
- Job Description
- Skills
- Responsibilities

Duplicates and null values were removed before analysis.

---

#  Methodology

## 1️ Text Preprocessing

- Lowercasing
- Special character removal
- Stopword removal using NLTK
- Text normalization

## 2️ Feature Engineering

TF-IDF Vectorization:

- max_features = 10000
- ngram_range = (1,2)
- min_df = 5

This converts textual job descriptions into numerical vectors.

## 3️ Similarity Matching

Cosine Similarity was used to:

- Compare recruiter-provided job description
- Rank jobs based on similarity score

Higher similarity score = better role match.

## 4️ Skill Gap Detection

- Extracted skill tokens from recruiter input
- Compared against job skill sets
- Identified missing skills

---

#  Results

Input Given : Seeking a Data Scientist with expertise in Python, Pandas, NumPy, machine learning, SQL, statistics, model evaluation, and data visualization. Experience with scikit-learn and cloud deployment is preferred.

###  Similarity Score Distribution

<img width="927" height="505" alt="Screenshot 2026-02-12 190205" src="https://github.com/user-attachments/assets/5adef525-ebed-4e44-9277-1085924fcc15" />


Most unrelated jobs show low similarity, while relevant roles show higher similarity scores.

---

###  Top 10 Matching Job Roles
<img width="1000" height="567" alt="Screenshot 2026-02-12 190210" src="https://github.com/user-attachments/assets/0bb315cb-2d3a-4672-8c81-8111fb33f23e" />


The system successfully ranks the most relevant job roles based on recruiter input.

---

###  Skill Gap Identification

The system highlights missing skills between:
<img width="730" height="204" alt="Screenshot 2026-02-12 190215" src="https://github.com/user-attachments/assets/12ed343c-f2ef-41c2-9794-f6023ee082c7" />

- Required role description
- Existing job skill sets

This provides explainable insights for recruiters.

---

#  Exported Results

<img width="951" height="288" alt="Screenshot 2026-02-12 190222" src="https://github.com/user-attachments/assets/181f99c5-b27d-42d8-8e36-9b6a302cedf4" />

This allows further analysis or integration into recruitment workflows.

---

#  Business Impact

This system can:

- Reduce manual screening workload
- Automate role matching
- Improve recruitment efficiency
- Provide transparent ranking logic
- Identify skill gaps instantly

---

#  Technologies Used

- Python
- Pandas
- Scikit-learn
- TF-IDF
- Cosine Similarity
- NLTK
- Matplotlib
- Seaborn

---

#  Conclusion

This project demonstrates:

- Real-world NLP preprocessing
- Text vectorization using TF-IDF
- Similarity-based ranking logic
- Skill gap detection
- Decision-support ML system implementation

---

# 👨‍💻 Author

Raghav Marwaha  
Machine Learning Intern  
Future Interns  

---
