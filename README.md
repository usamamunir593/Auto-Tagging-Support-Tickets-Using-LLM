# 🏷️ Auto Tagging Support Tickets Using LLM

## 🎯 Objective

Automatically classify customer support tickets into categories using LLM-based techniques:
- **Zero-shot classification** - No training data needed
- **Few-shot learning** - Learn from few examples
- **Top 3 predictions** - Ranked tag probabilities

---

## 🔧 Methodology / Approach

### Dataset
| Attribute | Value |
|-----------|-------|
| Total Tickets | 20 |
| Categories | 4 (Technical, Billing, Account, General) |

### Methods Implemented

| Method | Description | How It Works |
|--------|-------------|--------------|
| **Zero-Shot** | No examples needed | Semantic keyword matching |
| **Few-Shot** | 3 examples per class | Example similarity + zero-shot |
| **Top-3 Tags** | Ranked predictions | Probability-based ranking |

### Prompt Engineering
- Enhanced text context for better classification
- Keyword-based semantic understanding
- Example-based similarity matching

---

## 📈 Key Results & Observations

### Performance

| Method | Accuracy |
|--------|----------|
| Zero-Shot | ~80% |
| **Few-Shot** | **~90%** |
| Improvement | +10% |

### Top 3 Tags Example

Ticket: "My account was hacked and charged twice"

Account Access: 42.3% ████████████
Billing: 38.5% ███████████
Technical: 15.2% ████


### Key Observations

1. **Few-shot beats zero-shot** - Examples improve accuracy by ~10%
2. **Confidence is useful** - High confidence = reliable prediction
3. **Ambiguous tickets exist** - Some match multiple categories
4. **Simple approach works** - No heavy models needed for demo

### Recommendations
- Threshold >0.5 for auto-tagging
- Human review for low confidence
- Update examples regularly

---

## 🛠️ Technologies

- Python (Pandas, NumPy, Matplotlib)
- Simulated LLM behavior (keyword semantics)
- Zero-shot & Few-shot techniques

---

## ⏱️ Runtime

| Step | Time |
|------|------|
| Setup | <1 second |
| Classification | <1 second |
| **Total** | **~2 seconds** |

---

## 👨‍💻 Author

AI/ML Engineering Intern  
DevelopersHub Corporation
