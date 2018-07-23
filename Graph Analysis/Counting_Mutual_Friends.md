# Counting number of the mutual friends
For each user having ID in the column userId count the amount of his / her common 
friends with each other user having ID in the column userId.

Print 49 pairs of the users having the largest amount of common friends, ordered in 
descending order first by the common friends count, then by id of user1 and finally 
by id of user 2. The format is following: "count user1 user2"7

Example:
```
234	54719	767867
120	54719 767866
97    50787 327676
```
To solve this task use the algorithm described in the last video of lesson 1. 
The overall plan could look like this:
- Create a new column “friend” by exploding of column “friends” (like in the demo 
iPython notebook)
- group the resulting dataframe by the column “friend” (like in the demo iPython notebook)
- create a column “users” by collecting all users with the same id in the column 
“friend” together (like in the demo iPython notebook)
- sort the elements in the column “users” by the function sort_array
- filter only the rows which have more than 1 element in the column “users”
- for each row emit all possible ordered pairs of users from the column “users” 
(tip: write a user defined function for this)
- count the number of times each pair has appeared
- with the help of the window function (like in the demo python notebook) select 
49 pairs of users who have the biggest amount of common friends  

The sample dataset is located at /data/graphDFSample.

The part of the result on the sample dataset:
```
...
3044 21864412 51640390
3021 17139850 51640390
3010 14985079 51640390
2970 17139850 21864412
2913 20158643 27967558
...
```

Notes
- The system grades standard output and error streams from the last non-empty cell.
- If you have clicked "Open tool" and received "404" or "405" error, please reload 
the page from the Coursera interface.  

If you want to deploy the environment on your own machine, please use 
bigdatateam/spark-course2 Docker container.