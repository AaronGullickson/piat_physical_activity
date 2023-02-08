# Data Source Description

The data we will use for this research project come from the [Youth Risk Behaviorial Surveillance System](https://www.cdc.gov/healthyyouth/data/yrbs/index.htm) (YRBSS) data collected by the Centers for Disease Control and Prevention. The YRBSS is actual a collection of surveys that are collected at the state and sometimes school district level that help to monitor a variety of risk factors among adolescents like drug use, sexual behavior, diet, and physical activity. Not all states participate and not all states ask the same questions. For this research project we will be looking at 2019 YRBSS data for the following states: Arizona, Arkansas, Colorado, Hawaii, Idaho, Nevada, New Jersey, North Carolina, North Dakota, Pennsylvania, Rhode Island, Tennessee, Vermont, Virginia, and Wisconsin. We look at this subset of states because these states asked all of the questions relevant for analysis.


From the full data, I have extracted and recoded the following variables for our use as an analytical dataset. To load this dataset in R, you just need to run the setup code chunk in the full_report.Rmd R Markdown document. The name of the dataset in R is `yrbs`. 

* **state**: The name of the state. This is for informational purposes, but you will likely not need to use it.
* **grades**: A score based on the self-reported grades of the student. Students responded to the prompts of "Mostly A's", "Mostly B's", "Mostly C's", "Mostly D's", and "Mostly F's". I have coded those responses numerically to the corresponding GPA value. So students who said "Mostly A's" receive a 4, students who said "Mostly B's" receive a 3, etc. This is the key dependent variable.
* **physical_act**: The number of days in the last week that the student reported at least 60 minutes of physical activity. This is the key independent variable.
* **gender**: The student's self-reported gender recorded as "Male" or "Female." This is the key contextual variable.
* **race**: The student's self-reported race recorded as White, Latino, Black, Asian, American Indian, Pacific Islander, or Multiple Races.
* **school_grade**: The student's grade in school.
* **hungry**: Students were asked how often over the previous 30 days they went hungry because there was not enough food in their home. They could respond "Never", "Rarely", "Sometimes", "Most of the time", or "Always". The YRBSS lacks detailed information on the socioeconomic background of students, so this variable helps proxy for socioeconomic status, among other things.
* **felt_sad**: Students were asked if, over the past 12 months, they ever felt sad or hopeless almost every day for at least two weeks in a row that stopped them from doing usual activities.

