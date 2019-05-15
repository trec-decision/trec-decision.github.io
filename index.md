# WEBSITE UNDER DEVELOPMENT

## Track Overview
Search engine results underpin many consequential decision making tasks. Examples include
people using search technologies to seek health advice online, or time-pressured clinicians
relying on search results to decide upon the best treatment/diagnosis/test for a patient.

A key problem when using search engines in order to complete such decision making tasks, is
whether users are able to discern authoritative from unreliable information and correct from
incorrect information. This problem is further exacerbated when the search occurs within
uncontrolled data collections, such as the web, where information can be unreliable, generally
misleading, too technical, and can lead to unfounded escalations (White&Horvitz, 2009).
Information from search engine results can significantly influence decisions, and research
shows that increasing the amount of incorrect information about a topic presented in a SERP
can impel users to take incorrect decisions (Pogacar et al, 2017). As noted in the SWIRL III
report (Culpepper et al., 2018), decision making with search engines is poorly understood, and
likewise, evaluation measures for these search tasks need to be developed and improved.

## Goals of the Track

This track aims to 
* Provide a venue for research on retrieval methods that promote better
decision making with search engines, and
* Develop new online and offline evaluation
methods to predict the decision making quality induced by search results.

## Task
The track is planned over multiple years, with data and resources created in one year flowing
into the next year. We plan for the track to run for at least 3 years.

#### Year 1 (2019)
Participants devise search technologies that promote correct information over incorrect information, with the assumption that correct information can better lead people to make correct decisions.

Note: this task is more than simply a new definition of what is relevant. There are 3 types of results: correct and relevant, incorrect, and non-relevant. It is important that search results avoid containing incorrect results, and
ranking non-relevant results above incorrect is preferred.

Evaluation measures will consider relevance beyond topicality, including correctness of information and crediablity. 

Year 1 task summary: Given a data collection and a set of topics (portraied as questions, see topics for more information), your task is to return relevant and correct information that will help searchers make correct decisions. 

Following the year 1 assessment, the organizers will recruit test subjects to perform a decision
making task using a selection of the year 1 runs. That is, test subjects will be given a fixed result list (selected from the participating teams submitted runs) and a decision task. We will collect user interaction data as well as the users' decisions.

#### Year 2 (2020)
Given a query, a document ranking (results list) and interaction data of real users (collected right after year 1),
predict the decisions users will take at the end of the search process, along with their confidence when taking such decisions. This simulates an online evaluation process.

#### Year 3 (2021)
Given a query, a document ranking (results list), and assessments, predict the decision the user will take at the end of the search process (along with the confidence expressed by the user with respect to their decision). 
This simulates an offline evaluation process.


## Data
The Track plans to focus on topics within the consumer health search domain (people seeking
health advice online) to form user stories (search topics). Consumer health search represents
an ideal prototypical example of the consequential decisions that we want search engines to
correctly support. 


#### Search Topics
TBA


#### Collection (documents set)
TBA


## Submission of Runs
#### Format
Submission format will follow the standard TREC run format. The submission format when submitting ranked results is as follows: 

``qid Q0 docno rank score tag``

where:

* ``qid``:  the topic number.
* ``Q0``: unused and should always be Q0.
* ``docno``: the official document id number returned by your system for the topic qid.
* ``rank``:  the rank the document is retrieved,
* ``score``: the score (integer or floating point) that generated the ranking. The score must be in descending (non-increasing) order. The score is important to handle tied scores. (`trec_eval` sorts documents the the scores values and not your ranks values).
* ``tag``: a tag that uniquley identifies your group AND the method you used to produce the run. Each run should have a different tag. 

The fields should be spectated with a whitespace. The width of the columns in the format is not important, but it is important to include all columns and have some amount of white space between the columns.

Example run is shown below: 

```
1 Q0 clueweb12-1018wb-57-17875 1 14.8928003311 myGroupNameMyMethodName
1 Q0 clueweb12-1311wb-18-06089 2 14.7590999603 myGroupNameMyMethodName
1 Q0 clueweb12-1113wb-13-13513 3 14.5707998276 myGroupNameMyMethodName
1 Q0 clueweb12-1200wb-47-01250 4 14.5642995834 myGroupNameMyMethodName
1 Q0 clueweb12-0205wb-37-09270 5 14.3723001481 myGroupNameMyMethodName
...
```

#### Number of Submission

Each group is allowed up to 4 submissions.



## Assessing guidelines 
NIST assessors will judge documents in three categories:

* **Relevancy:** whether the document is relevant to the topic.
* **Treatment Efficacy:** whether the document contain correct information regarding the topic's treatment.  
* **Credibility:** whether the document is considered credible by the assessor.  


## Evaluation of Runs
We anticipate runs to be evaluated using some of the evaluation measures suggested by Lioma et al. (ICTIR'17), as well as traditional relevancy evaluation measures.
More details will be provided later. 


## Schedule  
#### 2019
* (TBA) Final guidelines available
* (TBA) Availability of Topics/Collection
* (TBA) Runs due
* (TBA) Results returned
* (TBA) Notebook paper due
* (TBA) TREC Conference
* (TBA) Final report due


## Organizers

#### [Christina Lioma, University of Copenhagen](https://di.ku.dk/Ansatte/?pure=en/persons/424829)
#### [Mark Smucker, University of Waterloo](http://mansci.uwaterloo.ca/~msmucker/)
#### [Guido Zuccon, University of Queensland](http://www.zuccon.net/)


## Contact
For more information or to ask questions, join the [google groups](https://groups.google.com/forum/#!forum/trec-decision-track)
