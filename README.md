This is a small side project to determine the most similar quote to any input with NLP techniques.
Such a function clearly has many potential applications, e.g. a speech writer gauging the originality of a particular phrase vs. its similarity to previously delivered rhetoric.  
First a set of ~ 25000 quotes were scraped from [brainyquote](https://www.brainyquote.com/) along with its labeled topics. 
Due to the strong overlaps and similarity between topic names, I forgoed label classification.
I generated a `word2vec` representation for each quote in the scraped database and determined its cosine similarity with any given sample.  
The results seem promising, although there appears to be a large variance in the most similar quote returned. 
The next steps are to deploy this NLP function into a web application with a functioning front-end. 
