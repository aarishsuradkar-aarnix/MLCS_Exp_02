Methodology – Steps in Defining a Problem in ML/AI
1. Understand the Problem Domain:
The domain of cybersecurity involves identifying, analyzing, and mitigating digital threats.
Specific areas include spam filtering, intrusion detection, malware analysis, and phishing
detection.
Example Context: In phishing detection, attackers craft fake websites that appear legitimate to
steal user credentials. These threats evolve constantly, making static detection systems insufficient.

2. Articulate the Problem Statement:
Problem Statement:
"Develop a machine learning model that classifies websites as phishing or legitimate with at least 90% accuracy, enabling early warning and automated takedown actions to reduce user exposure and financial loss."

This statement:
● Defines the task: classification 
● Outlines the success criteria: ≥90% accuracy
● Links to business goals: security, automation, cost saving

3. Identify Input Data Requirements:
● Data Needed:
o URL-based features (length, use of IP, special characters)
o WHOIS metadata (domain age, registrar)
o Domain reputation (VirusTotal, blacklists)
o Website content features (HTML tags, scripts)
● Format: CSV or JSON 
● Source: Public datasets like PhishTank, OpenPhish
● Bias & Privacy Considerations: Ensure dataset diversity across languages and regions;
avoid overfitting to a specific domain type.

4. Define Output Requirements:
● Output Format: Binary classification – “phishing” or “legitimate”
● Evaluation Metrics: Accuracy, precision, recall, F1-score
● Interpretability: Feature importance ranking or SHAP values
● Real-time Needs: Fast inference time (<1s per URL) for live web monitoring

5. Establish Constraints and Assumptions:
● Constraints:
o Real-time performance required (for automated web scanners)
o Limited labeled phishing data
o Compliance with data privacy regulations
● Assumptions:
o Data provided is representative of real-world web traffic
o URLs alone can sufficiently distinguish phishing attempts (without full HTML
content)
● Ethical Consideration: Ensure false positives are minimized to avoid unnecessary
disruption to legitimate businesses.

6. Evaluate Feasibility and Impact:
● Feasibility:
o Lightweight models (e.g., decision trees, logistic regression) can run in
constrained environments.
o Pre-trained transformers (e.g., URL-BERT) may enhance accuracy with more
computing power.
● Impact:
o Reduces manual investigation workload
o Helps in early detection of phishing campaigns
o Can be integrated with browser extensions or email filters

7. Document and Refine:

All steps, datasets, assumptions, and planned workflows should be documented in a version-
controlled format (e.g., README.md in GitHub or project documentation tool). Updates should reflect dataset changes, model performance evolution, and stakeholder feedback.
