
# Gen-AI Smart Calculator

An AI-powered smart calculator that interprets natural-language mathematical queries and returns accurate results with optional step-by-step explanations.

This project demonstrates how large language models can be combined with deterministic calculation logic to build reliable, user-friendly AI applications.

---

## Overview

Traditional calculators require rigid input formats.  
The Gen-AI Smart Calculator allows users to ask questions naturally, such as:

- “What is 15% of 240?”
- “Add 12 × 8 and then subtract 10”
- “Convert 5 kilometers to miles”

The system uses AI to understand intent and structure, while delegating all actual calculations to a controlled computation layer to ensure correctness.

---

## Key Features

- Natural language math query handling
- Supports arithmetic, percentages, and basic algebra
- Optional step-by-step explanations
- Deterministic calculation engine (no hallucinated math)
- Extensible design for additional domains (units, finance, formulas)

---

## High-Level Architecture

```

User Input
↓
AI Intent Parsing (LLM)
↓
Structured Math Expression
↓
Deterministic Calculation Engine
↓
Result + Explanation

```

**Important principle:**  
AI interprets intent — it does **not** perform the final calculation.

---

## Technology Stack

- **Frontend:** Node.js (or Web UI, if applicable)
- **Backend:** Python
- **AI Models:** Generative AI APIs (e.g., Gemini / OpenAI)
- **Computation:** Custom calculation logic (non-AI)

The architecture ensures accuracy, explainability, and safety.

---

## Why This Design

- Prevents incorrect AI-generated math
- Makes outputs predictable and testable
- Keeps AI usage focused on understanding, not reasoning
- Suitable for production systems where correctness matters

---

## Example Usage

**Input:**
```

What’s 12 × 8 plus 50?

```

**Output:**
```

12 × 8 = 96
96 + 50 = 146

Final Answer: 146

````

---

## Setup (Example)

```bash
git clone https://github.com/vishnuvardhanburri/Ai-smart-calculater.git
cd Ai-smart-calculater
````
<img width="1470" height="956" alt="Screenshot 2026-02-03 at 6 34 29 PM" src="https://github.com/user-attachments/assets/1a60dccd-c5dd-4f74-81da-325ae485a237" />
<img width="1470" height="956" alt="Screenshot 2026-02-03 at 6 34 35 PM" src="https://github.com/user-attachments/assets/bd28977d-e603-40eb-9f74-fad1ef6fabbb" />



https://github.com/user-attachments/assets/fcfd66db-f826-4931-920d-c40436eb7539


(Adjust setup instructions based on your actual implementation.)

---

## Future Improvements

* Web-based UI
* Conversation memory
* Advanced math and formulas
* Unit and currency conversion
* API version for external integrations

---

## License

MIT License


