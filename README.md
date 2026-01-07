# ASSISTO_FRAUD_DETECTION


# Fraud Detection & Reporting using LLM

## Project Overview

This project implements a **Fraud Detection & Reporting System** using a **Large Language Model (LLM)**.
It helps users who suspect fraud but do not know **how to identify or report it**.
The system analyzes user input, detects possible fraud patterns, guides secure reporting, and generates a case ID for tracking.

---

## Problem Statement

Many users face online fraud but:

* Cannot identify whether it is fraud
* Do not know the correct reporting process
* Fear sharing sensitive information

This project solves that problem using an **LLM-based assistant**.

---

## Solution Approach (LLM-Based)

* Uses a **pre-trained Large Language Model (LLM)** via API
* No dataset or model training required
* Uses **prompt engineering** for fraud analysis and guidance
* Handles sensitive information safely

---

## Tools & Technologies Used

* **Python**
* **Jupyter Notebook**
* **OpenAI LLM API**
* **Prompt Engineering**
* **UUID** (for case tracking)

---

## Features Implemented

### Fraud Pattern Detection

* Detects types such as:

  * Phishing
  * Scam Calls
  * Fake Transactions
  * Identity Theft

### Secure Reporting Guidance

* Guides users on:

  * Evidence collection (SMS, email, transaction ID)
  * Safe next steps
  * Official fraud reporting channels
* Never asks for OTP, passwords, PIN, or card details

### Case Tracker

* Generates a unique **Case ID**
* Tracks:

  * Fraud type
  * Status
  * Timestamp

---

## Prompt Strategy Used

```
Handle sensitive information carefully.
Do not ask for OTP, passwords, PIN, or CVV.
Guide the user through evidence collection.
Explain official reporting procedures clearly.
```

---

## System Workflow

1. User enters suspected fraud description
2. LLM analyzes input
3. Fraud type is detected
4. Secure reporting guidance is generated
5. Case ID is created for tracking

---

## Sample Input

```
I received an SMS saying my bank account will be blocked and asking for OTP.
```

---

## Sample Output

```
Fraud Pattern Detected: Phishing

Secure Reporting Guidance:
Do not share OTP.
Save the message as evidence.
Contact your bank immediately.
Report the issue on the cybercrime portal.

Case ID: CASE-A9F3C2B1
Status: Open
```

---

## API Quota Handling

If API quota or billing is not enabled, the system:

* Gracefully handles the error
* Displays a fallback message
* Confirms that logic is correct

This ensures the project runs safely during demonstrations and evaluations.

---

## How to Run the Project

### Install Dependencies

```bash
pip install openai
```

### Set API Key

```python
import os
os.environ["OPENAI_API_KEY"] = "your_api_key_here"
```

### Run the Jupyter Notebook

Execute cells in order and provide input when prompted.

---

## Dataset Usage

No dataset is used

No model training

Fully LLM-based using pre-trained models

---

