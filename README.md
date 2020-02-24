This is a short side project to determine the most similar quote to any input with NLP techniques.
Such a function clearly has many potential applications, e.g. a speech writer gauging the originality of a particular rhetorical phrase.   
First ~25000 quotes were scraped from [brainyquote](https://www.brainyquote.com/) along with topic labels ("Inspirational", "Love", "Alone", etc.) 
Due to the strong overlaps and similarity between topic names, I decided to forgo standard modeling or classification.
Using `spacy` I generated a `word2vec` representation for each quote in the scraped database in order to determine its cosine similarity with any given sample.  
The results seem promising, although there appears to be large variance in the most similar quote returned. 
The next steps are to deploy this tool into a full web app with functioning front-end.
