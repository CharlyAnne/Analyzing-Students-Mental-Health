# Analysis: Impact of Length of Stay on International Students’ Mental Health
Does going to university in a different country affect your mental health? 

This project analyzes how the length of stay (stay) impacts the average mental health diagnostic scores among international students. The three psychological metrics studied are:
* PHQ-9 test (todep) – Depression score
* SCS test (tosc) – Social connectedness score
* ASISS test (toas) – Acculturative stress score

## Goal: 

To return a summary table that groups international students by their length of stay and shows how mental health scores vary with time spent.

## Method:
Filter: Only international students were considered in the analysis.

Group by: `stay` (length of stay in years)

Aggregate:

`count_int`: Count of international students in each group.

`average_phq`: Mean of `todep` (PHQ-9) rounded to 2 decimals.

`average_scs`: Mean of `tosc` (SCS) rounded to 2 decimals.

`average_as`: Mean of `toas` (ASISS) rounded to 2 decimals.

Sort: Results were sorted by `stay` in descending order.

Limit: Displayed only the top 9 rows.

## Here is a data description of the columns in the dataset used.

| Field Name   | Description                                               |
|--------------|-----------------------------------------------------------|
| inter_dom    | Types of students (international or domestic)             |
| japanese_cate| Japanese language proficiency                             |
| english_cate | English language proficiency                              |
| academic     | Current academic level (undergraduate or graduate)        |
| age          | Current age of student                                    |
| stay         | Current length of stay in years                           |
| todep        | Total score of depression (PHQ-9 test)                    |
| tosc         | Total score of social connectedness (SCS test)            |
| toas         | Total score of acculturative stress (ASISS test)          |
