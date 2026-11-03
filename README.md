# Phishing Website Detection Using Machine Learning

**Project by:** Shubhangi Waghwase

## 1. Project description
This project uses supervised machine learning to classify website records as **Phishing** or **Legitimate** based on website and URL-related features. It trains and compares Decision Tree, Logistic Regression, and AdaBoost classifiers.

This is an academic demonstration, not a real-time browser protection product.

## 2. Dataset
- **Name:** UCI Phishing Websites (Dataset ID: 327)
- **Dataset page:** https://archive.ics.uci.edu/dataset/327/phishing+websites
- **Size:** 11,055 records and 30 input features (as described by UCI)
- **Target convention:** -1 = phishing, 1 = legitimate
- **License:** CC BY 4.0; provide attribution when reusing the dataset.

The notebook downloads the dataset directly through the `ucimlrepo` Python package. An internet connection is required for the first download.

## 3. Technologies used
- Python 3
- Jupyter Notebook
- pandas and NumPy
- scikit-learn
- Matplotlib
- UCI Machine Learning Repository (`ucimlrepo`)

## 4. Project files
- `Shubhangi_Waghwase_Phishing_Website_Detection.ipynb` — complete code and evaluation workflow
- `requirements.txt` — Python dependencies
- `Shubhangi_Waghwase_ProjectReport.docx` — project documentation
- `README.md` — project overview and run instructions

## 5. Setup instructions
1. Install Python 3.10 or later.
2. Place the notebook and `requirements.txt` in the same folder.
3. Open Command Prompt or Terminal in that folder.
4. Create and activate a virtual environment (recommended):

   **Windows**
   ```bash
   python -m venv .venv
   .venv\\Scripts\\activate
   ```

   **macOS/Linux**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

5. Install dependencies:
   ```bash
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```
6. Start Jupyter:
   ```bash
   jupyter notebook
   ```
7. Open `Shubhangi_Waghwase_Phishing_Website_Detection.ipynb` and choose **Kernel → Restart & Run All**.

## 6. Expected workflow
The notebook loads the UCI dataset, checks its shape and labels, prepares the features, creates an 80:20 stratified train/test split, trains three models, and displays accuracy, precision, recall, F1-score, classification reports, and confusion matrices.

**Do not assume or report an accuracy value before running the notebook.** Results depend on the installed library versions and the evaluation split.

## 7. Important limitations
- The model does not scan a live website or accept a raw URL directly.
- Historical training data cannot guarantee detection of new phishing methods.
- Predictions are not proof that a website is safe or unsafe.
- Use trusted security tools and independent checks; do not submit sensitive information to suspicious websites.

## 8. Dataset citation
Abdelhamid, N. (2015). *Phishing Websites* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C51W2X

## 9. Author
**Shubhangi Waghwase**
