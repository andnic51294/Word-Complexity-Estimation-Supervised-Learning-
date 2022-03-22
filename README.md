# Word Complexity Estimation-Supervised-Learning
Estimating the probability of a target word being complex.The training set consists of 14,002 labeled examples. The test set consists of another 1,764 examples.

## The training data will be provided in the following format:

1  China and Taiwan flexed their muscles.   17  37  flexed their muscles    10  10  3   2   0.25

2  China and Taiwan flexed their muscles.   17  23  flexed  10  10  2   6   0.4

3  China and Taiwan flexed their muscles.   30  37  muscles 10  10  0   0   0.0

Each line represents a sentence with one complex word annotation and relevant information, each separated by a TAB character.

The first column shows the ID of the training sample.
The second column shows the actual sentence where there exists a complex phrase annotation.
The third and fourth columns display the start and end offsets of the target word in this sentence.
The fifth column represents the target word.
The sixth and seventh columns show the number of native annotators and the number of non-native annotators who saw the sentence.
The eighth and ninth columns show the number of native annotators and the number of non-native annotators who marked the target word as difficult.
The tenth column shows the gold-standard label for the probabilistic regression task.

## Test Data
The test data will be in the following format:

1  Both China and the Philippines flexed their muscles on Wednesday.   31  37  flexed  10  10
In the test input format, only the first seven columns of the train format are given.

## Classifier and Results
The Random Forest classifier was used to estimate the probability of complexity with an mean absolut error of approximately 0.119
