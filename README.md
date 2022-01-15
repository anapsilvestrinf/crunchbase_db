# Analyzing Startup Fundraising Deals from Crunchbase
### Project completed as part of Dataquest's Data Engineering path.

----------------------------------------------------

## Introduction

In this project, we will reduce memory usage consumed by a dataset. Beyond that, we will load it in chunks into a new SQLite database. Our data is startup investments from Crunchbase.com while working with memory constraints.

Since the information on the startups and their fundraising rounds is always changing and the dataset is from October 2013, the dataset we'll be using isn't completely up to date. It can be downloaded [here](https://github.com/datahoarder/crunchbase-october-2013/blob/master/crunchbase-investments.csv).

The dataset consumes 10.3 megabytes of disk space, and pandas requires 4 to 6 times the amount of space in memory the file does on disk. However, we'll assume we only have 10 megabytes of available memory. 