

- **GitHub**: https://github.com/xiankangW-gi/A-Simple-Framework-for-News-Policy-Text-Analysis
- **Stars**: ⭐ 47 (last checked: 2026-02-16)

A lightweight, China-focused Python toolkit for collecting and processing **news** and **policy** text data, with optional utilities for lexicon expansion and baseline modeling.

## Key Features
- **Google News scraping (monthly)** → CSV (title/source/date/snippet/URL)
- **Full-text extraction** from news pages via **GNE (GeneralNewsExtractor)**
  - Includes an **async high-throughput** extractor
- **Policy library crawling** (e.g., State Council policy pages) → local text corpus
- **Chinese preprocessing**: tokenization + stopword removal
  - **HanLP** pipeline option
  - **jieba + custom dictionary** option
- **Optional**: domain lexicon expansion using **Word2Vec**
- **Optional**: baseline classification on embedding features (e.g., XGBoost)

## Repository Entry Points
- `monthlynews.py` — scrape Google News by month → CSV
- `news_full_text_high_performance.py` — async crawling + GNE extraction → `.txt`
- `newsfulltext.py` / `full_news.py` — alternative extraction workflows
- `main.py` / `energy_policy_full_text_final.py` — policy list retrieval + full-text crawling
- `policy_text_preprocessing.py` — HanLP-based preprocessing
- `cut_with_dic_use_jieba.py` — jieba tokenization with custom dictionary (`词库最终.txt`)
- `word2vec_train.py` / `word2vec_test.py` — Word2Vec train/test for lexicon expansion
- `train_xgboost.py` — baseline modeling (embeddings-as-features)

## Notes
- Several scripts use **hard-coded Windows paths**; update paths before running.
- Web scraping robustness may require throttling and retries depending on target sites.