# leetcode_question_searcher
I have created a search engine which gives leetcode questions based on word searched, this search engine works on tf-idf algorithm.  
Here is the link to the search engine [query-searcher](https://query-searcher.onrender.com/).  
At First, scrapped all the question links from leetcode websites using selenium and chrome webdriver.Then removed the links which are repeated.  
After that scrapped the text from all the question links except premium questions from the links which I had scrapped before.  
Here is the link to scrapped text [text scrapped](https://drive.google.com/drive/folders/1WbRkpDiL5KJLAnc3_KZOOTBYgAw7qPp-?usp=sharing).  
Then preprocessed the data using prep.py file and obtained vocab.txt,documents.txt,idf-values.txt,inverted-index.txt files.  
The files mentioned on line just above are then used to get the results related the searched string in a decreasing order of the score(idf*tf value) of the links.  
