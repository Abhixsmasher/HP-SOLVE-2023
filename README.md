
# WebSenKnowGraph - HP SOLVE 2023

The above code, files, and ouput graph generated are meant for the HP SOLVE competetion of 2023. The *WebSenKnowGraph* is a name given to the project which does Data Scraping for social media sites, in this case twitter, performs sentiment analysis and keyphrase generation on data and converts it into a qery-able knowledge graph.




## Features of the project

- Scraping of data on twitter without the need of APIs and through Xpath on (*Web*)
- Cleaning of text and Sentiment Analysis of Tweets using unsupervised models with high accuracy (*Sen*)
- Keyphrase extraction to get product and feature in spotlight of the tweet (*Know*)
- Knowledge Graph generation that can be visualized and queried to get appropriate output (*Graph*)


## Requirements

To run the project all we need is Jupyter Notebook along with a python interpreter (Anaconda used in this case). Next we need to install the needed libraries which can be done with the given code line

```python
  pip install libraries
```
The libraries is to be replaced with the given list that require installation and will be used in the project :-

* [time](https://www.geeksforgeeks.org/python-time-module/)
* [csv](https://docs.python.org/3/library/csv.html)
* [yake](https://pypi.org/project/yake/)
* [nltk](https://pypi.org/project/nltk/)
* [neointerface](https://pypi.org/project/neointerface/)
* [neo4j](https://pypi.org/project/neo4j/)
* [py2neo](https://pypi.org/project/py2neo/)
* [selenium](https://pypi.org/project/selenium/)
* [numpy](https://pypi.org/project/numpy/)
* [pandas](https://pypi.org/project/pandas/)
* [vadarsentiment](https://pypi.org/project/vaderSentiment/)

Other than the above libraries and software, we also need a running database in Neo4j along with user credentials of a user that can edit and access the database on the provided port access.

We also need a registered account detail on twitter for the scraping of tweets.



## Steps from One *End* to *another*

To get the knowledge graph output and other output files, the following steps are to be taken:

* Install and import the necessary libraries
* Run the function blocks
* Run the respective blocks to initiate a web driver and pass the twitter credentials
* Enter the product on which the scraping is suposed to be done on
* Stop the scraping when needed by scrollling 
* Close the driver and run the remaining blocks to receive the following output files :-
    
        1. .csv files of labelled data and keyphrases
        2. A knowledge graph in the GraphDB of Neo4j with nodes and relationship 
* For getting the nodes of keyphrase extracted from the tweet nodes, download the plugin of GraphXR in the Neo4j database and enable it.
* Move to the extract section after loading the db and select key phrases from labellled_tweets to get the final output knowledge graph
 This graph can be queried in the GraphXR enviornment itself in languages like cypher. The nodes themselves are saved in form of .csv files as nodes and relationships and can be accessed.

## Knowledge Graph with Index
[Screenshot](Knowledge_Graph_Output.png)


