# Starbucks JIMOTO Frappuccino dataset (2021)

This dataset is a binary matrix (incidence matrix) of an online survey in the csv format. 
During the summer of 2021, Starbucks Japan sold 47 types of Frappuccino as local specials of each prefecture in Japan. 
We obtained 329 valid responses indicating 5 types of Frappuccino that each respondent wanted to try (i.e., a 329-by-47 matrix with each row-marginal equals to 5).


### csv
- incidence\_matrix\_en.csv: Incidence matrix of the survey (prefecture names in alphabet)
- incidence\_matrix\_ja.csv: Incidence matrix of the survey (prefecture names in Japanese kanji)
- categories\_frapp.csv: Category (see below) of each Frappuccino
- demographic.csv: Demographic information (see below) of each respondent

### graphml
- starbuck_jimoto_frappuccino.graphml: Graph that contains all information in the csv files.


## Background and details
For the 25th anniversary of Starbucks Japan, 47 types of Frappuccino featuring each prefecture in Japan were sold from June 30 to August 3 in 2021. 
This campaign was titled *JIMOTO Frappuccino*, where *jimoto* is a Japanese word meaning "local." 
The word also implies "home town." 
For example, because these prefectures are major producers of mandarin oranges in Japan, the featured Frappuccino types in Shizuoka and Wakayama both use mandarin orange flavor (none of the featured Frappuccino types are identical). 
Although the list of all 47 types has been open to the public, customers can buy each type of Frappuccino only within the featured prefecture. 

We conducted an online survey on July 31 in 2021, asking about the five favored Frappuccino types. 
The respondents were recruited through a crowdsourcing service. 
We used *SurveyLegend* as a survey platform.
All types of Frappuccino were displayed along with their names and images in random order, and the respondents were asked to select exactly five items that they wanted to try. 
The preferences of the respondents may be considerably associated with the prefectures where they were born or grew up or with the prefectures where they currently live. 
However, it is also plausible that their preferences are purely dominated by the taste of the Frappuccino itself, e.g., respondents who like orange may tend to choose a Frappuccino provided in Shizuoka or Wakayama, despite these prefectures being spatially far apart. 

### Categories
We manually categorized each type of Frappuccino into four categories: fruit-based (*fruit*), chocolate-based (*chocolate*), tea-based (*tea*), and none of these three (*other*). 
The labels are determined subjectively by the contributor and are not necessarily precise. 
They are not considered as "ground-truth" labels and are only for a better interpretation.

### Demographic information
The survey also asks the prefecture that the respondent currently live (`living_prefecture `) and the hometown (`hometown_prefecture`).


## Contributors
- Tatsuro Kawamoto

## Funding
This dataset was collected by the contributor privately.

## Researches
- Tatsuro Kawamoto, "Single-trajectory map equation," arxiv:***.


## Citation
When you use this dataset in your publication, please cite this web page.

