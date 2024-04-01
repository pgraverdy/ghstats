---
title: "Github Repository Statistics for ORGANIZATION/PROJECT_NAME"
geometry: margin=2cm
output: pdf_document
---


# Introduction

## Summary

- **Project name**: PROJECT_NAME
- **Organization**: ORGANIZATION
- **URL**: PROJECT_URL
- **Report date**: REPORT_DATE


## Scope of the report

This report has been automatically generated using the gh-stats Notebook available at GHSTATS_URL.

The main objective of this report is to provide some factual information about the origin of the contributions in an Open Source project when discussing about IP attributions between contributors (when filing out authorship attribution declarations). 


This information is provided as is, and mostly reports about the commits of the different contributors. The actual value/impact of the contributions of a contributor, especially in a scientific project, can be unrelated to the number of commits performed or the number of lines written. For example:

- Rewrttting a core algorithm so that it can scale on multi-core processor can be a key contribution in a few lines of codes  

- Generating a UI with some code-generation tools, or reformating some code may generate/modify many lines, yet not qualify as a key contribution


Therefore, discussion between contributors should still take place, and a common agreement found about the importance of the different contributions.



## Technical notes on the statistics


- This report uses metrics/information from the Github project mentionned above, as well as Git statistics. Unless mentionned otherwise, all the statistics are based on (i) all the commits of the project (all branches) when providing full-project statistics, and (ii) on the latest commit on the `main/master` branch at the time of the report's generation when providing latest-code statistics. 

- The report is only on the Github repository mentionned above. If one software is split on multiple repositories (e.g., back-end and frond-end of a Web application), it is up to the contributors to decide how to merge the individual reports. 

- When providing full-project statistics on commit or LoC (Line of Code), we consider all the true commits of the repository (excluding merge requet commits). This means all commits on all the branches, even if not merged into the main/master branch.

- When providing latest-code statistics, this relates to the lastest code on the main/master branch cloned from Github (publicly available).

- We consider the "author" of the commit, and not the committer (another person may commit on behalf of a person).


Some additional information is provided as input of this report in the Annexes

- A list of commiter's names that should be merged (when a single person has commited code under different names on Github).

- A list of employers for the different contributors (when know) in order to do the IP distribution between different organizations, when useful.


## Repository configuration

### Main contributors

On large projects, many contributors may have only very marginal contributions (e.g., correcting a typo in the documentation). On the other side of the spectrum, a few contributors may be the source of most of the work/innovation in the project. For readability purposes, some statistics are only be provided for a list of main contributors.

The main contributors for this repository have been defined as:

MAIN_CONTRIBUTORS_TABLE

### Core folders

Within the GH repository, the files with the key contributions (scientific and technological) to the project may be located in specific folders, while other folders may be less relevant (e.g., datasets, documentation, smample code, ...). When generating the report, a list of core folders is defined. Some statistics are provided for all files in the repository, as well as for the files in the core folders.

- For the commits, we consider as "Core commit" a commit where at least one of the modified files is in the core folder.

- As a limitation to this folder appraoch, the files at the root of the repository are not considered for Core statistics.


The core folders for this repository have been defined as:

CORE_FOLDERS_TABLE


# Full-project Statistics

This section provides information on the contributions during the whole project lifetime. Hence, for projects with a long history and many versions, older contributions may have been rewritten or removed over time (but may still be important and/or significant to explain the state of the current project.


## Global statistics

- Number of commits (including merge) : NUMBER_COMMITS_WITH_MERGE
- Number of merge : NUMBER_MERGE
- Number of true commits (single parent) : NUMBER_COMMITS
- Number of contributors : NUMBER_CONTRIBUTORS
- Number of main contributors : NUMBER_MAIN_CONTRIBUTORS


- Latest commit date : LATEST_COMMIT_DATE
- Latest commit sha : LATEST_COMMIT_SHA
- Local repository commit date: LOCAL_REPO_COMMIT_DATE
- Local repository commit sha : LOCAL_REPO_COMMIT_SHA

## Main contributors statistics

In the following charts, commits and LoC statistics are provided for the main contributors (all the other contributors are merged in "Others"). 


![](CHART_MAIN_CONTRIBUTORS_COMMITS){width=50%} ![](CHART_MAIN_CONTRIBUTORS_LOC){width=50%}


Same data as pie charts for the percentage


![](PIE_FULL_COMMITS_MAIN_CONTRIBUTORS){width=50%} ![](PIE_FULL_LOC_MAIN_CONTRIBUTORS){width=50%}
  

The details of the statistics is given in the table below


![](TABLE_CONTRIBUTORS_STATS_FULL){width=50%} 


## Affiliation statistics

In the following tables and charts, commits and LoC statistics are provided for each known affiliation (check the relevant table in Annex). Note that one contributor may have different affiliations over time.


![](CHART_COMMITS_AFFILIATION){width=50%} ![](CHART_LOC_AFFILIATION){width=50%}


Same data as pie charts for the percentage


![](PIE_COMMITS_AFFILIATION){width=50%} ![](PIE_LOC_AFFILIATION){width=50%}


The details of the statistics is given in the table below


![](TABLE_AFFILIATIONS_STATS_FULL_WITH_CORE){width=80%} 


## Analysis


THIS SECTION SHOULD BE COMPLETED IN THE MARKDOWN TO PROVIDE EXPLANATIONS ON THE TABLES AND GRAPHS ABOVE.

.


.


.


.


.


.



# Latest-code Statistics


In this section, statistics on the latest code in the main/master branch are provided using Git blame.


## Main contributors statistics


![](CHART_LATEST_COMMITS_MAIN_CONTRIBUTORS){width=50%} ![](CHART_LATEST_LOC_MAIN_CONTRIBUTORS){width=50%}


![](PIE_LATEST_COMMITS_MAIN_CONTRIBUTORS){width=50%} ![](PIE_LATEST_LOC_MAIN_CONTRIBUTORS){width=50%}


The details of the statistics is given in the table below


![](TABLE_CONTRIBUTORS_STATS_LATEST){width=50%} 


## Affiliation statistics


![](CHART_LATEST_COMMITS_AFFILIATION){width=50%} ![](CHART_LATEST_LOC_AFFILIATION){width=50%}

The details of the statistics is given in the table below

![](TABLE_LATEST_INFO_AFFILIATION){width=50%} 


## Analysis

THIS SECTION SHOULD BE COMPLETED IN THE MARKDOWN TO PROVIDE EXPLANATIONS ON THE TABLES AND GRAPHS ABOVE.


.


.


.


.


.


.

# Conclusion

THIS SECTION SHOULD BE COMPLETED IN THE MARKDOWN TO PROVIDE EXPLANATIONS ON THE TABLES AND GRAPHS ABOVE.

Questions:

- Are the main contributors the only contributors to contact for the authorship attribution (i.e., the pther ones have no real contribution, or not significant enough)?

- Are some of the contributors (main or others) not relevant anymore for the current (latest) version?

- What are the authorship attribution percentage for the contributors?


.


.


.


.


.


.


# Annexes

## Contributors account merging

Due to different configurations on different computers (or changes over time), the same user may commit code under different names. To properly attribute commits/statistics to individual contributors, a merging table can be provided when generating this report to rename contributors.


The following merging table as been used in this report:

ACCOUNT_MERGING_TABLE


## Contributors' affiliation

For this report, the following affiliations have been used (contributor, affiliaton, period):

ACCOUNT_AFFILIATION_TABLE
