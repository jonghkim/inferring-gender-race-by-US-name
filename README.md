# Inferring Gender and Race based on the First Name

This is a repository to share a gender-name and a race-name datasets
Usually, both features are inferred at once. However there was a scarse or no repository who collect them in a single repository.

I found these two sources from a paper written by [Lin and Pursiainen (2018)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3045050)

## Gender-Name Dataset
| Column header | Definition |
| :---: | :---: |
| sex | gender |
| name | first name |
| gender.prob | gender probabilities at given name |

This dataset is created by [Peter Organisciak](https://github.com/organisciak/names) who estimates name frequencies by gender based on birth name statistics in U.S. Thus, the inferred gender is derived from the probability which cojointly consider both names and age distributions among living people in 2014.

## Race-Name Dataset

|Column header | Definition |
| :---: | :---: |
| name | Surname |
| rank | National rank at given year |
| count	| Frequency: number of occurrences nationally in 2010 |
| prop100k	| Proportion per 100,000 population for name |
| cum_prop100k	| Cumulative proportion per 100,000 population |
| pctwhite	| Percent Non-Hispanic White Alone |
| pctblack	| Percent Non-Hispanic Black or African American Alone |
| pctapi	| Percent Non-Hispanic Asian and Native Hawaiian and Other Pacific Islander Alone |
| pctaian	| Percent Non-Hispanic American Indian and Alaska Native Alone |
| pct2prace	| Percent Non-Hispanic Two or More Races |
| pcthispanic	| Percent Hispanic or Latino origin |
	
Source: U.S. Census Bureau, 2010 Census.	
Note: Fields suppressed for confidentiality are assigned the value (S).	

This dataset is compiled by [Word, Coleman, Nunziata and Kominski (2008)](https://www.researchgate.net/publication/265005903_Demographic_Aspects_of_Surnames_from_Census_2000), based on the U.S. Census data.

The race is classified by two tress. Firstly, they calculate percentages of 1. Hispanic, 2. Non-Hispanic. After then, they calculate percentages of Whites, Blacks, Asians and Native Americans among Non-Hispanic.

## References
- [US Names Datasets](https://github.com/organisciak/names)
- [Demographic Aspects of Surnames from Census 2000](https://www.researchgate.net/publication/265005903_Demographic_Aspects_of_Surnames_from_Census_2000)
- [Frequently Occurring Surnames from the 2010 Census](https://www.census.gov/topics/population/genealogy/data/2010_surnames.html)
- [Frequently Occurring Surnames from the 2000 Census](https://www.census.gov/topics/population/genealogy/data/2000_surnames.html)
- [Gender Differences in Reward-Based Crowdfunding](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3045050), 2018

## For Citation
```
@misc{jonghkim,
  author = {Jongho Kim},
  title = {inferring-gender-race-by-US-name},
  year = {2018},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/jonghkim/inferring-gender-race-by-name-us}},
}
```