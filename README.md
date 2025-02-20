# Empowering Indonesian Internet Users: An Approach to Counter Online Toxicity and Enhance Digital Well-being

## Overview

This repository contains datasets, models, and code implementations related to our research on detecting and categorizing online toxicity in the Indonesian language using Natural Language Processing (NLP). Our study proposes a **3-stage methodology** for analyzing online toxicity:

1. **Type:** Identifying different types of toxicity.
2. **Target Audience:** Identifying the targeted audience of toxic comments.
3. **Topics:** Categorizing toxicity based on context and discussion topics.

We fine-tuned **IndoBERTweet** and **Indonesian RoBERTa** models for multilabel and multiclass classification tasks. Our findings show that IndoBERTweet consistently outperforms Indonesian RoBERTa across all three stages.

📄 Read the full paper: [Click Here!](https://doi.org/10.1016/j.iswa.2024.200394)

---

## Repository Structure

```
📂 dataset
 ├── online-toxicity-target-processed.csv
 ├── online-toxicity-target.csv
 ├── online-toxicity-type-processed.csv
 ├── online-toxicity-type.csv
 ├── targeted-online-toxicity-cat-processed.csv
 ├── targeted-online-toxicity-cat.csv

📂 model
 ├── 📂 Stage 1 (Type Classification)
 │   ├── Toxic_Type_*.ipynb (Experiments with IndoBERTweet & RoBERTa)
 │
 ├── 📂 Stage 2 (Target Classification)
 │   ├── Target_*.ipynb (Experiments with IndoBERTweet & RoBERTa)
 │
 ├── 📂 Stage 3 (Topic Classification)
 │   ├── TC_*.ipynb (Experiments with IndoBERTweet & RoBERTa)

📄 README.md

```

---

## Dataset

The datasets used in this research are provided in the **dataset/** directory. The datasets contain labeled Indonesian-language text for various toxicity classification tasks:

- **online-toxicity-type.csv**: Raw dataset for toxicity type classification.
- **online-toxicity-target.csv**: Raw dataset for identifying targeted audiences.
- **targeted-online-toxicity-cat.csv**: Raw dataset for toxicity topic classification.

We also provide processed versions of these datasets (with `-processed` suffix) for direct model training.

---

## Models

The **model/** directory contains Jupyter Notebooks for fine-tuning **IndoBERTweet** and **Indonesian RoBERTa** models. The experiments are divided into three stages:

### Stage 1: Toxicity Type Classification

- Fine-tuning models to classify different types of toxicity (e.g., hate speech, cyberbullying, offensive language, etc.).

### Stage 2: Targeted Audience Classification

- Training models to determine the target audience of toxic comments (e.g., individuals, groups, public figures, etc.).

### Stage 3: Topic Classification

- Categorizing toxicity based on topics (e.g., politics, religion, gender issues, etc.).

Each stage includes multiple notebooks with different hyperparameter settings, ensuring optimal model performance.

---

## Key Findings

✅ IndoBERTweet consistently outperforms Indonesian RoBERTa in all classification stages.
✅ The best IndoBERTweet models achieve higher **precision, recall, and F1-score** than RoBERTa.
✅ Our methodology is effective for **real-world toxicity detection**, including classifying unseen Indonesian-language content from Twitter/X.
✅ The results contribute to **automated moderation tools** for safer online communities.

---

## How to Use

### 1️⃣ Install Dependencies

```bash
pip install transformers datasets torch scikit-learn pandas

```

### 2️⃣ Load and Train a Model

Run any notebook from the `model/` directory to train a classification model.

### 3️⃣ Predict on New Data

Modify the inference cells in the notebook to classify new text samples.

---

## Citation

If you use this repository for your research, please cite our paper:

```
@article{yourpaper2024,
  title={Empowering Indonesian Internet Users: An Approach to Counter Online Toxicity and Enhance Digital Well-being},
  author={Andry Alamsyah, Yoga Sagama},
  journal={Information Sciences and Web Applications},
  year={2024},
  doi={10.1016/j.iswa.2024.200394}
}

```

---

## License

This repository is released under the **MIT License**. You are free to use and modify the code for research and development purposes.

---

## Contact

For questions or collaborations, feel free to reach out via:
📧 Email: [yogasagamaa@gmail.com](mailto:yogasagamaa@gmail.com)

🔗 LinkedIn: [Your LinkedIn](https://www.linkedin.com/in/yogasagama/)
