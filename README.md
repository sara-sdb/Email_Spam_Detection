# Email Spam Detection Project

This project focuses on creating a smart email spam detection system that leverages both content analysis and sender domain verification. By integrating these two approaches, the system effectively filters unwanted messages and helps protect users from various email-borne threats.


## How the System Works

### Sender Domain Verification

- Every incoming email is checked against a list of suspicious domains.
- Emails sent from domains frequently linked to spam are flagged immediately, providing a strong initial filter.

### Content-Based Detection

- At the core is a **Naive Bayes Classifier**, known for its efficiency and effectiveness in text-based tasks.
- The model calculates the likelihood that an email text is spam by using a trained model on the given dataset.


## Development & Evaluation

- The classifier is trained on a labeled dataset containing examples of both spam and legitimate emails.
- Performance is evaluated using standard metrics: **accuracy**, **precision**, **recall**, and **F1-score** to ensure dependable real-world results.
- The system is designed for interpretability:  
  Users can review which features (domain or content cues) contributed to any given classification, supporting transparency and user trust.


## Goals

- Accurately identify and filter spam emails to improve inbox quality.
- Safeguard users from phishing, malware, and other cyber risks.
- Offer clear, understandable reasons for each spam decision.
- Maintain high efficiency and real-time operation.


## Technology Stack

The system is built in Python using the following libraries:

- **NumPy** and **Pandas** for data processing
- **Seaborn** for visualizations
- **Scikit-learn** for machine learning and evaluation
- **NLTK** for NLP tasks


## Setup

Install the necessary Python libraries with:

```bash
pip install numpy pandas nltk scikit-learn seaborn
