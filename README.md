**README**

This is a project that illustrates the use of NLP in python to topic-model congressional bills.

I've attached the powerpoint project for the core summary, and recommend opening the nmf_display.html file in a web browser for an illustrative data visualization.

For those that would prefer a higher level of detail:

The remote_scraper is designed to be run on an AWS environment in Python 3.0 using pymongo. However, it is written with original break-points that occurred in that project, simply running it as-is is not advisable. For anyone not comfortable editting the written scraping methods, it is strongly encouraged to unpack the zipped *bills.json* file. I will additionally note that as written, the scraping methods can take several hours to run. Again, for ease of use, the zipped bills.json file is available.

The local_analysis file was written python 2.7, and dependencies should be clearly visible by the listed imports in the first box of the jupyter notebook. I did most of my work in this notebook format and recommend it for anyone attempting to parse the work on their own.

Note that for your own replications of the LDAvis in the local_analysis notebook, running LDAvis multiple times on the same exact dataset may result in different-looking graphs - this has to do with the massive amount of dimensionality reduction being done. Graphs that contain the same information on the right hand side may NOT look the same visually, so results are typically *not* strictly reproducible.

---

Intended Order Of Work:

1) **RECOMMENDED:** Unpack the bills.json file with a .zip extractor.

1a) **ALTERNATIVE:** Run remote_scraper. **HOWEVER,** please take a look at the specific code in the remote_scraper algorithm before running - it can take an extended time (hours/overnight) to do the scraping, and the code as written was designed specifically to handle an event-related break that occured in the original execution of filling the db - it may not break at the same points for you, which could cause duplication errors that will later bias the analysis section.

2) Make sure you have installed any dependencies that are required by the first box (which has all the imported packages) in the local_analysis notebook.

3) The local_analysis notebook should be good to run! I hope the word cloud and visualizations are enjoyable to view! Please note my earlier comments about the irreproducibility of appearance of the LDAvis charts.
