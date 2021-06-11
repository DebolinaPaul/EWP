# R Codes for Entropy Weighted Power k-means
This repository contains the R codes for EWP algorithm. The algorithm is based on our AISTATS'20 paper, 

Chakraborty, S., Paul, D., Das, S. and Xu, J., 2020, June. Entropy weighted power k-means clustering. In International Conference on Artificial Intelligence and Statistics (pp. 691-701). PMLR. http://proceedings.mlr.press/v108/chakraborty20a.html

If you find these codes useful, kindly acknowledge so by citing the aforementioned paper.

The main function is entropy_weight.power.k.means

### entropy_weight.power.k.means
#### Inputs:

1. X      : an $n \times p$ matrix whose rows denote the data points.
2. s      : The initial exponent fparameter for the power mean. Default is -1.
3. lambda : The entropy penalization parameter. Must be non-negative.
4. eta    : Learning rate for s. Default is 1.04.
5. tmax   : Maximum number of iterations to be run. Default is 200.
6. tol    : Maximum relative error the algorithm should achive. Defailt is 1e-05.

#### Outputs

1. theta  : A $k \times p$ matrix, whose rows represent the cluster centroids.
2. label  : A n length vector representing the class labels.
3. weight : A p length vector of the found feature weights.

The codes for Power _k_-means (http://proceedings.mlr.press/v97/xu19a.html) is given is implemented in the power.k.means function. 
