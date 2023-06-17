# leetcode_question_searcher
I have created a search engine which gives leetcode questions based on word searched, this search engine works on tf-idf algorithm.  
Here is the link to the search engine [query-searcher](https://query-searcher.onrender.com/).  
Firstly, I have scrapped all the question links from leetcode websites using selenium and chrome webdriver.  
Then I have removed the links which are repeated.  
After that I have scrapped the text from all the question links except premium questions from the links which I had scrapped before.  
I am attaching the link to scrapped text here [text scrapped](https://drive.google.com/drive/folders/1WbRkpDiL5KJLAnc3_KZOOTBYgAw7qPp-?usp=sharing).  
Then I have preprocessed the data using prep.py file and obtained vocab.txt,documents.txt,idf-values.txt,inverted-index.txt files.  
The above mentioned files are then used to get the results related the searched string in a decreasing order of the score(idf*tf value) of the links.  
