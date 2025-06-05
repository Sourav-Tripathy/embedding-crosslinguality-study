# embedding-crosslinguality-study
A multilingual embedding experiment exploring how language, word order, and translation affect vector similarity across embedding models. Measures cosine similarity and vector order consistency across translated texts to assess language independence and reverse compatibility for RAG systems.

## languages taken for study

**"odia","hindi","spanish","french","telgu","english"**

## Exp1 - (about)

In experiment1 I use **"meta-llama/llama-4-scout-17b-16e-instruct"** to generate a 1000 word essay on a given prompt and then translate that essay into 5 langauges using the same model by a custom system message for proper translation(using llama as they are best at multilaguage benchmark) and then embedd each translated essay using the **"paraphrase-multilingual-MiniLM-L12-v2"**(which is an open source embedding model from hugging face).
After embedding i used cosine similarity to findout the similarity between each translated piece by their embedding and plotted various graphs to see how embeddings of each languge differ and the similarity of how close each language are for the same essay.

## Exp2 - (about)

In experiment2 I use the same embedding model used in experiment1 and take 5 words and their translated version in the same 5 langauge in experiment1 and then embedd them to see for each word how similar the embeddings are using both cosine similarity and various graphs where I plot raw embeddings and compare .

### MORE EXPERIMENTS TO BE ADDED