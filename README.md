# Embeddings

**Embeddings** are mathematical representations of objects (such as words, sentences, or other types of data) into a continuous vector space. In this space, similar objects are located close to each other, and dissimilar objects are far apart. The primary goal of embeddings is to capture semantic or relational information, allowing for efficient similarity search, clustering, and downstream machine learning tasks.

### Use of Embeddings

- **Natural Language Processing (NLP):** Embeddings in NLP help convert words, phrases, or even entire documents into numbers (or vectors). This allows computers to process and understand human language in a more meaningful way. Essentially, embeddings help capture the relationships between words, so that words with similar meanings are represented as vectors that are close to each other.
- **Recommendation Systems:** In recommendation systems (like those used by Netflix, Spotify, or Amazon), embeddings are used to represent both users and items (like movies, songs, or products). Each user and item is represented as a vector, and the system recommends items based on how "close" they are to the user's preferences in this vector space.
- **Image Processing:** In image processing, embeddings help represent the important features of images (like objects, textures, or colors) as vectors. Instead of looking at the raw pixels, embeddings capture the "essence" of the image, making it easier for computers to compare and classify images.

### Comparison Between Best Methods for Word-level Embeddings

This is a summary of the most used embedding models and the benefits of each. Some could be better for different use cases and also we need to consider the computation complexity, since sometimes the difference in accuracy is not justified by the cost involved in training.

**History of Models and Complexity:**

| **Item**                                                          | **Year Developed** |   **Computation Complexity**   |
| ----------------------------------------------------------------: | :----------------: | :----------------------------: | 
| **Word2Vec**                                                      |        2013        | **Low computational complexity.** Uses a shallow neural network, so it trains quickly, even on large datasets. |
| **GloVe**                                                         |        2014        | **Medium computational complexity.** Involves matrix factorization, which can be resource-intensive for very large corpora. |
| **FastText**                                                      |        2016        | **Medium computational complexity.** Slightly more complex than Word2Vec due to subword information, but still efficient. |
| **ELMo (Embeddings from Language Models)**                        |        2018        | **High computational complexity.** Uses deep bidirectional LSTMs (long short-term memory networks) and requires a large amount of computational power and memory. |
| **BERT (Bidirectional Encoder Representations from Transformers)**|        2018        | **Very high computational complexity.** Uses transformers with bidirectional attention mechanisms, requiring substantial computational power (often needs GPUs/TPUs for training). |
| **Sentence-BERT (SBERT)** |        2019        | **High computational complexity.** Uses transformers but fine-tuned with a focus on sentence embeddings. More efficient than BERT in this context but still resource-intensive. |

**Best Use Cases, Pros and Cons:**

| **Item**     | **Use Cases** |   **Concrete Use Cases**   |
| -----------: | :----------------: | :----------: | :----------: | 
| **Word2Vec** | Simple tasks where efficiency is key. | Text classification, Clustering, Word Similarity. |
| **GloVe**    | Tasks requiring global co-occurrence statistics. | Document Classification, Language Modeling. |
| **FastText** | Handling rare words and out-of-vocabulary (OOV) words, especially in morphologically rich languages. | Handling Rare Words in Low-Resource Languages, Search Engines for Multilingual Queries, Text Classification in Morphologically Rich Languages. |
| **ELMo (Embeddings from Language Models)** | Context-heavy tasks where polysemy matters | Sentiment Analysis, Question Answering, Named Entity Recognition. |
| **BERT (Bidirectional Encoder Representations from Transformers)** | Complex NLP tasks requiring deep contextual understanding. | Text Classification, Machine Translation, Question Answering. | Sentiment Analysis, Question Answering, Named Entity Recognition. | Complex NLP Tasks Requiring Deep Contextual Understanding. | Text Classification, Machine Translation, Question Answering. |
| **Sentence-BERT (SBERT)** | Sentence or paragraph-level tasks like semantic search, paraphrase detection, and sentence similarity. | Semantic Search for Retrieving Similar Documents, Paraphrase Detection, Sentence Similarity Tasks. |
