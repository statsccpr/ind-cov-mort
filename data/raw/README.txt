# 3 days standardized data wrangled into
/raw/date/

# original data from

https://coronavirus.jhu.edu/data
https://covid19.healthdata.org/
https://data.cdc.gov/browse?q=covid&sortBy=relevance

daily original sorted into
/jhu/
/ihme/
/cdc/

## notes 
* cdc has changed their naming conventions a few times over the 2020-2021 year
* before 1/30/2021 the cdc daily downloads were always cumulative, start 2020-02-01 to end date value of `Data As Of` . Although the start date and end date columns are present, the end date was useless placeholder.
* post 1/30/2021 moving towards historical file in long (longitudinal) format. Now, need to make use of 3 primary keys
`Data As Of` `Start Date` `End Date` . Can download the longitudinal format at any time T (don't need daily dl) and specify start date end date range to look back retroactively. The `Start Date` sometimes jumps around,, now stretches back to 2020-01

* post 1/30/2021 also has state x sex x age group death counts

* have not adapted to this new cdc format
