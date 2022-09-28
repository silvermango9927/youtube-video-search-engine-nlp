## Problem Statement
Employees at companies often have to parse through a ton of information in documentation/JIRA/Confluence etc while building their new project. Reading so much documentation and "how to do X" can often be super boring though. 

## Our solution
It is an open source app that scours fully-subtitled videos on the YouTube Database to respond to user queries with an appropriate link leading them to find a solution. Further, timestamps are also provided to make the solutions even more accessible.

This project utilises the following libraries:
* [YouTube Transcript API](https://github.com/jdepoix/youtube-transcript-api)
* [YouTube Search](https://github.com/joetats/youtube_search)
* Scikit-learn
* [Natural Language Toolkit](https://github.com/nltk/nltk)

This project employs natural language processing to boil the transcripts of relevant fetched youtube videos down to just the essential keywords. After that the collections library is used to convert the required keywords into array to preprocess them. [Cosine similarity](https://www.sciencedirect.com/topics/computer-science/cosine-similarity) is used to determine the relevance and how similar the keywords present in the transcript were when compared to the query from the user.

## Future improvements/initiatives
* Basing this on either a web-app or a command line interface so more people can access this
* Creating a clever filter that can help detect and filter out videos without clear transcripts
* Can recommend better videos based on their like ratio, views and subscriber of the channel
