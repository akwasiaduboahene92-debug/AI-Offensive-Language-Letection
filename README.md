# AI-Offensive-Language-Detection
NLP + Machine Learning Model for Detecting and Analysing Offensive Content on X

 Overview
This project demonstrates how **AI and Natural Language Processing (NLP)** can automatically detect, classify, and visualize offensive or abusive language on social media platforms.  
It uses a transformer-based model to analyze real tweets collected via the **Twitter API v2**, identifying patterns of online toxicity and social discourse.

This prototype forms an early step toward understanding how AI moderation tools detect harmful content online.

 ⚙️ Pipeline Overview

1. **Tweet Collection:**
   - Real-time data using Tweepy and the Twitter API v2 (Recent Search)
2. **Data Cleaning:**  
   - Removes URLs, hashtags, emojis, mentions, and duplicates
3. **Classification:**  
   - Uses `cardiffnlp/twitter-roberta-base-offensive` to score each tweet as *Offensive* or *Non-Offensive*
4. **Clustering & Topic Modelling:**  
   - TF-IDF + KMeans to group related topics  
   - LDA (Latent Dirichlet Allocation) to extract thematic patterns
5. **Visualization:**  
   - Offensive score distribution  
   - Cluster-based analysis  
   - Comparison between offensive and non-offensive tweets
6. **Ethics & Privacy:**  
   - Author IDs are anonymized  
   - No identifiable data stored in compliance with GDPR



 📂 Dataset

| File | Description |
| **twitter_cvawg_phase1_results.csv** | Processed dataset of tweets with offensive scores and clustering results |
| **requirements.txt** | Dependencies required to run the project |
| **README.md** | This documentation |
| *(optional)* **AI_Offensive_Language_Analysis.ipynb** | Google Colab notebook version |

---

## 🔬 Example Model Output

| Text Snippet | Offensive | Non-Offensive |

| “So many celeb D-bags need to be unemployed by AI.” | 0.38 | 0.61 |
| “AI is revolutionizing assistive technology for the blind.” | 0.11 | 0.89 |

---

## 📈 Next Steps

- Expand dataset with full-archive Twitter access (Academic API)
- Integrate Perspective API for toxicity calibration
- Compare accuracy across multiple transformer models
- Detect false positives and cultural bias in model predictions

---

## 🧩 Tech Stack

| Category | Tools |
|-----------|--------|
| Language | Python 3.10+ |
| Data Collection | Tweepy (Twitter API v2) |
| NLP | Hugging Face Transformers |
| ML & Analysis | Scikit-learn, Gensim |
| Visualization | Matplotlib, PyLDAVis |
| Storage | Pandas, CSV |

---

## 📎 Author

**Akwasi Adu-Boahene**  
🎓 Researcher in AI, Data Science & Digital Ethics  
📧 akwasiaduboahene92@gmail.com  

## 🪪 License

This project is released under the **MIT License** — for research and educational purposes only.  
Please cite appropriately if used in academic or ethical AI research.

---

## 🌍 Acknowledgements

- [Cardiff NLP Group](https://github.com/cardiffnlp) for the RoBERTa offensive model  
- [Hugging Face](https://huggingface.co) for open-source AI tooling  
- [Twitter API](https://developer.twitter.com/en/docs/twitter-api) for public data access

⭐ **If you find this project useful, please star it and follow for updates.**
