# ROBT 407 — SVM learning labs

Four hands-on notebooks with theory, experiments and real-data mini-projects.

| Class | Notebook | Run |
|---|---|---|
| Linear SVMs | [View notebook](https://github.com/berdakh/ROBT407-SVM-Labs/blob/main/student/201_linear_svm.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/berdakh/ROBT407-SVM-Labs/blob/main/student/201_linear_svm.ipynb) |
| Dual SVMs | [View notebook](https://github.com/berdakh/ROBT407-SVM-Labs/blob/main/student/202_dual_svm.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/berdakh/ROBT407-SVM-Labs/blob/main/student/202_dual_svm.ipynb) |
| Kernel SVMs | [View notebook](https://github.com/berdakh/ROBT407-SVM-Labs/blob/main/student/203_kernel_svm.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/berdakh/ROBT407-SVM-Labs/blob/main/student/203_kernel_svm.ipynb) |
| Soft-margin SVMs | [View notebook](https://github.com/berdakh/ROBT407-SVM-Labs/blob/main/student/204_soft_margin_svm.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/berdakh/ROBT407-SVM-Labs/blob/main/student/204_soft_margin_svm.ipynb) |

## Course overview

Four student workbooks connect SVM theory to implementation, visual experiments and real-data mini-projects. Each has seven coding tasks and ten quiz questions (28 tasks and 40 questions total).

- Linear SVM: geometry, margins and robustness; Iris species.
- Dual SVM: optimization, KKT conditions and support vectors; two wine classes.
- Kernel SVM: polynomial and RBF kernels; scikit-learn's 8×8 handwritten digits.
- Soft-margin SVM: hinge loss, regularization and model selection; Breast Cancer Wisconsin classification.

[Open the course page](https://berdakh.github.io/ROBT407-SVM-Labs/).

## Prerequisites and running

Use Python 3 with basic NumPy, linear algebra, differentiation and classification knowledge. In Colab, open a notebook above, sign in and save a copy to Drive. Run cells in order and complete the TODO functions, quiz responses and explanations. The implementation functions intentionally return `None` until completed; checks provide reminders. The model-selection reference workflow is supplied for exploration.

For a local environment:

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m jupyter lab
```

Open a notebook in `student/` with a Python 3 kernel. Datasets are generated or bundled with scikit-learn; package installation requires network access. Static figures are the default. Set `ENABLE_WIDGETS = True` for optional sliders when supported by your frontend.

Each project uses scaling inside pipelines, explicit parameter grids, five-fold stratified cross-validation and a held-out test. See `validation.txt` for the prior execution record and `tested_versions.json` for tested package versions; dependencies are not pinned.

## Educational context

ROBT 407, Fall 2026. Textbook context: *Learning From Data* by Yaser S. Abu-Mostafa, Malik Magdon-Ismail and Hsuan-Tien Lin. Notebooks cite lecture-source page anchors; the source PDFs are not included. Suggested pacing is about 90 minutes of core activities plus 2–3 hours of extensions and mini-project work per class. The Wisconsin dataset is used to teach classification methodology, and the exercise does not establish clinical suitability.

This repository contains student-facing materials. The course page source is in `docs/`. No license has been selected.
