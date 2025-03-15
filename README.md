# Drug-Recommendation-Project

## 📌 Overview  
This project aims to build a **data-driven drug recommendation system** using **collaborative filtering, autoencoders, and SVD**. It helps users find **safe and effective over-the-counter (OTC) medications**, considering **drug interactions and review-based effectiveness**.  

## 💡 Problem Statement  
- Searching for OTC drugs online lacks **clarity and accuracy**.  
- Existing sources **miss drug interactions** and **rely on unreliable ratings**.  
- Many similar projects lack **public datasets** or are hidden behind paywalls.  

## 📊 Data Sources  
| **Dataset**           | **Description**                                         |  
|----------------------|-----------------------------------------------------|  
| **Stanford BioSNAP** | 5.5M+ drug-drug interaction samples.                  |  
| **DrugBank**        | Drug ID, names, and synonyms.                          |  
| **UCI Drug Review** | 23K+ drug-condition-review combinations.                |  

## 🛠 Methodology  
### **1️⃣ ALS (Alternating Least Squares)**  
- Treats conditions as **rows** and drugs as **columns**.  
- Uses **weighted ratings** for better reliability.  
- Captures **hidden patterns** for improved recommendations.  

### **2️⃣ Autoencoder-Based RecSys**  
- **Neural Network-based** dimensionality reduction for user-item interactions.  
- 7-layer model with **ReLU activation** and a **learning rate of 0.001**.  
- **t-SNE visualization** for latent space representation.  

### **3️⃣ Collaborative Filtering with SVD**  
- **Singular Value Decomposition (SVD)** on drug-condition data.  
- Captures **95% variance** using only **5 components**.  
- Ensures **safe recommendations** by identifying **negative drug interactions**.  

## 🎯 Key Outcomes  
✅ **More reliable drug recommendations** than traditional search engines.  
✅ **Identifies harmful drug interactions** to ensure safety.  
✅ **Useful for both general users and healthcare professionals.**  

## 📈 Results  
- Successfully **recommended drugs for Pneumonia** with strong validation.  
- **MSE of 0.184** for Autoencoder-based recommendations.  
- **SVD captured 95% variance**, ensuring high accuracy.  


