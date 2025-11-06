# 🧠 Fake News Detection System with Source Tracking

Welcome to the **Fake News Detection System** — an AI-powered web application built using **Streamlit**, **Machine Learning**, and **Graph Neural Network (GCN)** concepts.  
This project analyzes and visualizes the spread of misinformation across platforms like **Twitter** and **Reddit**, while comparing it with verified data from **GNews**.

🔗 **Live Demo:** [Fake News Detection App](https://savouriest-roxanne-botryose.ngrok-free.dev/)

---

## 🚀 Features

### 📰 Real or Fake News Classification
- Accepts any news text from the user.
- Uses **TF-IDF** and **Cosine Similarity** to compare input with verified **GNews** articles.
- Classifies input as:
  - ✅ **Real News** (similarity ≥ 70%)
  - ❌ **Fake News** (similarity < 70%)
- Displays confidence percentage and visual progress bar.

---

### 🌐 Multi-Platform Data Integration
- Fetches and analyzes news from:
  - 🐦 **Twitter**
  - 👽 **Reddit**
  - 📰 **Google News (GNews API)**
- Combines posts, authors, and metadata into a unified dataset.

---

### 📊 Fake News Ratio Visualization
- Calculates each user’s **Fake News Ratio** (fraction of fake posts per author).
- Displays:
  - 📈 Bar chart showing top fake-news spreaders.
  - 📊 Histogram of fake-news posting activity.
- Highlights **Top 10 users** spreading fake news, along with their **platforms and post URLs**.

---

### 🕸️ Network Graph Visualization
- Constructs a **Graph Network** using `NetworkX`.
- Nodes = posts; edges = textual similarity above 0.5.
- Fake posts appear in **red**, real posts in **blue** — illustrating clusters of misinformation.
- Helps visualize how fake news spreads across similar content.

---

### 🔗 Source Tracking
- Provides direct URLs for **Twitter** and **Reddit** posts.
- Enables transparency and traceability of misinformation sources.

---

## 🧩 Tech Stack

| Category | Technologies Used |
|-----------|------------------|
| **Frontend / UI** | Streamlit |
| **Backend / ML** | Python, Scikit-learn, NumPy, pandas |
| **Visualization** | Matplotlib, Seaborn, NetworkX |
| **Text Analysis** | TF-IDF Vectorizer, Cosine Similarity |
| **Graph Analysis (GCN Concept)** | PyTorch Geometric |
| **APIs** | GNews API, Twitter API, Reddit API |

---

## ⚙️ How It Works

1. **Input:** User enters a news headline or article.
2. **TF-IDF Processing:** Converts input and verified sources into vectorized features.
3. **Cosine Similarity:** Measures similarity between input and real GNews data.
4. **Classification:** Displays similarity score and classifies news as real or fake.
5. **Visualization:**
   - Fake-news ratio per author.
   - Network graph showing connections between similar posts.
6. **Source Tracking:** Displays original post URLs for transparency.

---
## 🤝 Contribution

### 1. Fork the Repository
- Go to the GitHub page of this project:  
  [https://github.com/kuheli31/Fake-News-Detector](https://github.com/kuheli31/Fake-News-Detector)  
- Click on the **Fork** button (top-right corner). This will create a copy of the repository under your GitHub account.

### 2. Clone Your Fork
- Open GitHub Desktop, Git Bash, or your preferred Git client.
- Clone your forked repository to your local computer. For Git Bash, run:
```bash
git clone https://github.com/<your-username>/Fake-News-Detector.git
```

### 3. Create a New Branch
- Always make changes in a new branch instead of main.
- Name the branch with your name or feature, for example:
```bash
git checkout -b kuheli-branch
```

### 4. Make Your Changes
- Open the file `Fake_News_Detection.ipynb` in **Google Colab**.  
- Make your improvements, such as:
  - Adding new features
  - Fixing bugs
  - Improving documentation or examples
  - Enhancing visualizations or outputs
- After making your changes, **save the notebook** in Google Colab.  
- Then, save a **copy back to this GitHub repository** folder directly from Google Colab:
  1. Click on **File → Save a copy in GitHub**.
  2. Choose your forked repository and the branch you created (e.g., `kuheli-branch`).
  3. Add a **descriptive commit message** about your changes.
  4. Click **OK** to push the changes to your GitHub fork.
  
### 5. Commit Your Changes (If using Git locally)
- Commit your changes with a clear message explaining what you did:
```bash
git add .
git commit -m "Added feature X / Fixed issue Y / Updated README"
```

### 6. Push Your Branch to GitHub
```bash
git push origin kuheli-branch
```

### 7. Create a Pull Request in Github website
- Go to your forked repository on GitHub.
- Click Compare & pull request.
- Add a descriptive title and explain your changes in detail.
- Submit the pull request. Your changes will be reviewed and merged.

---

## ⚖️ License & Copyright

© 2025 [Kuheli Bera](https://github.com/kuheli31). All rights reserved.  

This repository and its contents are protected under copyright law.  
You are free to **use and study** the code for **personal or educational purposes** only.  
**Redistribution or commercial use without explicit permission is prohibited.**


