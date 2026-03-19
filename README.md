# Detection-of-Fake-News-Trustworthiness-In-Social-Media-Using-Machine-Learning

<h1> Overview <h1\>

The rapid proliferation of digital misinformation presents a significant challenge to the integrity of social media ecosystems. Most existing solutions rely on fact-checking semantic claims, which quickly become outdated. This project develops a robust, content-agnostic machine learning system for automated fake news detection by prioritizing Textual Stylometry—the structural "fingerprints" of deceptive writing.

By extracting features such as sentiment polarity, lexical diversity, and punctuation ratios, the models evaluate how the news is written rather than what it is about, allowing the system to remain effective across diverse and evolving topics.

Methodology
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
