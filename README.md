# NLP-Project-Fake-News-Detection
NLP-Project-Fake-News-Detection

### Dataset Used : LIAR Dataset 
Paper : https://arxiv.org/abs/1705.00648 <br>
Data : https://www.cs.ucsb.edu/~william/data/liar_dataset.zip

### Original Source:
The paper did not release the source code.

### List of commands:
Run all the cells in the ipython notebook.

#### Train :
**function : train(model,architecture, use_pos, use_meta, use_dep)** <br>
* params : <br>
  - model : keras Sequential model <br>
  - architecture : 'lstm' or 'cnn' <br>
  - use_pos : boolean (tells whether the POS embeddings are to be used as input to the model for training) <br>
  - use_meta : boolean (tells whether the metadata is to be used as input to the model for training)  <br>
  - use_dep : boolean (tells whether the Dependency parse embeddings are to be used as input to the model for training)  <br>

#### Evaluation on test:
**function_1 : (false_predicted,true_predicted) = evaluate(model, use_pos, use_meta, use_dep)**
* params : <br>
  - model : keras Sequential model <br>
  - use_pos : boolean (tells whether the POS embeddings were used as input to the model while training) <br>
  - use_meta : boolean (tells whether the metadata was used as input to the model while training)  <br>
  - use_dep : boolean (tells whether the Dependency parse embeddings were used as input to the model while training)  <br>
* returns : <br>
  - false_predicted : dictionary with *keys* as indices of test samples that were classified as "pants-on-fire" (false news) and *values* as the softmax probability for this class label. <br>
  - true_predicted : dictionary with *keys* as indices of test samples that were classified as "true" (not a fake news) and *values* as the softmax probability for this class label.  <br>

**function_2 : print_best_false_true_predicted(false_predicted,true_predicted)**
* params : <br>
  - outputs from the above mentioned evaluate() function. <br>
* outputs : 
  - prints top 5 sentences which where predicted as "pants-on-fire" (fake news) with highest softmax probabilities. <Br>
  - prints top 5 sentences which where predicted as "true" (not fake news) with highest softmax probabilities.
  

## Software and Library Requirements:

Just do `pip install -r requirements.txt`