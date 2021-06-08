# Prediction

Prediction of student behavior has been a prominant area of research in learning analytics and a major concern for higher education institutions and ed tech companies alike. It is the bedrock of [methodology within the world of cognitive tutors](https://solaresearch.org/hla-17/hla17-chapter5/) and these methods have been exported to other areas within the education technology landscape. The ability to predict what a student is likely to do in the future so that interventions can be tailored to them has seen major growth and investment, [though implementation is non-trivial and expensive](https://www.newamerica.org/education-policy/policy-papers/promise-and-peril-predictive-analytics-higher-education/). Although some institutions, such as [Purdue University](https://www.itap.purdue.edu/learning/tools/forecast.html), have seen success we are yet to see widespread adoption of these approaches as they tend to be highly institution specific and require very concrete outcomes to be useful. 

## Purpose of the Project
* Create predictions of which students are likley to drop out of which courses and use these predictions to inform semester planning
* Construct classification models (CART, C4.5 and C5.0) to predict student dropout and state validation metrics for the model
* Compare classification models on appropriate metrics

## Data

The data (drop-out.csv) comes from a university registrar's office. The code book for the variables are available in the file code-book.txt.

## Procedure

* Examine the variables and their definitions
* Sseparate  data set into a training set and a test set
* Randomly select 25% of the students to be the test data set and leave the remaining 75% for training data set
* Predict the student level variable "complete"
* Visualize the relationships between the chosen variables as a scatterplot matrix

![image](https://user-images.githubusercontent.com/70524046/121271258-4cd87780-c891-11eb-9a19-feaeb39f0b46.png)

* Construct a classification tree that predicts complete using the caret package
* Train a Conditional Inference Tree using the `party` package on the same training data
* Install the C50 package, train and then test the C5.0 model on the same data
* Compare the models with caret

## Software

[R](https://www.r-project.org/)

[RStudio](https://www.rstudio.com/)

[caret](https://topepo.github.io/caret/train-models-by-tag.html)

[C50](https://topepo.github.io/C5.0/)

[Weka Suite](https://www.cs.waikato.ac.nz/~ml/weka/)

[Java Runtime Environment (JRE) and Java Development Kit](http://www.oracle.com/technetwork/java/javase/downloads/jre9-downloads-3848532.html)

[RWeka](https://cran.r-project.org/web/packages/RWeka/index.html)

[rpart](https://cran.r-project.org/web/packages/rpart/rpart.pdf)
