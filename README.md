# Anaphora Coref Resolution (Hindi)

## Dataset

Built a small dataset marking the clusters of anaphoras and co references. For example,
X → श्याम खुद कमरा साफ़ करता है
Y → 1    1  0     0   0    0
Each cluster of noun and pronoun are marked with integers other than 1 and all others are marked as 0. We made a small dataset with about 20 sentences.
 

## Features & Results

- Used BERT model bert_multi_cased_L-12_H-768_A-12. This model has been pre-trained for multiple languages on the Multilingual Wikipedia
- Model Flow : Input layer > Preprocessing > BERT encoder > Dropout > Dense
- Used optimizer Adam with loss function - CategoricalCrossentropy
- Model was trained for 100 epochs
- Though the accuracy turns out to be about 98%, these results may not be of significant importance as the dataset used is really small.
 
