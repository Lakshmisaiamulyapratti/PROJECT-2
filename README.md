# PROJECT - PHASE 2: Document Indexing for Search Engine

## DocumentIndexerHC:
DocumentIndexerHC is a Python tool for creating forward and inverted indices to the documents collected to perform text search. This tool removes stopwords and performs stemming using NLTK then the documents are indexed into a condensed form for easy search.

## Features:
--> Loading of Custom Stopwords: Excludes terms specified in an external file for further modification to the list of stopwords being utilized by the software.

--> Processing of text: Offsets it with NLTK’s Porter Stemmer which aims to convert different inflected forms of the same word to a standard form.

--> Forward index: Each number represents documents with document ID and these numbers are elements in term frequency within the document.

--> Inverted index: Associates the term with the documents in which it was found, as well as terms per document.

## Pre-requisites:

--> Python 3.x

--> NLTK library:

The stopwords can be downloaded from the NLTK library (Loper and Bird, 2002) where one has to install it and download the stopwords corpus.

--> Required Files:

-> stopwordlist.txt: Name of the custom stopwords file where, one stopword is written in a single line, which excludes from the indexing.

-> Files present in the document: Documents should be placed in a folder named ft911 for example and file names should start with ft911_. 

Each document must be formatted as below:

-> <DOCNO> tag contains a document ID that is unique. 

-> <TEXT> tag contains content of text that is to be indexed. 

## Usage and setup instructions:

--> Initializing the Indexer: An instance of DocumentIndexerHC is to be created.

--> Custom Stopwords loading: Additional stopwords to be loaded from stopwordlist.txt.

--> Documents processing: A program to process the documents stored in a specified directory to construct the forward and the inverted indices.

--> Indices saving to files: Stores the forward and inverted indices to output files so that they would be retrieved later as needed.

## Files generated as output:

--> forward_index.txt: Associates each document with terms present within the document, and the number of occurrences of each term, information on term frequency per document.

--> inverted_index.txt: Links each term directly to each document in which it occurs, with the added frequency count so that a user can quickly search the index by term. 

## Example Workflow:

We have just created stopwordlist.txt and put the documents in the ft911 directory and started the indexing. The forward and inverted indices will be written into the forward_index.txt and inverted_index.txt.

These files allow for:

--> Analysis at document-Level: Get a brief look on which terms are most often used in document as fast as possible.

--> Search at term-Level: Locate all documents concerning a particular word together with the number of occurrences of the term in every document.



#### By,
#### Name: Harichandana Mukkamala
#### Mail ID: HarichandanaMukkamala@my.unt.edu
