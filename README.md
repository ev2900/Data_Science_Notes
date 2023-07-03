# Key Concepts in Classification Model(s)

**True positive** an outcome where the model correctly predicts the positive class. A correct prediction <br>
**True negative** an outcome where the model correctly predicts the negative class. A correct prediction <br>
**False positive** an outcome where the model incorrectly predicts the positive class. An incorrect prediction <br>
**False negative** an outcome where the model incorrectly predicts the negative class. An incorrect prediction <br>

## Precision, Accuracy & Recall

**Precision** 
* $\frac{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives}{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} false \hspace{1mm} positives \hspace{1mm}}$
  
* The best possible precision a model can achieve is 1
* The worst possible precision a model can achieve is 0
* If you picture a target with a bullseye - precision is how tight a grouping of shots at the target are
* Precision can also be thought of as the proportion of positive identifications that were actually correct
* *Example* if we have a classification model that predicts will it rain or not and the model has a precision of 0.5 (ie. 50%). When the model predicts it will rain it is correct 50% of the time
* Bear in mind that precision only looks at positives. The formula for precision does not include true or false negatives
  
**Accuracy**
* $\frac{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} negatives}{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} negatives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} false \hspace{1mm} positives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} false \hspace{1mm} negatvies \hspace{1mm}}$
* OR $\frac{number \hspace{1mm} of \hspace{1mm} correct \hspace{1mm} predictions}{total \hspace{1mm} number \hspace{1mm} of \hspace{1mm} predictions}$
  
* The best possible accuracy a model can achieve it 1
* The worst possible accuracy a model can achieve is 0
* If you picture a target with a bullseye - accuracy is how close the shots at the target are to the center of the bullseye
* Accuracy can also be thought of as the proportion of predictions the model got right
* *Example* if we have a classification model that predicts will it rain or not and the model has a accuracy of 0.5 (ie. 50%). When the model predicts it will rain OR it will not rain it is correct 50% of the time
* Bear in mind that accuracy can be impacted by data skew or an unbalanced data set. An unbalanced data set is one that has a dispositional amount of a single class. Using our will it rain classification model example - if we have a data set with 10 days of weather history and 9 of the days it did not rain our data set is skewed in the direction of the negative class. Accuracy determined by testing with a skewed data set can resulting in a misleading depiction of accuracy. This reason is why recall is often used instead of accuracy

**Recall**
* $\frac{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives}{number \hspace{1mm} of \hspace{1mm} true \hspace{1mm} positives \hspace{1mm} + \hspace{1mm} number \hspace{1mm} of \hspace{1mm} false \hspace{1mm} negatives}$

* The best possible recall a model can achieve is 1
* The best possible recall a model can achieve is 1
* Recall can be thought of as the proportion correctly classified positive classes among all the real positive classes
* Using our will it rain classification model example, recall is proportion of times the model predicated it would rain among all the times it actually rained

**Which metric is most important?**
Using our will it rain classification model example
* Optimize for accuracy when you want to predicting both when it will rain and when it will not rain correctly and our dataset is balanced enough
* Optimize for precision when you want predictions of when it will rain to be as correct  as possible
* Optimize for recall when we want our model to spot as many real rainy days as possible

Bonus **F1 score**
* $2 * \frac{Precision \hspace{1mm} * \hspace{1mm} Recall}{Precision \hspace{1mm} + \hspace{1mm} Recall}$

* Harmonic mean of precision and recall
* Combines precision and recall into a single metric
