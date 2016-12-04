### Notes on munging this data:
- we wanted to look at whether there was any relationship between child's first placement upon entry into the system and their ultimate final outcome upon exiting the system for the last time (good, bad, neutral)
	* There was no easy way to identify final outcome since data is by spells and different students have different numbers of spells

	* We had to consult with experts to apply value judgement to each final placement exit

	* We discovered there are 44 students for whom we have no information about their entry into the system. (First spell is missing from data)
	
- best practices for this data set

	* A large part of my time was spent making sure I understood the nuances and terminology of the data set, as well as trying to understand how the included data was or was not relevant to the questions we were attempting to answer.

    * The merge spreadsheet is helpful because it has a large amount of granular data, but there is a lot of overlap in what/how things are recorded. It is difficult to tease out the necessary data, and also to double check for accuracy/duplication.  

    * In addition to data dictionary, the list of naming conventions for columns / explanation of what data is referring to is necessary, as some of the naming conventions seem counter-intuitive to someone outside the system.


    * We created a scxript to reduce the data to one row per student so we could more easily look for direct trends from initial entry to  final coutcome. Because sequence/number data is single-digit '1', rather than all double-digit '01', it is easy to introduce errors when filtering or removing duplicates.

    * May be useful to keep two tables- one with student first entry and placement exit (with reason), another to preserve individual placement and spell data. 

- best practices for ideal data set
    * In an ideal world, data collection would be streamlined so there is less overlapping data (seq number, 'home_rmvl_seq', two 'placement exit' columns with different info, etc.) Standardize input / cleanse old data to std and then update and keep it cleansed at points of further entry.

    - if possible, work mainly from merged spreadsheet b/c don’t really need minutiae or can more easily do w/ linking table, and this is cleanest.


### Future work


- There is still a large amount of work to do to get to an algorithm. More feature exploration is necessary.

- Just for an alogrithm that places a child based on entry statistics without in-depth provider consideration, we would need several more hours of data exploration and descriptive stats, feature determination
- 10 - 20 hours of model testing, refining (try categorization)

- Integrating this with the current work on provider analysis would be additional hours as well.


### Other thoughts (unfiltered)

	- duplication of effort
		* Although the mobility team discovered the duplication errors in the data early, it turned out that this directly impacted the scripts and data we were attempting to work with, so much time yesterday was spent duplicating their efforts unknowingly, and then adjusting my work to use their cleaned data in an effort to maintain version control and minimize any errors I made in this process.


	- duplication in data set and how to pick which is relevant, etc.
		* It was very difficult to tell which data in the set was relevant, even with the data dictionary, because the terminology is specialized but also mimics other familiar terms. This makes a lot of the data names counter-intuitive and the dataset take longer to grasp initially.

	- I think the placement team has a lot of interesting pieces of work, that could make something strong together, but it was difficult to coordinate.

	- Although the merged spreadsheet is cleaner than the original data, there still seems to be places (in sequence numbers, tracking spells vs placements, noting reason for placement or cw exit, etc,) where data is being collected in multiple ways with different practices and it's hard to tell which is accurate.

	For example, 
