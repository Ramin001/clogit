# clogit
clogit model for migration based on observable wages in each location

This is a part of my job market paper here: https://drive.google.com/file/d/1Odvw_r1a8RxpTdEYvFOd2xjHgrS3DdFs/view?usp=sharing
The goal is to set up a conditional choice model in which households choose their residential location based on their individual wages in all possible destinations. Note that these wages vary across spouse-location pairs, so the unit of obvservation here is individual-location, which makes the size of the model too large to be estimated in Stata, as it takes whole data as a single batch. Here the trick is to set it up in python iteratively on multiple batches, so it can be estimated using a reasonable memory size.
