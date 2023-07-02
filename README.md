## Key Concepts in Classification Models

**True positive** an outcome where the model correctly predicts the positive class. Also know as a correct prediction <br>
**True negative** an outcome where the model correctly predicts the negative class. Also know as a correct prediction <br>
**False positive** an outcome where the model incorrectly predicts the positive class. Also know as an incorrect prediction <br>
**False negative** an outcome where the model incorrectly predicts the negative class. Also know as an incorrect prediction <br>

**Precision** 
* $\frac{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives}{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} false \hspace{1mm} positives \hspace{1mm}}$
  
* The best possible precision a model can acheive is 1
* The worst possible precision a model can acheive is 0
* If you picture a target with a bullseye - precision is how tight a grouping of shots at the target are
* Precision can also be thought of as the proportion of positive identifications that were actually correct
* *Example* if we have a classification model that predicts will it rain and the model has a precision of 0.5 (50%). When the model predicts it will rain it is correct 50% of the time 
  
**Accuracy**
* $\frac{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} negatives}{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} negatives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} false \hspace{1mm} positives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} false \hspace{1mm} negatvies \hspace{1mm}}$ OR $\frac{number \hspace{1mm} of \hspace{1mm} correct \hspace{1mm} predictions}{total \hspace{1mm} number \hspace{1mm} of \hspace{1mm} predictions}$
  
* The best possible accuracy a model can acheive it 1
* The worst possible accuracy a model can acheive is 0
* If you picture a target with a bullseye - accuracy is how close the shots at the target are to the center of the bullseye
* Accuracy can also be thought of as the proportion of predictions the model got right

**Recall**
* $\frac{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives}{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} false \hspace{1mm} negatives}$

* The ability of a model to find all the relevant cases within a data set
* Recall can be a better metric to measure a model - instead of accuracy

**F1**
* 2 * ( Precision * Recall ) / (Precision + Recall)
