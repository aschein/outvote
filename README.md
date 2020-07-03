# Outvote
Data and code for replicating analysis of Outvote's 2018 randomized study.

The MIT License (MIT)

Copyright (c) 2020 Aaron Schein

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

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
