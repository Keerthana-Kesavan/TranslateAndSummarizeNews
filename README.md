# **Text Analysis Algorithms**

Welcome to the Text Analysis Algorithms section of my GitHub repository. In this repository, I provide details on three key algorithms for text analysis, each designed to extract valuable information and insights from textual data.

## **1. Automatic Extraction Based on Weighting**

### **Overview**

This algorithm employs a statistical approach to extract key information from text documents. It treats sentences as ordered sequences and words as ordered sequences within sentences. The process involves the following steps:

1.Weighting of Words: Words are assigned weights using the tf-idf (term frequency – inverted document frequency) approach. This weight reflects the importance of each word in the document.\
2.Weighting of Sentences: Each sentence is assigned a weight based on the sum of the weights of its constituent words.\
3.Sentence Selection: Sentences with weights above a certain threshold are chosen for inclusion in the summary.\
4.Sentence Ordering: The selected sentences are ordered in the summary in the same sequence as they appear in the original document.


### **Additional Details**

+ The weighting process considers word frequency, location within the document, syntactic structure, and presence in the document title.
+ Term frequency measures how often a word appears within a document, while inverted document frequency indicates the inverse of how many documents a word appears in.
+ Preprocessing techniques such as stop word removal, term normalization, and synonym replacement are applied.


## **2. Automatic Summary Extraction Based on User Query**


### **Overview**

This algorithm focuses on generating summaries that are tailored to user queries. It combines two key parameters to weigh sentences:

1.tf-idf Weighting: Similar to the first algorithm, this approach uses tf-idf weighting to assess the importance of sentences within a document.\
2.Query Relevance: The weight of a sentence is influenced by the number of times the user's query terms appear within it.\

### **Applications**
This method is highly applicable in creating custom story search engines. Users can input queries such as "student wizard magic potions," and the search engine will present relevant stories, such as those resembling Harry Potter, complete with summaries extracted based on the user's query. This ensures users find the most relevant content.

## **3. Information Extraction**

### **Overview**

This advanced algorithm operates in two phases: information selection and summary generation. It significantly enhances the quality of automatic text summarization by considering the following steps:

1.Preprocessing: Removal of punctuation, bracket symbols, and abbreviation expansion.\
2.Part of Speech Annotation: Each word is annotated with its part of speech information (e.g., noun, verb, adjective).\
3.Subject-Verb-Object Extraction: Triplets are extracted from each sentence.\
4.Filtering: Elimination of triplets involving certain verb types.\
5.Noun Phrase Generation: Creation of subject, object, and indirect object noun phrases.\
6.Verb Complement Generation: If no subject is present, prepositional phrases are generated to complement noun phrases.\
7.Verb Phrase Generation: Construction of verb phrases to connect all components.\
8.Ranking: Sentences are ranked based on the document frequency of their terms.\
9.Summary Composition: Sentences are merged to form a coherent summary, with subjects being selectively removed to improve readability.

## **Semantic Analysis**

This method offers an enhanced understanding of text by conducting grammatical analysis. It holds great potential for the development of intelligent agents capable of gaining deeper semantic knowledge from textual data.

Feel free to explore the code and documentation for each of these algorithms in the respective directories.
