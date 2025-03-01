Fake News Detection in Dravidian Languages-DravidianLangTech@NAACL 2025
The proliferation of online social media over the past few years has significantly streamlined the ways in which individuals are able to communicate with one another. Users of social media platforms are able to exchange information, communicate and maintain awareness of current events. On the other hand, much of the recent information that has been emerging on social media is false and, in some instances, is intended to mislead users. This type of content is commonly referred to as fake news. Any false or misleading information that appears as original news is considered as fake news. 

 

There are two subtasks:

Task 1: The goal of this task is to classify a given social media text into original or fake. The sources of data are various social-media platforms such as Twitter, Facebook etc. Given a social media post, the objective of the shared task is to classify it into either fake or original news. For example, the following two posts belong to fake and original categories, respectively. 

Task: This is a comment / post level classification task. Given a Youtube comment, the systems submitted by the participants should classify it into original or fake news. To download the data and participate, go to the Participate tab

Task 2: The Fake News Detection from Malayalam News (FakeDetect-Malayalam) shared task provides a platform for researchers to address the pressing challenge of identifying and flagging fake news within the realm of Malayalam-language news articles. In an age of information overload, accurate detection of misinformation is crucial for fostering trustworthy communication. The core objective of the FakeDetect-Malayalam shared task is to encourage participants to develop effective models capable of accurately detecting and classifying fake news articles in the Malayalam language into different categories. Here, we considered five fake categories - False, Half True, Mostly False, Partly False and Mostly True

Task: This is a comment / post level classification task. Given a comment/news, the systems submitted by the participants should classify it into the five classes mentioned above. To download the data and participate, go to the Participate tab 

Following are some general guidelines to keep in mind while submitting the working notes.

Basic sanity check for grammatical errors and reported results
Papers should have sufficient information for reproducing the mentioned results- Papers should follow the appropriate style (We will use NAACL 2025 style: details below)
Check the papers for text reuse / Plagiarism. This includes self-plagiarism as well. We would like to stress this point as EACL is quite strict about it. Any paper found to have plagiarized content should be rejected without further consideration.
Please ensure the author names do not have any salutations like Dr., Prof., etc in the final version




Submit separate zip files for each task. Submission should be a zip file with your team name containing tsv files  - 'teamname_task_run.tsv'  e.g. the zip file may contain teamname_task2_run.tsv. The submission will be evaluated with macro average F1-score.

Submission Links:

Task 1: https://forms.gle/TT2FGPmf3xR7erCW9
Task 2: https://forms.gle/5KaKqvce8bf34B4F6


Submission should be a .zip file with your team name containing .csv files for individual lanaguge or task:
[Create Zip File: Team_name.zip]
Include CSV Files For Each Language
[Single Submission: Team_name_Language_Task.csv]
Examples:
VEL_Tamil_task1.csv
VEL_Tamil_task2.csv
[Multiple Submissions: Team_name_Language_Task_Runs.csv] (max. 3 submissions in each language are allowed)
Examples:
VEL_Tamil_task1_run1.csv
VEL_Tamil_task1_run2.csv
VEL_Tamil_task2_run1.csv
VEL_Tamil_task2_run2.csv
(Please note that if there is any wrong submission or wrong format will not be considered).
The submission will be evaluated with a macro average F1-score.
Column header must present for the prediction CSV files same as the test set:

CSV File Structure: The prediction.csv file must include two columns:
Id
Labels
Ensure that the column headers are exactly as mentioned in the given test dataset.
Overleaf Template:
TBA

Working notes Submission link
TBA

 
The classification system’s performance will be measured in terms of macro-averaged Precision, macro-averaged Recall, and macro-averaged F1-Score across all the classes. Participants are encouraged to check their system with the sklearn classification report

https://scikit-learn.org/stable/modules/generated/sklearn.metrics.classification_report.html
 

If you are using our dataset, please cite the below papers

 

@inproceedings{subramanian2024overview,
  title={Overview of the Second Shared Task on Fake News Detection in Dravidian Languages: DravidianLangTech@ EACL 2024},
  author={Subramanian, Malliga and Chakravarthi, Bharathi Raja and Shanmugavadivel, Kogilavani and Pandiyan, Santhiya and Kumaresan, Prasanna Kumar and Palani, Balasubramanian and Premjith, B and Vanaja, K and Mithunja, S and Devika, K and others},
  booktitle={Proceedings of the Fourth Workshop on Speech, Vision, and Language Technologies for Dravidian Languages},
  pages={71--78},
  year={2024}
}

@inproceedings{devika2024dataset,
  title={From Dataset to Detection: A Comprehensive Approach to Combating Malayalam Fake News},
  author={Devika, K and Haripriya, B and Vigneshwar, E and Premjith, B and Chakravarthi, Bharathi Raja and others},
  booktitle={Proceedings of the Fourth Workshop on Speech, Vision, and Language Technologies for Dravidian Languages},
  pages={16--23},
  year={2024}
}

@inproceedings{fakenews-2023-overview,
    title = "Overview of the Shared Task on Fake News Detection from Social Media Text",

    author = "Subramanian, Malliga and 

      Chakravarthi, Bharathi Raja and

      Shanmugavadivel, Kogilavani and

      Pandiyan, Santhiya and

      Kumaresan, Prasanna Kumar and

      Palani, Balasubramanian and

      Singh, Muskaan and

      Raja, Sandhiya and

      Vanaja and

      S, Mithunajha",      

    booktitle = "Proceedings of the Third Workshop on Speech and Language Technologies for Dravidian Languages",

    month = September,

    year = "2023",

    address = "Varna, Bulgaria ",

    publisher = "Recent Advances in Natural Language Processing",

}

 