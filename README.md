This is a small side project to determine the most similar quote to any input with NLP techniques and gain some practice with web scraping and web app development. 
Such a function clearly has many potential applications, e.g. a speech writer gauging the originality of a particular phrase vs. its similarity to previously delivered rhetoric.  
First, a set of ~ 25000 quotes were scraped from the \href{https://www.brainyquote.com/} website along with labeled topics. 
Due to the strong overlaps and similarity between topic names, I forgoed traditional classification.
I generated a word2vec vectorization for each quote in the scraped database and looked at its cosine similarity with any given sample.  
The results seem promising, although there appears to be a large variance in the most similar quote returned. 
The next steps are to deploy the NLP model into a web application with a functioning front-end. 
