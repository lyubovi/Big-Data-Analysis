# Hive Assignment 2. DML: Find Most Popular Tags
Compare most popular tags in year 2016 with tags in 2009. Tag popularity is the number of questions (post_type_id=1) with this tag. Output top 10 tags in format:

```
tag <tab> rank in 2016 <tab> rank in 2009 <tag> tag popularity in 2016 <tag> tag popularity in 2009
```
Example:

```
php 5 3 1234 5678
```
For 'rank' in each year use rank() function. Order by 'rank in 2016'.

The part of the result on the sample dataset:

```
...
android 3   52  1809    25
php 4   3   1673    215
python  5   11  1585    108
c#  6   1   1519    423
...
```

