### Water quality testing results 2016-2017

This repo contains the Jupyter notebooks, data and charts from water our quality testing project with the Hackuarium. This repo is a build from the hammerdirt/notes repo. That folder has been trashed only a local copy exists.

#### The data:
The original data is stored in two files - Data_2016.csv and Data_2017.csv. This data is in its original format, there are a few duplicate records and there is some formatting to be done if you want to use it.

The data has been cleaned and stored in the JSON folder. Identifiers like colony colors, week dates or week numbers and any information we needed to index the results is stored in the utililties folders as JSON objects.

#### The workbooks:

If you clone this repo everything is local and will work just fine.

ATTENTION: The file output is in the notebook, so if you change something without changing the filename or destination folder,
you will overwrite the original.


There are three workbooks : 

1 - Preparing the data: we go through all the gymnastics necesary to  make JSON output for other applications. Our end-use is a web based app that has the same output as the notebook.

2- Output for hdhc: The JSON output is used to make the various charts

3- Micro-bar-chart: We tap into the original data to make barchart arrays of all the results per location per day.

#### Packages and dependencies:

The requirements file is from "pip freeze >" this should be good for anybody using a virtual env. If you are using Anaconda
go off the list. If in doubt here are the list of imports from the the note book:

1. import pandas as pd
2. import numpy as np
3. import matplotlib
4. import matplotlib.pyplot as plt
5. import json
6. import re
7. from textwrap import wrap
8. import matplotlib.ticker
9. import os
10. import seaborn as sns

#### Contributing:

Submit a pull request if you see something that really needs to be changed.


