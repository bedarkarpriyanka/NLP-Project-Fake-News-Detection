# NLP-Project-Fake-News-Detection
NLP-Project-Fake-News-Detection

## Dataset Used:
https://arxiv.org/abs/1705.00648

## Original Source:


## List of commands:
### Train:

train(model_lstm,'lstm', use_pos, use_meta, use_dep)

### Evaluation on test:

(fw,tb) = evaluate('lstm', False)
print_best_false_true_predicted(fw, tb)

## Software and Library Requirements:
Pandas, Numpy, Keras, Nltk, Nltk.Corpus, Spacy, CPickle, Operator, IPython
