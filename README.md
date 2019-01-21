# AISES
Automation Examination system


## Cases Considered
1. Extracts Questions from Excel Sheet. We call it Question banks. Every exam is created from Question Banks Excel Sheets. Exams created and stored in Excel sheets which can be read while starting Exam.(Automation of Paper generation)
2. Each answers will be stored in a text files which will be stored to compare the anwers given by students.(Record Keeping of Answers)
3. Algorithm to compare the descriptive Exam papers. Checking will be alloted to Admin so when no usage of server the checking can take place, Teacher just need to set flag which Exams are over and calculation need to be done.

## Paragraph Comparing algorithm
1. Breaking into sentences.
2. Tokenizing every sentences.
3. Remove articles / prepositions / words with low weighted stop words, we belive in exams the key words presence thows more intuition into how much a student knows about the concepts.
4. Lemmatizing the remaining tokens. 
5. Comparing and matching weights with sentences, to know the presence of the sentences.
6. Weight of Every Sentence is given Equal. Calculation of percentage of sentences similarity is made. We assumes if 80% of all High weighted words can makes the senteces similar. And according to it we sum it up to calculate the similarity of the paragraphs.


## To Run 
Python version used 3.7

1) install all requirement

2) Run following in python terminal

```python
import nltk
nltk.download('punkt')
nltk.download('averaged_perceptron_tagger')
nltk.download('wordnet')
```
