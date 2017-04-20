**README**

This is a project that illustrates the use of NLP in python to topic-model congressional bills.

I've attached the powerpoint project for the core summary, and recommend opening the nmf_display.html file in a web browser for an illustrative data visualization.

For those that would prefer a higher level of detail:

The remote_scraper is designed to be run on an AWS environment in Python 3.0 using pymongo.

The remainder of the files are best viewed in python 2.7, and their own dependencies should be clearly visible by the listed imports in the first box of the jupyter notebook - I did most of my work in this notebook format and recommend it for anyone attempting to parse the work on their own.

remote_scraper can take a significant amount of time to run, so for convenience I've also uploaded a zipped data file - simply open the zipped *bills.json* file and local_analysis should be able to run if dependencies have been resolved.
