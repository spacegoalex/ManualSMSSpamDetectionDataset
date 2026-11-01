# Manual SMS Spam Detection Dataset

A manually curated, crowd-sourced dataset for Indonesian SMS spam classification and natural language processing benchmarks.

## Dataset Overview

This dataset was created to support research on lightweight SMS spam classification. Messages were manually collected from real-world communication channels (personal SMS and instant messaging exchanges) across peers, colleagues, and family networks, followed by manual labeling and text sanitization.

- **Primary Language:** Indonesian (Bahasa Indonesia) / Informal Slang (Bahasa Gaul)
- **Format:** CSV (`.csv`)
- **Encoding:** UTF-8

## Data Schema

The dataset file (`dataset.csv`) contains the following columns:

| Column Name | Data Type | Description | Values / Examples |
| :--- | :--- | :--- | :--- |
| `text` | string | Sanitized message content | `"Selamat anda mendapatkan hadiah..."` |
| `label` | string / int | Ground-truth class annotation | `spam` (1) or `ham` (0) |

> **Note on Data Sources:**  
> - **Spam:** Real unsolicited SMS promotional texts, phishing attempts, fraud lures, and unwanted broadcasts.  
> - **Ham (Normal):** Real-world benign messages sourced from personal communication (SMS and WhatsApp) to reflect conversational Indonesian sentence structures.
