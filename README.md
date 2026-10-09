
For an overview of the assignment domain and implementation, see: [PyTorch tutorial](https://docs.pytorch.org/tutorials/intermediate/seq2seq_translation_tutorial.html). All notebook code credits and references it.</br></br>

#### Additional notes
This notebook version contains code changes made according to 1. and 2. of the assignment (see **Assignment** section below).
The pretrained word2vec is applied to only the english decoder, as word2vec google-news does not contain french vectors.

#### Assignment
Train and evaluate the model, then implement the attention strategy near the end of the (PyTorch tutorial) page. </br></br>
Make the following changes to the code:</br>
1. Replace the embeddings with pretrained word embeddings such as word2vec, Fastext, or GloVe.
2. Try 3 experiments with more layers,  or more hidden units. Compare the training time and results.</br></br>
Submit a link to a git hub repository or other public facing git remote repo that I can access.

##### Datasets
1. pytorch tutorial's dataset 
2. gensim's word2vec google news model

##### Directory
`eng-fra.txt`: this assignment's translation dataset </br></br>
`A6_RNN.ipynb`: all code implementation and discussion of 3 experiments' results at the end of the notebook.</br></br>
`outputs/baseline_output.md`: baseline output after training and evaluation using the tutorial's code, unchanged. This instance uses the encoder and decoder. </br></br>
`outputs/attention_output.md`: baseline output after training and evaluation using the tutorial's code, unchanged. This instance uses the encoder and attention decoder. </br></br>
`outputs/decoder_pretrained_embed_output.md`: baseline output after the decoder's embeddings were replaced with word2vec pretrained embeddings. This instance uses the encoder and decoder with the word2vec embeddings. </br></br>
`outputs/3_experiments_output.md`: 3 experiments' output after training after the attention decoder's embeddings were replaced with word2vec pretrained embeddings. These instances use the encosder and attention decoder. </br></br>
`results/experiments_comparison.png`: table visual comparing the three experiments' performance and loss results




