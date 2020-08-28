# AiChamp_Screening



Four Tasks were assigned as contained in "Screening_Test_-_AI_Champ_1.pdf" in the root folder

Task 1 was a manual task of downloading 50 linkedIn profiles as pdf. These can be found in folder profile_pdfs

Tasks 2 and 3 were completed using Python Code. The scripting has been done in ipython notebook format. 
The output for these tasks is present in Output Folder as csv files.


Libraries Used to complete the tasks:
pandas : for creating dataframe and saving output to csv
os : to set filepaths
glob : to recursively read pdfs
fitz : to read text from pdfs (Task 2)
nltk : Natural Language toolkit to do text cleaning,remove stopwords,tokenize text,perform lemmatization etc
re : regular expressions library
textblob : to create word blocks to be used in tf-idf(to extract essential words)
math : to calculate log in idf

The following user defined functions have been used to perform the tasks
1)extractTextFromPDF(filepath)
Input : PDF Filepath
Output : text contained in pdf as string

2)get_wordnet_pos(treebank_tag)
Input : nltk's pos_tag 
Output: wordnet tag 

3)cleanAndTokenizeText(text)
Input : text as string
Output : list of words after cleaning text, tokenizing it, removing stop words, performing lemmatization 

4)getMostFrequentWords(text)
Input : text as string
Output : list of 20 tuples(word,frequency_of_word) for most frequent words

5)tf,idf,n_containing and tf_idf
Input : Take blob and bloblist as input .blob is the text of one document.bloblist is self explanatory
Output : These functions are used to calculate various formuales used in tf-idf calculations 
For further help, read comments in the ipython notebook

6)getMostImpWords(list_of_documents_text):
Input : list of each document text as element of list
Ouput: list of list of most important words for each document



