# Hive Assignment 1. DDL: Create Tables
The purpose of this task is to create an external table on the posts data of the stackoverflow.com website.

Create your own database and 'use' it. Create external table 'posts_sample_external' over the sample dataset with posts in '/data/stackexchange1000' directory. Create managed table 'posts_sample' and populate with the data from the external table. 'Posts_sample' table should be partitioned by year and by month of post creation. Provide output of query which selects lines number per each partition in the format:

```
year <tab> month <table> lines count
```

where year in YYYY format and month in YYYY-MM format. The result is the 3th line of the last query output.

The result on the sample dataset:

```
2008    2008-10 73
```
