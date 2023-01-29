# Credit-Scoring

- Decision tree is a model that represents a sequence of if-then-else decisions. It’s
easy to understand, and it also performs quite well in practice.
- We train decision trees by selecting the best split using impurity measures. The
main parameters that we control are the depth of the tree and the maximum
number of samples in each leaf.
- A random forest is a way to combine many decision trees into one model. Like a
team of experts, individual trees can make mistakes, but together, they are less
likely to reach an incorrect decision. 
- A random forest should have a diverse set of models to make good predictions.
That’s why each tree in the model uses a different set of features for training.
- The main parameters we need to change for random forest are the same as for
decision trees: the depth and the maximum number of samples in each leaf.
Additionally, we need to select the number of trees we want to have in the
ensemble.
- While in a random forest the trees are independent, in gradient boosting, the
trees are sequential, and each next model corrects the mistakes of the previous
one. In some cases, this leads to better predictive performance.
- The parameters we need to tune for gradient boosting are similar for a random
forest: the depth, the maximum number of observations in the leaf, and the
number of trees. In addition to that, we have eta — the lear

## Notes

To train a random forest, we can do this :
- Train N independent decision tree models
- For each model, select a random subset of features and use only them for training
- When predicitng, combine the output of N models into one
