# NLP-Project-Fake-News-Detection
NLP-Project-Fake-News-Detection

### Dataset Used:
LIAR Dataset :
Paper : https://arxiv.org/abs/1705.00648
Data : https://www.cs.ucsb.edu/~william/data/liar_dataset.zip

### Original Source:
The paper did not release the source code.

### List of commands:
### Train :
train(model_lstm,'lstm', use_pos, use_meta, use_dep)

### Evaluation on test:

(fw,tb) = evaluate('lstm', False)

print_best_false_true_predicted(fw, tb)

## Software and Library Requirements:
Keras==2.2.2
matplotlib==2.1.2
numpy==1.15.4
pandas==0.22.0
pydot==1.4.0
scikit-learn==0.19.1
scipy==1.0.0
sklearn==0.0
spacy==2.0.18
tensorboard==1.9.0
tensorflow==1.9.0
spacy==2.0.18
nltk==3.4
