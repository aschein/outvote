# Outvote
Data and code for replicating analysis of Outvote's 2018 randomized study.

## What's included:

* [outvote_data.csv](https://github.com/aschein/outvote/blob/master/dat/outvote_data.csv): CSV containing anonymized data for all eligible subjects.
* [outvote_analysis.ipynb](https://github.com/aschein/outvote/blob/master/src/outvote_analysis.ipynb): Jupyter Notebook that shows how to process data and replicates basic results.

## Details of data

The data file [outvote_data.csv](https://github.com/aschein/outvote/blob/master/dat/outvote_data.csv) contains anonymized data for all n=195,118 eligible subjects. Each row contains a subject's:

* Z: assignment (1=assigned treatment, 0=assigned control)
* D: receipt (1=messaged, 0=not messaged)
* Y: voting outcome (1=voted, 0=did not vote)
* M: confident match to voter rolls (1=yes, 0=no)
* Q: position in first queue (1,2,3,... or NaN)

The refined study population consists of subjects with M=1 and Q <= 103.
 
