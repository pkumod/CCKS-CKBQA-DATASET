# CCKS-CKBQA-Datasets
Here is the datasets for CCKS CKBQA competitions. The CCKS conference annually hosts a series of competition tasks and we have been hosting the CCKS Chinese Knowledge Based Question Answering contests since 2018. Hundreds of teams sign up and over 20 of them commit a valid final result each year.

The information of previous competitions can be found with the following links:

CCKS 2018: https://www.biendata.xyz/competition/CCKS2018_4/

CCKS 2019: https://www.biendata.xyz/competition/ccks_2019_6/

CCKS 2020: https://www.biendata.xyz/competition/ccks_2020_7_4/

CCKS 2021: https://www.biendata.xyz/competition/ccks_2021_ckbqa/

... and more!

The datasets consists of benchmark queries set and an open-domain knowledge graph. 

# The benchmark queries
All queries are manually written by students with KBQA knowledge. Up to now, we now have more than 6,000 queries for training and 2,000 for validation and these number is growing every year.

We make sure that at least 50% are complex questions involving over 1 relation so the queries will challenge the performance of KBQA systems. The previous champions achieves at most 0.8 in terms of F1 score. There is still great potential.

The data format is rather simple. Each query consists of 3 lines: the first is the question in Chinese, the second is a corresponding SPARQL, and the third is the answers. For example:

````
q1:新子憧的声优是哪一年出道的？
select ?x where { <新子憧> <配音> ?y. ?y <出道时间> ?x.} 
"2010"	
````
# The dataset
Our dataset is an enriched version of PKUBASE(http://www.openkg.cn/dataset/pku-pie), with several domain-specific knowledge graphs included. Besides, it will be expanded in future contests.

The dataset now contains over 60 million triples and 7 million entities.

The dataset is available via Baidu Netdisk (extraction code t08r): https://pan.baidu.com/s/12ipl18cSTUdrT0w2NIOJ6Q#list/path=%2F

Or Google Drive:
https://drive.google.com/file/d/1pHkwBw45tqlps-LcJlxdtDhrZD86DlJ-/view?usp=sharing



# About Us
It's our hope to maintain a useful benchmark for the Chinese KBQA community. If there is any problems or valuable advices please send an issue freely.
