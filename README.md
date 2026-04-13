# 🎬 Netflix Show Recommendation Model — Collaborative Filtering in Excel

## Project Overview
A recommendation model built entirely in Microsoft Excel that predicts
what a new Netflix subscriber will enjoy — based on the viewing habits
of similar subscribers. No code required. Pure data logic using
Pearson correlation, replicating the core algorithm behind Netflix's
real recommendation engine.

**Tool:** Microsoft Excel  
**Dataset:** 1,000 Netflix subscribers · 9 shows · synthetic viewing data  
**Author:** Neel Shah | [LinkedIn](https://linkedin.com/in/neel-shah-654a1b27b)

---

## 🧠 How the Model Works

Collaborative filtering works by finding subscribers who watch similar
shows to a new user — then recommending what those similar users
enjoyed that the new user hasn't seen yet.
Step 1 → Build a viewer-show matrix (1,000 rows × 9 columns)
Step 2 → Calculate Pearson correlation between every pair of subscribers
Step 3 → For a new user, find the top N most similar viewers
Step 4 → Recommend shows those similar viewers rated highly
Step 5 → Rank recommendations by predicted rating score

---

## 📊 What Is Pearson Correlation?

Pearson correlation (r) measures how similarly two subscribers rate shows:
- r = +1.0 → Perfect agreement (watch the same things)
- r = 0.0  → No relationship
- r = -1.0 → Opposite tastes

In Excel: `=CORREL(subscriber_A_ratings, subscriber_B_ratings)`

<img width="1103" height="255" alt="Screenshot 2026-04-13 102328" src="https://github.com/user-attachments/assets/35fa4cc8-8a3b-4cb6-8dae-ca2725ddc914" />


---

## 🔍 Key Finding

> The correlation matrix discovered **genre clusters without genre labels**.
> Subscribers who liked Sci-Fi shows clustered together naturally.
> Subscribers who liked Crime/Thriller shows formed a separate cluster.
> The algorithm found patterns the data never explicitly stated.

---

## 📁 Files in This Repository
 netflix_recommendation_model.xlsx  # Full model with correlation matrix
├── netflix_portfolio.html             # Portfolio webpage (dark theme)
└── README.md

---

<img width="899" height="237" alt="Screenshot 2026-04-13 102349" src="https://github.com/user-attachments/assets/1576809b-423f-40c8-8526-7bc37d220b7e" />

<img width="801" height="615" alt="Screenshot 2026-04-13 102424" src="https://github.com/user-attachments/assets/3da7ac98-1ad8-4937-90ec-39767f5b20c5" />

<img width="408" height="515" alt="Screenshot 2026-04-13 102519" src="https://github.com/user-attachments/assets/543c4a17-5951-49ff-8c78-d0f03761201d" />

<img width="504" height="311" alt="Screenshot 2026-04-13 102536" src="https://github.com/user-attachments/assets/67d27fb8-d938-4f14-b40a-031cb78affa5" />


## 🚀 How to Use
1. Open `netflix_recommendation_model.xlsx`
2. Navigate to the **Correlation Matrix** sheet
3. Enter a new subscriber's viewing history in the input row
4. The model automatically calculates similarity scores
5. Recommended shows appear ranked by predicted rating

---

## 💼 Why This Project Matters
Netflix's real recommendation engine uses a more complex version of
exactly this logic — matrix factorisation and collaborative filtering.
Building it from scratch in Excel proves you understand the underlying
statistical principle, not just a library that does it for you.
