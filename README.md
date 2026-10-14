# AI-Powered Cybersecurity Threat Detection System

A beginner-friendly Python machine-learning demo that classifies **synthetic network-event records** as Normal or Suspicious. It generates data, trains a Random Forest classifier, evaluates predictions, saves the model, and creates charts.

> **Important:** This project uses fictional, generated data. It does not monitor a real network, analyze actual malware, or provide production-grade threat detection. Scores only measure performance on the synthetic demo data.

## Features
- Reproducible synthetic dataset generated locally
- Data preprocessing with a scikit-learn pipeline
- Random Forest classification
- Accuracy, precision, recall, and F1-score
- Saved model, confusion matrix, event distribution chart, and text report
- Sample event prediction

## Tech stack
Python 3.10+, pandas, NumPy, scikit-learn, Matplotlib, joblib.

## Folder structure
```text
AI-Powered-Cybersecurity-Threat-Detection/
├── main.py
├── requirements.txt
├── README.md
├── .gitignore
├── data/       # generated CSV
├── models/     # saved model
├── outputs/    # charts and evaluation report
├── screenshots/ # portfolio screenshots
├── docs/
└── src/
    ├── __init__.py
    └── pipeline.py
```

## Run on Windows
1. Install Python 3.10+ from https://www.python.org/downloads/ and select **Add Python to PATH**.
2. Extract the ZIP and open the folder in VS Code.
3. Open a terminal in the project folder and run:
   ```bat
   py -m venv .venv
   .venv\\Scripts\\activate
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   python main.py
   ```

## Run on macOS/Linux
```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
python main.py
```

## Workflow
1. Generate `data/synthetic_network_events.csv`.
2. Split records into training and testing sets.
3. Impute missing values and scale features in a pipeline.
4. Train and evaluate a Random Forest model.
5. Save `models/threat_detection_model.joblib`.
6. Save charts and metrics under `outputs/`.
7. Predict a sample event as Normal or Suspicious.

## Demo features
`packet_size`, `failed_logins`, `request_frequency`, `connection_duration`, and `unique_ports`. Label `0` means Normal; `1` means Suspicious. These are invented features for learning, not a real public dataset.

## Portfolio proof
After running, capture `screenshots/terminal-results.png`, `screenshots/confusion-matrix.png`, `screenshots/event-distribution.png`, and `screenshots/github-repository.png`. Add images to this README with Markdown links, for example:
```markdown
![Confusion matrix](outputs/confusion_matrix.png)
```

## Future improvements
- Use a documented public dataset such as NSL-KDD or CICIDS
- Add data validation and configurable alert thresholds
- Build a Streamlit dashboard or local Flask API
- Compare Random Forest, Logistic Regression, and Isolation Forest
- Add tests and model versioning

## GitHub topics
`cybersecurity`, `machine-learning`, `threat-detection`, `python`, `scikit-learn`, `network-security`, `beginner-project`

## Author
Student learning project — AI-Powered Cybersecurity Threat Detection System.
