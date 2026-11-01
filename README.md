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

## Anonymization & Ethical Considerations

To protect user privacy, all messages have undergone anonymization:
- Phone numbers replaced with `[PHONE]`
- URLs and suspicious links masked with `[URL]`
- Personal names, account numbers, and OTP codes scrubbed or generalized
- No metadata (sender/receiver IDs, timestamps, or device identifiers) is retained.

## Citation

If you use this dataset in your research or paper, please cite it as follows:

```bibtex
@misc{manual_sms_spam_dataset_2026,
  author       = {Siemen Gunawan Iksan},
  title        = {Manual SMS Spam Detection Dataset},
  year         = {2026},
  publisher    = {GitHub},
  journal      = {GitHub repository},
  howpublished = {\url{[https://github.com/spacegoalex/ManualSMSSpamDetectionDataset](https://github.com/spacegoalex/ManualSMSSpamDetectionDataset)}}
}
