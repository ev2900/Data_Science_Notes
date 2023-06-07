## Key Concepts in Classification Models

**True positive** an outcome where the model correctly predicts the positive class. Also know as a correct prediction <br>
**False positive** an outcome where the model incorrectly predicts the positive class. Also know as an incorrect prediction <br>
**False negative** an outcome where the model incorrectly predicts the negative class. Also know as an incorrect prediction <br>

**Precision** 
* Number of true positives / ( number of true positives + number of false **positives**)
* The best possible precision a model can acheive it 1
* The worst possible precision a model can acheive is 0

**Recall**
* Number of true positives / ( number of true positives + number of false **negatives**)
* The ability of a model to find all the relevant cases within a data set
* Recall can be a better metric to measure a model - instead of accuracy

**F1**
* 2 * ( Precision * Recall ) / (Precision + Recall)
