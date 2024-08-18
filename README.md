# Random500Coded-noFP.csv

* Figure 1  
  * Use `questionCreationDate` to get number of questions per year  
* Table 1  
  * Question Popularity  
    * Score \- `questionScore`  
    * Answer \- `AnswerCount`  
    * Comment \- `CommentCount`  
    * View \- `questionViewCount`  
    * Popularity \- As described in Section 4.1.2  
* Table 2  
  * Answer Popularity  
    * Score \- `answerScore`  
    * Comment \- `answerCommentCount`  
    * Popularity \- As described in Section 4.1.2  
* Figure 2  
  * Use `code` to get the name of the subtheme  
    * Find percentage of each subtheme  
  * Similar for major theme, except add the subthemes (or make a dict of which subthemes correspond to major themes)  
* Table 3  
  * Can use `Random500Coded-Major-noFP.csv` or `Random500Coded-noFP.csv`  
    * Use `AnswerCount` to get num answers for each theme  
    * These datasets do *not* have duplicates, so increment question by 1 for each row for the corresponding code/label  
    * Succes status  
      * `AcceptedAnswerId` not blank means *Successful*  
      * `AcceptedAnswerId` AND `AnswerCount` \> 0 means *Ordinary*  
      * `AnswerCount` \== 0 means *Unsuccessful*

# AllSOAnswerData.csv

# AllSOQuestionData.csv

* The above 2 files have about a million random questions and answers  
* Used for normalization  
* Question Popularity  
  * Score \- `Score`  
  * Answer \- `AnswerCount`  
  * Comment \- `CommentCount`  
  * View \- `viewCount`  
  * Popularity \- As described in Section 4.1.2  
* Answer Popularity  
  * Score \- `Score`  
  * Comment \- `CommentCount`  
  * Popularity \- As described in Section 4.1.2  
* Table 3, 4  
  * Using above 3, get popularity metrics for each theme  
    * See paper for more details

# Random500Coded-Major-noFP.csv

* Same data as `Random500Coded-noFP.csv` except these have the major theme labels instead of the subtheme labels in the column for `code`  
* Used for Figure 4, 5; Table 5  
  * Although `Random500Coded-noFP.csv` could’ve been used…

# Random500HWWO-noFP.csv

* Table 6  
  *  Uner column `HWWO`  
    * Labelled as `how`, `what`, `why`, `other`

# Codes

'Specifications': \['api', 'hr', 'os', 'lu'\],   
'Remote': \['wireless', 'cpmr'\],  
'Connections': \['internet', 'wpi', 'sc'\],  
'Coordinates': \['position', 'orientation'\],  
'Moving': \['mp', 'obstacles', 'mapping', 'SLAM'\],  
'Actuator': \['ik', 'hc', 'wc', 'mc', 'balance'\],  
'Programming': \['pointers', 'dt', 'overflow', 'list'\],  
'Error': \['li', 'bf'\],  
'Timing': \['timing', 'multithreading', 'rg'\],  
'Incoming': \['cameras', 'vision', 'line tracking', 'sensors'\],  
'Other' : \['gs', 'bp', 'repeat', 'decoupling', 'install', 'ra', 'ros', 'rn', 'dl', 'rl', 'dc', 'distance'\]