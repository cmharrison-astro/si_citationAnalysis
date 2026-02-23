# Sonic Intangibles Citation Analysis Project

## Notebooks

There are two notebooks:

1. notebooks/get_data_openalex.ipynb

Performs an API query on OpenAlex (https://openalex.org/) database of published works. Designed to collate basic information on published works on some criteria search as contains "sonification" in the Title or Abstract. This also collates a list of all **cited** works by each **citing** work in the form of lists of OpenAlex IDs. The table is in this format:

Publication_ID Reference_ID
Work1 Work28
Work1 Work254
Work1 Work123
Work2 Work1
Work2 Work24
Work2 Work56

| Publication_ID | Reference_ID |
| ----------- | ----------- |
| Work 1      | Work28      |
| Work 1      | Work254     |
| Work 1      | Work2       |
| Work 2      | Work321     |
| Work 2      | Work24      |
| Work 2      | Work1       |
| Work 2      | Work29      |
| Work 2      | Work456     |
| Work 2      | Work664     |


2. Notebooks/sonification_citation_analysis.ipynb

Performs a citation network analysis on the output from the OpenAlex query.

## Data

Fake data was created to represent three groups (by design).

* Group 1 (well connected), N=7
* Group 2 (isolated except one line, N=6)
* Group 3 N=5
* Group 4 N=4
* Group 5 N=4

In this fake data, one paper was chosen to be highly cited: WOS:000279731700007