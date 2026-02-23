# si_citationAnalysis
Sonic Intangibles Citation Analysis Project

There are two notebooks:

1. notebooks/get_data_openalex.ipynb

Performs an API query on OpenAlex (https://openalex.org/) database of published works. Designed to collate basic information on published works on some criteria search as contains "sonification" in the Title or Abstract. This also collates a list of all **cited** works by each **citing** work in the form of lists of OpenAlex IDs. The table is in this format:

Publication_ID Refernece_ID
Work1 Work28
Work1 Work254
Work1 Work123
Work2 Work1
Work2 Work24
Work2 Work56


2. Notebooks/sonification_citation_analysis.ipynb

Performs a citation network analysis on the output from the OpenAlex query.