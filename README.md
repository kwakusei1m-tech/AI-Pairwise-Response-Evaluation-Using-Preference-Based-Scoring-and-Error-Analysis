# AI-Pairwise-Response-Evaluation-Using-Preference-Based-Scoring-and-Error-Analysis
This project evaluates AI-generated responses using side-by-side comparison. It identifies which response is better, why it is preferred, and what quality dimensions drive those decisions, with a focus on clarity, completeness, and reasoning quality.

# 🧠 AI Evaluation of Pairwise Responses Using Preference Dissection Dataset

## 📌 Overview
This project evaluates AI-generated responses using a **side-by-side (SxS) comparison framework**.

Each record contains:
- one query
- two competing AI responses

The goal is to determine:
- which response is better
- why it is better
- what drives preference decisions

---

## 🎯 Objectives
- Identify which of two responses is stronger  
- Understand what drives preference decisions  
- Detect recurring failure patterns in weaker responses  
- Evaluate consistency across response comparisons  

---

## 📊 Dataset
- Preference Dissection Dataset  
- Structure:
  - query  
  - response_1  
  - response_2  

---

## ⚙️ Methodology

### ✅ Evaluation Dimensions
Each response is scored on:
- Accuracy  
- Relevance  
- Completeness  
- Consistency  
- Clarity  
- Reasoning Quality  

---

### ✅ Side-by-Side Comparison
- Both responses rated independently  
- Preferred response selected:
  - response_1  
  - response_2  
  - tie  

---

### ✅ Error Analysis
Weaker responses tagged with:
- missing_key_step_or_omission  
- weaker_reasoning  

---

## 📈 Visual Analysis

### 📊 Preferred Response Distribution
visuals/pref_preferred_response_distribution.png

**Insight:**  
Tie outcomes dominate, indicating low differentiation between response pairs.

---

### 📊 Quality Dimension Gap
visuals/pref_dimension_gap_distribution.png

**Insight:**  
Clarity and completeness are the strongest drivers of preference decisions.

---

### ⚠️ Error Taxonomy
visuals/pref_weaker_response_error_taxonomy.png

**Insight:**  
Weaker responses fail due to missing steps and weaker reasoning, not incorrect answers.

---

### 🔍 Closest Cases Analysis
visuals/pref_top10_closest_cases_table.png

**Insight:**  
Many response pairs have very small score gaps, confirming weak differentiation.

---

## 💡 Key Findings

- ✅ Most responses are similar → high tie rate  
- ⚠️ Differentiation driven by clarity and completeness  
- ⚠️ Weak responses lack steps and reasoning  
- ✅ Accuracy and relevance are generally strong  

---

## 🧠 Key Insight

> The issue is not correctness, but differentiation — responses are often equally acceptable but not optimised.

---

## 🏢 Business Implications

- ⚠️ Low differentiation → weak ranking performance  
- ⚠️ Generic responses reduce user experience quality  
- ✅ Reliable correctness baseline  

---

## 🚀 Recommendations

- Improve response clarity  
- Improve completeness  
- Add step-by-step guidance  
- Reduce shallow reasoning  
- Enhance ranking discrimination  

---

## ⚠️ Challenges

- High tie rate reduces insight depth  
- Response similarity limits preference analysis  
- Scoring subjectivity  

---

## 🔧 Future Improvements

- Expand dataset  
- Add human preference comparison  
- Introduce inter-rater agreement  
- Enhance taxonomy  

---

## 🛠 Tools Used

- Python (pandas, numpy)  
- Matplotlib / Seaborn  
- Jupyter Notebook  

---

