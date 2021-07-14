Training the collaborative filtering algorithm for movie ratings. The movies dataset has a rating for 943 users and 1682 movies.
The goal is to train the collaborative filtering algorithm to predict movie ratings.
Execute the script ex8 cofi.m, which loads the dataset and calls the corresponding functions.
The matrix R is a binary-valued matrix, where is a user i has given rating for a movie j then R(i,j)=1; otherwise, R(i,j)=0.
The algorithm predicts the highest rating for the users with no rating, where R(i,j)=0.
The i-th row of matrix X corresponds to the feature vector for the i-th movie, and the matrix theta corresponds to the parameters.
The file cofiCostFunc.m computes the cost function and gradient (with vectorized implementation) for collaborative filtering based on matrixes X and theta.
Then adding regularization to the cost function and correspondingly the gradients to avoid high variance and have a better algorithm.
After learning the cost function and gradients with regularization, use the algorithm to predict movie recommendations.
