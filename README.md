Resume to Job Matcher

An NLP-Based Project for Resume Screening
Prepared by: Rupesh Saini

Project Introduction

This project aims to match resumes with job descriptions based on textual similarity. It calculates a match percentage and suggests improvements to increase the chances of shortlisting.

Methodology

1. User Input: The user pastes their resume and job description into text fields.


2. Text Preprocessing:

Tokenization using NLTK

Stop word removal



3. Vectorization:

Uses CountVectorizer from sklearn to transform text into numerical vectors.



4. Similarity Calculation:

Cosine similarity is computed to determine how well the resume matches the job description.



5. Key Term Extraction:

Identifies missing skills/keywords from the job description and suggests adding them.




Key NLP Concepts Used

Stop Words Removal: Eliminates common words that do not contribute to meaning.

Word Tokenization: Splits text into individual words for better processing.

Cosine Similarity: Measures how similar the resume is to the job description.

Key Term Extraction: Identifies missing skills and provides suggestions.


Why Use NLTK Instead of SpaCy?

Better control over text preprocessing for this specific use case.

Built-in stop word lists and tokenization tools.

While SpaCy is better suited for larger NLP pipelines, NLTK is sufficient for this simpler text analysis.


Implementation Overview

Converts the resume and job description into vectors using CountVectorizer.

Computes cosine similarity to determine match percentage.

Uses NLTK for stop word removal.

Extracts missing key terms from the job description and suggests them for inclusion in the resume.


How to Run

1. Install the required dependencies:

pip install streamlit sklearn nltk


2. Run the Streamlit app:

streamlit run app.py


3. Paste your resume and job description in the provided text fields.


4. Click the "Match" button to get a match percentage and keyword suggestions.



Live Demo

Check out the live version of the Resume Matcher here:
Resume Matcher App

Conclusion

The Resume to Job Matcher helps job seekers optimize their resumes by identifying missing keywords and providing actionable feedback. Using NLP techniques like cosine similarity, tokenization, and stop word removal, the project provides accurate resume-job description matching.


---

Author

Rupesh Saini

