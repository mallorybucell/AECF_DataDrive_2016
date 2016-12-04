## Explanation of files
- Deduplication_of_removal_reason_data.ipynb
	This is a script written to extract removal reasons from 'final_merge_minus_abscondence.csv', and limit to one entry per client. It produces 'removal_reason_per_child.csv'

- removal_reason_per_child.csv
	CSV file that contains removal reason information, one row per unique client ID. This can be easily merged with Andri's script to add final outcome info and create data set with one entry per unique client

- notes.md
	Some thoughts on the process, next steps, etc.

- Playing_with_updated_merge_data.ipynb
	Exploration of data to try and explain why total unique client IDs did not match total unique system entries.  Turns out the entry of 44 clients is not recorded in the data.  Last cell in notebook outputs list of the impacted client ids.