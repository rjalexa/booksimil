# booksimil
 Weaviate python V4 usage notebook

 This minimal notebook illustrates a very simple tour of Weaviate V4 python client

 It depends on a local Weaviate container for which a docker-compose has been provided.
 You should run it either locally or via an SSH tunnel on the 8077 and 50051 ports

 It also depend on your OpenAI API key being provided (in the .env file)

 Copy/rename the .env-example file to a .env file

 The data directory contains description data  about approximately 2000 ebooks. Most are English but there also are some Italian books.

 Just run the notebook step by step observing its behaviours.

 Please note that the current version will throw an error if the data insertion portion is run again with the collection already created.

 To run all again either change the collection name in the .env file or delete the collection in the Weaviate database.
