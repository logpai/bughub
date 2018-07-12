# BugRepo

BugRepo maintains a collection of bug reports that are publicly available for research purposes. Bug reports are a main data source for facilitating NLP-based research in software engineering. We categorize the datasets into the following research directions.


### 1. Duplicate bug idenfication

| Project                                  |              Timespan | #Components | \#Issues | \#Issue/day | \#Duplicates | %Duplicates | Median Resolving Time |
| :--------------------------------------- | :-------------------- | ----------: | -------: | ----------: | -----------: | ----------: | --------------------: |
| [Mozilla Core](https://bugzilla.mozilla.org/buglist.cgi?resolution=---&query_format=advanced&product=Core) | 1997/03/28 ~ 2013/12/31 |         130 |  205,069 |        33.5 |       44,691 |       21.8% |            102.1 days |
| [Firefox](https://bugzilla.mozilla.org/buglist.cgi?resolution=---&query_format=advanced&product=Firefox) | 1999/07/30 ~ 2013/12/31 |          52 |  115,814 |        22.0 |       35,814 |       30.9% |             76.4 days |
| [Thunderbird](https://bugzilla.mozilla.org/buglist.cgi?resolution=---&query_format=advanced&product=Thunderbird) | 2000/04/12 ~ 2013/12/31 |          23 |   32,551 |         6.5 |       12,501 |       38.4% |             83.7 days |
| [Eclipse Platform](https://bugs.eclipse.org/bugs/describecomponents.cgi?product=Platform) | 2001/10/10 ~ 2013/12/30 |          21 |   85,156 |        19.1 |       14,404 |       16.9% |             29.8 days |
| [JDT](https://bugs.eclipse.org/bugs/describecomponents.cgi?product=JDT) | 2001/10/10 ~ 2013/12/31 |           6 |   45,296 |        10.1 |        7,688 |       17.0% |             23.0 days |
| [Spark](http://issues.apache.org/jira/browse/SPARK) | 2010/04/01 ~ 2018/01/10 |          29 |   22,639 |         8.0 |        3,077 |       13.6% |              7.1 days |
| [Hadoop](http://issues.apache.org/jira/browse/HADOOP) | 2005/07/24 ~ 2017/11/01 |          45 |   12,855 |         2.9 |        1,861 |       14.5% |             14.3 days |
| [MapReduce](http://issues.apache.org/jira/browse/MAPREDUCE) | 2006/03/17 ~ 2018/01/15 |          63 |    7,019 |         1.6 |          977 |       13.9% |             28.2 days |
| [HDFS](http://issues.apache.org/jira/browse/HDFS) | 2006/04/06 ~ 2018/01/12 |          71 |   12,779 |         3.0 |        1,659 |       13.0% |              9.7 days |
| [HBase](http://issues.apache.org/jira/browse/HBASE) | 2007/02/27 ~ 2018/01/21 |          95 |   19,788 |         5.0 |        1,340 |        6.8% |              6.8 days |
| [Cassandra](http://issues.apache.org/jira/browse/CASSANDRA) | 2009/03/07 ~ 2018/01/21 |          24 |   14,071 |         4.3 |        2,083 |       14.8% |              8.6 days |
| [Mesos](http://issues.apache.org/jira/browse/MESOS) | 2011/02/16 ~ 2018/01/26 |          40 |    8,454 |         3.3 |          800 |        9.5% |             23.5 days |


**Train/test data splitting**: We split each dataset into 80%, 20% according to the chronological order as train/test data respectively.

| Project          |              Total (+/-) |              Train (+/-) |            Test (+/-) |
| :--------------- | -----------------------: | -----------------------: | --------------------: |
| Mozilla Core     | 205,069 (54,237/150,832) | 164,055 (50,122/113,933) | 41,014 (4,115/36,899) |
| Firefox          |  115,814 (34,262/81,552) |    92,651 (30,026/62625) | 23,163 (4,236/18,927) |
| Thunderbird      |   32,551 (11,631/20,920) |   26,040 (10,046/15,994) |   6,511 (1,585/4,926) |
| Eclipse Platform |   85,156 (19,845/65,311) |   68,124 (17,518/50,606) | 17,032 (2,327/14,705) |
| JDT              |   45,296 (10,127/35,169) |    36,236 (8,859/27,377) |   9,060 (1,268/7,792) |
| Spark            |    19,766 (2,813/16,953) |    15,812 (2,425/13,387) |     3,972 (388/3,566) |
| Hadoop           |       10,624 (827/9,797) |        8,499 (656/7,843) |     2,125 (171/1,954) |
| MapReduce        |        5,608 (880/4,728) |        4,486 (779/3,707) |     1,122 (101/1,021) |
| HDFS             |     10,676 (1,530/9,146) |      8,540 (1,398/7,142) |     2,136 (132/2,004) |
| HBase            |      16,594 (455/16,139) |      13,275 (384/12,891) |      3,319 (71/3,248) |
| Cassandra        |    11,950 (1,261/10,689) |        9,560 (962/8,598) |     2,390 (299/2,091) |
| Mesos            |        6,564 (615/5,949) |        5,251 (535/4,716) |      1,313 (80/1,233) |


**Links to more duplicate bug report datasets**
+ [[MSR'14]: Generating Duplicate Bug Datasets](https://doi.org/10.5281/zenodo.1144098)
+ [[MSR'17]: Rediscovery Datasets: Connecting Duplicate Reports](https://zenodo.org/record/400614)

**Publications**
+ [**ICSE'07**] Per Runeson, Magnus Alexandersson, Oskar Nyholm. [Detection of Duplicate Defect Reports Using Natural Language Processing](https://ieeexplore.ieee.org/document/4222611/), *International Conference on Software Engineering (ICSE)*, 2007.
+ [**ICSE'10**] Chengnian Sun, David Lo, Xiaoyin Wang, Jing Jiang, Siau-Cheng Khoo. [A Discriminative Model Approach for Accurate Duplicate Bug Report Retrieval](https://ieeexplore.ieee.org/document/6062072/), *International Conference on Software Engineering (ICSE)*, 2010.
+ [**ASE'11**] Chengnian Sun, David Lo, Siau-Cheng Khoo, Jing Jiang. [Towards More Accurate Retrieval of Duplicate Bug Reports](https://ieeexplore.ieee.org/document/6100061), *IEEE/ACM International Conference on Automated Software Engineering (ASE)*, 2011.
+ [**ASE'12**] Anh Tuan Nguyen, Tung Thanh Nguyen, Tien N. Nguyen, David Lo, Chengnian Sun. [Duplicate Bug Report Detection With a Combination of Information Retrieval and Topic Modeling](http://www.comp.nus.edu.sg/~specmine/suncn/papers/ase12.pdf), *IEEE/ACM International Conference on Automated Software Engineering (ASE)*, 2012.
+ [**ISSRE'16**] Xinli Yang, David Lo, Xin Xia, Lingfeng Bao, Jianling Sun. [Combining Word Embedding with Information Retrieval to Recommend Similar Bug Reports](https://ieeexplore.ieee.org/document/7774514/), *IEEE International Symposium on Software Reliability Engineering (ISSRE)*, 2016.
+ [**TSE'17**] Mohamed Sami Rakha, Cor-Paul Bezemer, Ahmed E. Hassan. [Revisiting the Performance Evaluation of Automated Approaches for the Retrieval of Duplicate Issue Reports](https://ieeexplore.ieee.org/document/8048025/), *IEEE Transactions on Software Engineering (TSE)*, 2017.
+ [**ICSE'18**] Amar Budhiraja, Raghu Reddy, Manish Shrivastava. [LWE: LDA Refined Word Embeddings for Duplicate Bug Report Detection](https://dl.acm.org/citation.cfm?id=3195078), *International Conference on Software Engineering (ICSE)*, 2018.
+ [**ICSE'18**] Amar Budhiraja, Kartik Dutta, Raghu Reddy, Manish Shrivastava. [DWEN: Deep Word Embedding Network for Duplicate Bug Report Detection in Software Repositories](https://dl.acm.org/citation.cfm?id=3183440.3195092), *International Conference on Software Engineering (ICSE)*, 2018.

### 2. Bug localization

Bug localization is a process to map a bug report to the corresponding buggy source file. This dataset contains bug reports, commit history, and API descriptions of six open source Java projects including Eclipse Platform UI, SWT, JDT, AspectJ, Birt, and Tomcat. The dataset is currently available [here](http://openscience.us/repo/issues/bugfiles.html).

| Project  | Timespan                | #Bugs mapped |
| :-------- | -----------------------: | --------------: |
| AspectJ  | 2002-03-13 ~ 2014-01-10 | 593            |
| Birt     | 2005-06-14 ~ 2013-12-19 | 4,178           |
| Eclipse  | 2001-10-10 ~ 2014-01-17 | 6,495           |
| JDT      | 2001-10-10 ~ 2014-01-14 | 6,274           |
| SWT      | 2002-02-19 ~ 2014-01-17 | 4,151           |
| Tomcat   | 2002-07-06 ~ 2014-01-18 | 1,056           | 

**Publications**

+ [**FSE'14**] Xin Ye, Razvan C. Bunescu, Chang Liu. [Learning to Rank Relevant Files for Bug Reports using Domain Knowledge](http://ace.cs.ohiou.edu/~razvan/papers/fse14.pdf), *ACM SIGSOFT International Symposium on Foundations of Software Engineering (FSE)*, 2014.
+ [**TSE'16**] Xin Ye, Razvan C. Bunescu, Chang Liu. [Mapping Bug Reports to Relevant Files: A Ranking Model, a Fine-Grained Benchmark, and Feature Evaluation](https://ieeexplore.ieee.org/document/7270328/), *IEEE Transactions on Software Engineering (TSE)*, 2016.
+ [**ICSE'16**] Xin Ye, Hui Shen, Xiao Ma, Razvan C. Bunescu, Chang Liu．[From Word Embeddings to Document Similarities for Improved Information Retrieval in Software Engineering](https://ieeexplore.ieee.org/document/7886921/), *International Conference on Software Engineering (ICSE)*, 2016.
+ [**IJCAI'16**] Xuan Huo, Ming Li, Zhi-Hua Zhou. [Learning Unified Features from Natural and Programming Languages for Locating Buggy Source Code](https://www.ijcai.org/Proceedings/16/Papers/230.pdf), *International Joint Conference on Artificial Intelligence (IJCAI)*, 2016.
+ [**IJCAI'17**] Xuan Huo, Ming Li. [Enhancing the Unified Features to Locate Buggy Files by Exploiting the Sequential Nature of Source Code](https://www.ijcai.org/proceedings/2017/0265.pdf), *International Joint Conference on Artificial Intelligence (IJCAI)*, 2017.


### 3. Bug triaging

Given a software bug report, bug triaging is the process to identify an appropriate developer who could fix the bug. Automatic bug triaging algorithm can be formulated as a classification problem, which takes the bug title and description as the input, mapping it to one of the available developers (class labels). The dataset is currently available [here](http://bugtriage.mybluemix.net/).

| Project      | \#Bugs  | \#Bugs for classifier |
| :------------ | -------: | ---------------------: |
| Chromium     | 383,104 | 118,643               |
| Mozilla Core | 314,388 | 128,215               |
| Firefox      | 162,307 | 24,214                |

**Publications**

+ Senthil Mani, Anush Sankaran, Rahul Aralikatte. [BugTriage: Exploring the Effectiveness of Deep Learning for Bug Triaging](http://bugtriage.mybluemix.net/paper/DeepTriage.pdf), *Arxiv*, 2018.


### 4. Bug-fixing time estimation
The bug report datasets hosted in this repository contain detailed information about bug fixing time tracking, which can thus be used for research on bug-fixing time estimation.

**Publications**

+ [**ICSE'13**] Hongyu Zhang, Liang Gong, Steven Versteeg. [Predicting Bug-fixing Time: an Empirical Study of Commercial Software Projects](https://www.researchgate.net/publication/261314373_Predicting_bug-fixing_time_An_empirical_study_of_commercial_software_projects), *International Conference on Software Engineering (ICSE)*, 2013.
+ [**MSR'11**] Pamela Bhattacharya, Iulian Neamtiu. [Bug-fix Time Prediction Models: Can We Do Better?](http://alumni.cs.ucr.edu/~pamelab/bugfixtime.pdf), *International Working Conference on Mining Software Repositories (MSR)*, 2011.

### 5. Bug information mining
Lamkanfi et al. [MSR'13] contributed a dataset with over 200.000 reported bugs extracted from the Eclipse and Mozilla projects. Besides providing a single snapshot of a bug report, they also include all the incremental modifications as performed during the lifetime of the bug report. The dataset is currently available [here](https://github.com/ansymo/msr2013-bug_dataset).

| Project          | \#Components | \#Bugs |
| :---------------- | ------------: | ------: |
| Eclipse Platform | 22           | 24,775 |
| JDT              | 6            | 10,814 |
| CDT              | 20           | 5,640  |
| GEF              | 5            | 5,655  |
| Mozilla Core     | 137          | 74,292 |
| Firefox          | 47           | 69,879 |
| Thunderbird      | 23           | 19,237 |
| Bugzilla         | 21           | 4,616  |

**Publications**

+ [**MSR'13**] Ahmed Lamkanfi and Javier Perez and Serge Demeyer. The Eclipse and Mozilla Defect Tracking Dataset: a Genuine Dataset for Mining Bug Information. *International Working Conference on Mining Software Repositories (MSR)*, 2013.

# License
The datasets are freely available for research purposes.

[LogPAI Team](https://github.com/orgs/logpai/people), 2018.
