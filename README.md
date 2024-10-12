# Embeddings

**Embeddings** are mathematical representations of objects (such as words, sentences, or other types of data) into a continuous vector space. In this space, similar objects are located close to each other, and dissimilar objects are far apart. The primary goal of embeddings is to capture semantic or relational information, allowing for efficient similarity search, clustering, and downstream machine learning tasks.

### Use of Embeddings

- **Natural Language Processing (NLP):** Embeddings in NLP help convert words, phrases, or even entire documents into numbers (or vectors). This allows computers to process and understand human language in a more meaningful way. Essentially, embeddings help capture the relationships between words, so that words with similar meanings are represented as vectors that are close to each other.
- **Recommendation Systems:** In recommendation systems (like those used by Netflix, Spotify, or Amazon), embeddings are used to represent both users and items (like movies, songs, or products). Each user and item is represented as a vector, and the system recommends items based on how "close" they are to the user's preferences in this vector space.
- **Image Processing:** In image processing, embeddings help represent the important features of images (like objects, textures, or colors) as vectors. Instead of looking at the raw pixels, embeddings capture the "essence" of the image, making it easier for computers to compare and classify images.

### Summary of Best Methods for Word-level Embeddings
Method	Best Use Cases	Pros	Cons
Word2Vec	Simple tasks where efficiency is key.	Fast, efficient, good at semantic relationships.	Static embeddings, struggles with polysemy, no OOV handling.
GloVe	Tasks requiring global co-occurrence statistics.	Captures global context, good for word analogies.	Static embeddings, OOV issues, needs a large corpus.
FastText	Handling OOV and rare words, morphologically rich languages.	Handles OOV well, captures subword information.	Static embeddings, context-insensitive.
Contextualized (ELMo, BERT)	Context-heavy tasks where polysemy matters.	Dynamic, context-sensitive.	Computationally expensive, not typically necessary for word-level tasks.

| **Item**                                                          | **Year Developed** |   **Computation Complexity**   |
| ----------------------------------------------------------------: | :----------------: | :----------------------------: | 
| **Word2Vec**                                                      |        2013        | Low computational complexity. 
                                                                                           Uses a shallow neural network,
                                                                                           so it trains quickly, even on 
                                                                                           large datasets.                |
| **GloVe**                                                         |        2014        | 23.99 |
| **FastText**                                                      |        2016        | 19.99 |
| **ELMo (Embeddings from Language Models)**                        |        2018        | 42.99 |
| **BERT (Bidirectional Encoder Representations from Transformers)**|        2018        | 42.99 |
| **Sentence-BERT (SBERT)                                         **|        2019        | 42.99 |
