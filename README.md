
# Resume Screening

In an organization, hiring resources is an important part for the growth of an 
organization. The career portal will usually list out different job openings.
Individual candidates and third party consultancy will be uploading numerous
resumes for each job profile.

However, for the hiring comititee, going through each of the resume and 
selecting the candidate for interview is a tedious manual process.

Till date, hiring team has been assigning matching percentage to the candidate's
resume according to the match to the exxact job description (JD). However, going
through each resume is still a time taking process.

In this project, we introduce a ML model, which can extract text from resume and
will predict the match percentage with respect to the JD.


## Acknowledgements

 - [Analytics Vidhya Blog](https://www.analyticsvidhya.com/blog/2021/06/resume-screening-with-natural-language-processing-in-python/)
 - [How to turn text into Features](https://towardsdatascience.com/how-to-turn-text-into-features-478b57632e99)

  
## Documentation

The ML model was trained and finalized using following process :-

Step 1 - Fetch the Training Date which has candidate Id and the matching 
percentage assigned.

Step 2 - Extract text from resume PDF of each candidate and clean up the text.

Step 3 - Train TFIDF word embedding model on the extracted text and transform to word vectors.

Step 4 - Train Regression Models with the word vectors and the match percentage
as Label.

Step 5 - Perform cross validation tests to analyze the model performance.

Step 6 - From Test Folder, extract the resume text and transform to word vector
using the earlier trained TFIDF embedding model.

Step 7 - Use the trained regression model to predict the match percentage of test data resumes.

  
## Tech Stack

Colab Notebook, NLTK, TFIDF, Machine Learning, NLP

  
## Installation

Install PDF Text extraction libraries with PyPDF2, pdfplumber, textract

```bash
    pip install PyPDF2
    pip install pdfplumber
    pip install textract

```

Download NLTK Library Stop words

```bash
    import nltk
    nltk.download('stopwords')
```
    