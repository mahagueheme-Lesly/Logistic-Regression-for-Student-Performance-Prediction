
# Logistic Regression for Student Performance Prediction

## Overview
This project predicts whether a student **passes or fails** in two subjects: **Mathematics** and **Portuguese**.  
It also investigates which factors most influence student performance in each subject.

Currently, the work has started on the **Math dataset**, and the next steps will include regularization and Portuguese analysis.

---

## Questions We Are Answering
1. Can we predict **Pass (1) / Fail (0)** for students in Math and Portuguese based on their attributes?  
2. Which features most influence passing in each subject?  
3. Do students who perform well in Math also perform well in Portuguese?  
4. How does overfitting affect the model, and can regularization improve generalization?

---

## Dataset
- Two datasets are available:
  - `student-mat.csv` → Math course grades  
  - `student-por.csv` → Portuguese course grades  
- **Merged dataset:** Combined on common student attributes for cross-subject analysis.  
- **Columns:** For Pass/Fail prediction:
  - `pass_math` → 1 = Pass, 0 = Fail  

> You can still work with individual datasets if preferred. Any changes to datasets or features should be communicated.

---

After you clone

1. **Create and activate a virtual environment named `VENV`:**

```bash
python -m venv VENV
# Windows
VENV\Scripts\activate
# macOS/Linux
source VENV/bin/activate

2. Install required libraries

pip install -r requirements.txt

If you install any new library, add it to requirements.txt.


---



## Current Progress

- Data loaded and cleaned  
- Categorical variables encoded  
- Model implemented for **Math dataset** using **logistic regression from scratch**  
- Training accuracy: ~74%  
- Test accuracy: ~71% → slight overfitting detected  
- Feature importance computed to understand variable influence


## Next Steps

1. Apply **regularization** to reduce overfitting.  
2. Repeat the model for **Portuguese dataset**.  
3. Compare feature importance between Math and Portuguese.  
4. Investigate correlation of performance across subjects.  
5. Plot graphs for visual insights (grades distribution, correlations, feature importance).  
6. Optional: Compare from-scratch model with `scikit-learn` logistic regression to validate results.
