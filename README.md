# Detection-of-Fake-News-Trustworthiness-In-Social-Media-Using-Machine-Learning

<h1> Overview </h1>

The rapid proliferation of digital misinformation presents a significant challenge to the integrity of social media ecosystems. Most existing solutions rely on fact-checking semantic claims, which quickly become outdated. This project develops a robust, content-agnostic machine learning system for automated fake news detection by prioritizing Textual Stylometry—the structural "fingerprints" of deceptive writing.

By extracting features such as sentiment polarity, lexical diversity, and punctuation ratios, the models evaluate how the news is written rather than what it is about, allowing the system to remain effective across diverse and evolving topics.

<h1> Methodology </h1>

The data pipeline consists of gathering baseline datasets (like WELFake, Politifact, Gossipcop) and augmenting them through external scraping using the newspaper3k library to balance the classes.

A comprehensive feature engineering process extracts 9 distinct stylometric attributes:

1. Word Count

2. Sentiment Polarity

3. Subjectivity

4. Lexical Diversity

5. Capitalization Ratio

6. Exclamation Frequency

7. Average Word Length

8. Question Mark Count

9. Digit Ratio

<img width="659" height="381" alt="Feature Importance" src="Visuals/Feature Importance.png" />

Note: The original large datasets and interim CSV files are not included in this repository due to size limits. You can generate the full dataset by running the Jupyter notebooks in numerical order.

<h1> Model Performance & Overfit Mitigation </h1>

Initial training phases revealed significant overfitting in complex models, with generalization gaps reaching nearly 17%. Through strategic pruning, depth limitation, and hyperparameter optimization, the generalization gap was successfully reduced to 4.80%, achieving a peak test accuracy of <span>82.16%</span> with an AUC of 0.90.

<img width="659" height="381" alt="Feature Importance" src="Visuals/Benchmark of Model Performance.png" />

<img width="659" height="381" alt="Feature Importance" src="Visuals/ANN Correlation Matrix.png" />

<img width="659" height="381" alt="Feature Importance" src="Visuals/ROC Curve.png" />
