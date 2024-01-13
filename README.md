# Weaviate Python V4 Usage Notebook

This minimal notebook illustrates a very simple tour of Weaviate V4 python client.

## Dependencies
- It depends on a local Weaviate container for which a docker-compose has been provided.
  - You should run it either locally or via an SSH tunnel on the 8077 and 50051 ports.
- It also depends on your OpenAI API key being provided (in the `.env` file).
  - Copy/rename the `.env-example` file to a `.env` file.
- The data directory contains description data about approximately 2000 ebooks. Most are English but there also are some Italian books.

## Setup
- First of all, run `poetry install` to add the required python packages.
- Just run the notebook step by step observing its behaviors.

> **Note:** The current version will throw an error if the data insertion portion is run again with the collection already created.
> - To run all again either change the collection name in the `.env` file or delete the collection in the Weaviate database.

---

## Program Description

This program will read a collection of metadata about approx. 2000 books, will create a Weaviate collection for it using OpenAI's text2vec "text-embedding-ada-002" model. The rest of the notebook will show a few different types of semantic and generative queries.

---

