Movie Recommendation System
The Training Data
The training data: a set of movie ratings by 200 users (userid: 1-200) on 1000 movies (movieid: 1-1000). The format of the data is as follows: the file contains 200 blocks (users) of
lines. Each line contains a triple : (U, M, R), which means that user U gives R points to movie M. In other words, U is the User ID, M is the Movie ID, and R is the corresponding rating. A
rating is a value in the range of 1 to 5, where 1 is "least favored" and 5 is "most favored".

The Test Data
There are three test files: test5.txt, test10.txt and test20.txt.
A pool of movie ratings by 100 users (userid: 201-300). Each user has already rated 5
movies. The format of the data is as follows: the file contains 100 blocks of lines. Each block
contains several triples : (U, M, R), which means that user U gives R points to movie M. Please
note that in the test file, if R=0, then you are expected to predict the best possible rating
which user U will give movie M. The following is a block for user 276. (line 6545-6555 of
test5.txt)

276 42 4 // user 276 gives movie 42 4 points.
276 85 2 // user 276 gives movie 85 2 points.
276 194 5 // user 276 gives movie 194 5 points.
276 208 5 // user 276 gives movie 208 5 points.
276 585 1 // user 276 gives movie 585 1 point.
276 4 0 // need to predict user 276's rating for movie 4
276 26 0 // need to predict user 276's rating for movie 26
276 33 0 ...
276 56 0
276 63 0
276 67 0
276 72 0

Tasks
Your task is to design and develop collaborative filtering algorithms that predict the unknown
ratings in the test data by learning users' preference from the training data.
Please complete the following experiments:
1. User-Based Collaborative Filtering Algorithms (40 points)
1.1 Implement the basic user-based collaborative filtering algorithms
Please implement two versions of the basic user-based collaborative filtering algorithm as the
Cosine similarity method and Pearson Correlation method.
1.2 Extensions to the basic user-based collaborative filtering algorithms
Please implement the following two modifications (individually and both) to the standard
algorithm (using Pearson Correlation): 1. Inverse user frequency; 2. Case modification.
2. Item-Based Collaborative Filtering Algorithm (30 points)
Please implement the item-based collaborative filtering algorithm based on adjusted cosine
similarity.
3. Implement your own algorithm (15 points)
You can implement your own algorithm to improve your recommendation performance. The
grading will be based on the performance and novelty of the algorithm. Please describe your
own algorithm in detail in the report.
4. Results Discussion (15 points)
Please provide the following information
Compare the accuracy of the various algorithms. Please include a table to show the Mean Absolute
Error (MAE) of your different algorithms that you obtain from the online submission system. Do
you think your results are reasonable? How can you justify the results by analyzing the advantages
and disadvantages of the algorithms?


