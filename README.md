# Collecting Data - Assignment 4
## Past vs. Present: American Presidential Inaugurals

<img src="https://github.com/LTelnekes/Collecting-Data---A4/blob/main/Presidents_Image.jpg?raw=true" alt="Presidents in Corpus" height="500" align="center"/> 

[Official Portraits of Presidents in this Corpus](https://www.loc.gov/free-to-use/presidential-portraits/)


### Corpus Description
This corpus contains 10 American Presidential Inaugural Speeches. It consists of the first five presidential inaugurals (1789, 1793, 1797, 1801, 1805) as well as the last five presidential inaugurals (2005, 2009, 2013, 2017, 2021). This collection was created to explore the potential change of the rhetorical genre of the presidential inaugural speech over time. The results can potentially demonstrate shifts in trends, as well as relevant topics in presidential discourse at the wake of a new administration entering the White House. 

### Target Audience
The dataset is intended for scholars and others that are interested American political culture, rhetoric, and history as well as humanists interested in the 
analysis of linguistic trends within the genre of the American political inaugural address, analyzed through digital tools and methods. 

### Intended Use
The corpus is designed for research purposes, allowing for the study of language and rhetoric within the inaugural adresses of these American Presidents, as well as a comparitive analysis. The CSV-file can be used for several analyses, as well as the conservation of these 10 inaugural adresses. 

### Text Selection Criteria
The speeches in the corpus were selected by the time they were given by the President. As the limits of this assignment only allowed for a certain sized corpus, the first 5 inaugurals in the history of the U.S. were selected, as well as the 5 most recent inaugurals. By selecting the same amount of speeches in both time periods, the dataset represents a relevant and representative corpus for comparision. 

### Data Collection Process
The transcripts of the speeches were collected from [The American Presidency Project](https://www.presidency.ucsb.edu/documents/app-categories/spoken-addresses-and-remarks/presidential/inaugural-addresses). The metadata was created in line with this assignment's criteria and collected from the same source. The President's Inaugural Adresses are available through many online resources, and according to [New Media Rights](https://www.newmediarights.org/business_models/artist/president%E2%80%99s_inaugural_speech_public_domain) belongs to the public domain, "because of the general rule that all works created by the federal government are in the public domain."


### Cleaning and Preprocessing
The transcripts of the speeches are stored in seperate txt files, so in total, 10 seperate txt files were collected and converted and merged with a CSV file of metadata in a Python Dataframe. Using Python, the text in the speeches were cleaned for analysis and storing. Furthermore, tokenization and lemmatization were applied to standardize the language in the corpus.


### Annotations
Annotations were added to identify and count thematic keywords, with the following tools employed:
spaCy for NLP tasks such as tokenization and lemmatization.
Custom Python scripts for keyword frequency analysis.

To the original CSV I used the spaCy library to add Doc, Tokens, Lemma's, Part-Of-Speech and Named_Entities and their corresponding NE_Words to the songs. To make this easier I have converted the CSV into a dataframe.


### File Format and Description of Columns
- `.txt` transcrips of the inaugural adresses
- `.csv` metadata of the inaugural adresses
- `.jpg` image of the presidents in the corpus

**Colums in CSV:**

| Variable      | Description                                  |
| ------------- | -------------------------------------------- |
| Filename       | The filename corresponding to the correct speech file|
| name_president     | The name and surname of the President             |
| president_no  | The number in the line of presidents                     |
| date_of_inaugural          | The date the inaugural adress was delivered by the President |
| Speech       |  The unedited speech as it appears in the txt file |
| Doc    | The text as processed by using spaCy    |
| Tokens           | Tokenized transcript of speech                      |
| Lemmas          | Lematized transcript of speech                        |
| POS           | Part of Speech: information about syntacic role of words in transcript. Each word has its own POS tag |
| Proper_Nouns | The words tagged by spaCy as proper nouns | 
| Named_Entities          | The categories of entities in the transcripts                       |
| NE_Words          | The words assigned to the Named Entities in the transcripts |


### Additional Notes
- A more complete comparative analysis would include all the Inaugural Adresses and would dive deeper into contextual information to arrive at more nuanced conclusions.
- I have added some examples of how you can use this coprus and dataframe to make visualizations which can serve as the basis of new research
