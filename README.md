# HCE Data 100 Curriculum Dev (Project 1)

Project 1 (Spring 2019) is a potential point of intervention where we can introduce a dataset from the Data Engineers. The current project uses a dataset containing all of the restaurants in the San Francisco/Bay Area, where students familiarize themselves with basic Pandas commands. Replacing this dataset with one that can allow for HCE tools and questions to be posed can allow for this project to enable students to learn how to use Pandas while emphasizing the context and meaning of the dataset being used.

## 💻 Project Goal

Project 1 as it stands is a fully functional, well thought out piece of educational material. The core aim of both versions of Project 1 (the already existing project and this proposed replacement) is to familiarize students with basic Pandas commands while emphasizing the context and meaning of the dataset of interest. The priority of the project should be placed in educating students of the relevant technical skills. The HCE team views this replacement as an opportunity to expand potential learning beyond its technical requirements: to educate students about the racial disparities in educational outcome in California, and ultimately to guide students to recognize data sets as connected to and indicative of larger discourses with real world implications. The project offers a unique method of viewing perspectives of an on-going national debate regarding the legitimacy of affirmative action on college campuses.

We have chosen to replace the San Francisco restaurant health score data set with a California Department of Education data set which has school name, zip codes, associated school data, and their respective ACT and SAT scores. 


## 📋 Project Outline

### Similarities With The Original Project

**Question Directory (Tracking Changes):**

  ✅ : Original question that is retained

  ➡️ : New number of retained question

  ❌ : Question removed
  

**Question 1.**

  1a ❌ | 1b ❌ | 1c ➡️ 1a | 1d ➡️ 1b | 1e ➡️ 1c

**Question 2.**

  2a ✅ | 2b ✅

**Question 3.**

  3a ✅ | 3b ➡️ 3b & 3e | 3c ✅ | 3d ❌ | 3e ❌ | 3f ✅

**Question 4.**

  4a ✅ | 4b ✅ | 4c ✅ | 4d ✅ | 4e ✅ | 4f ✅ | 4g ✅ | 4h ✅ | 4i ✅

**Question 5.**

  5a ✅ | 5b ➡️ 6c

**Question 6.**

  6a ✅ | 6b ✅ | 6c ❌

**Question 7.**

  7a ➡️ 5b | 7b ➡️ 5c | 7c ➡️ 5d

**Question 8.**

  8a ❌ | 8b ➡️ 7c | 8c ➡️ 7d | 8d ❌ | 8e ➡️ 7e


**Total:**

7 questions missing
  - 1a and 1b are terminal operations.
  - Data is too clean to apply questions 3d and 3e.
  - No time information for 6c.

28 questions maintained

6 questions added (6d, 7a, 7b, 8a, 8b, 8c)
  - Not shown in the directory above.


### Differences From The Original Project

The missing values in the project replacement are more minimal than in the original data set. Every school in the directory is properly labeled and has an associated zip code that are correct. Significantly, the school directory dataset was missing SOC type features for Some schools also have missing emails and phone numbers, though these features are much less significant. The school directory data set was left joined with the ACT scores data set, producing many missing values and for the purposes of this project, leaving the data set we have chosen with many rows that are meaningless. These missing values still provide an opportunity for students to clean a data set, and practice an important part of the data lifecycle. Indeed, in the real world, these sorts of missing values generated by joining differing data sets is perhaps more common.

### School Directory & ACT Scores

The original project explores two datasets, restaurants and inspections, that the course developers have used to teach students to work with data at different levels of granularity. In order to deliver a similar level of complexity, the team has joined the school directory data with average ACT Scores data. The resulting table has granularity at the individual school level, and the table corresponds to the restaurants table in the original project.

### Demographics

The demographics table is organized so that each row corresponds to a given ethnicity and gender (ex. male Hispanic, female White). Although ACT Scores and Inspection Scores share similar data characteristics, the ACT Scores table has identical granularity as the school directory table. The demographics table was therefore chosen as a second table that replaces the inspections table in the original project.

### Question 8

Question 8 of the project is composed of (three) free response questions intended to motivate students to think about the context and background of the data they're dealing with. They are given the opportunity to answer questions such as why are they seeing the differences that they have observed in the data and what are some interventions that they can think of to work towards remedying this issue. By posing these questions we expect students to explore the implications of analyzing and taking conclusions away from real world data and how data science should be combined with human context for interpretation.

## 📊 Data

Public schools and districts data: https://www.cde.ca.gov/ds/si/ds/pubschls.asp

School enrollment (demographics) data: https://www.cde.ca.gov/ds/sd/sd/filesenr.asp

Postsecondary preparedness (ACT scores) data: https://www.cde.ca.gov/ds/sp/ai/

*Note that original data have been manipulated within ipynb to fit project goals.*

  - Joined school directory data and ACT scores data (left join on school directory). The resulting table partially contains null values       in columns corresponding to ACT scores as a result (for example, a given school may not necessarily be a high school). 

## 📚 Resources

Brookings Institute article regarding racial differences in educational outcomes: https://www.brookings.edu/articles/unequal-opportunity-race-and-education/

Article on Chancellor Christ's Diversity Initiatives: https://alumni.berkeley.edu/california-magazine/spring-2019/chancellors-letter-diversity-initiatives

Data 100 Jupyter Notebook edit guides: https://docs.google.com/document/d/1PxhuVf84c_CQu8CgYhHgBw4ptDbX7tc7HgAIyhAfgy8/edit
