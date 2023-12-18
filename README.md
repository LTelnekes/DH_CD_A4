# Collecting-Data---A4

Your github repository should contain:
- A data directory containing corpus files in the text format.
- A single CSV file with all corpus data and annotations.
- The code (Jupyter Notebook) for preprocessing and annotating your text files.
- A README.md file with the relevant documentation.

Documentation should include at least a brief description of:
- The corpus itself.
- Your target audience and the intended use of the corpus.
- Text selection criteria.
- The data collection process.
- Cleaning and/or preprocessing steps if you’ve done any.
- Annotations that you’ve added and tools that you used for that.
- The format of the files in the corpus (in this case, probably txt and csv), as well as the description of the columns in the CSV file.
- The quality checks, if you’ve done any.
- Anything else that you think is important to mention.

Your Jupyter Notebook should contain all the code for preprocessing and annotating your text files. It can also include your code for text data collection, but it doesn’t have to - you can also start from reading your previously downloaded text files into the Notebook. The Jupyter Notebook should end with saving your annotated corpus as a CSV file.

Your CSV file should include all your data from all corpus files, one text document per row, and the following columns:
- Filename (the name of the original text file in the data folder).
- Title (optional; if your texts have titles).
- Document (the original text exactly as it appears in the text file),
- Text (optional; preprocessed text of this document, if you’ve done any cleaning/preprocessing).
- Tokens (tokenized text of this document).
- Lemmas (lemmatized text of this document).
- Parts-of-speech (parts of speech of all the tokens in this document).
- Metadata (optional; in case you want to include any other information about this document - e.g., author, year, etc.).
- Submit a link to your github repository.

Hint: for this assignment, don’t make your corpus too big, otherwise preprocessing might take too long, and your CSV can be large. It may be easier if your corpus has not more than 10,000 word tokens. In any case, please make sure that the total size of your files, including the data folder, is not larger than 100 MB.
