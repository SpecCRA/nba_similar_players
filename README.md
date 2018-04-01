# Finding Similar NBA Players with Machine Learning

## Summary
* This script uses KDTree algorithm to find recent similar NBA players to the players in the championship teams in 2003 and 2011. The data used was gathered from [this script.](https://github.com/SpecCRA/nba_data_scrapers) The final visualizations are in 3 tables as shown in the picture files.
* A detailed blog post can be viewed [here.](https://anaspiringsportsnerd.wordpress.com/2018/04/01/using-maths-to-find-similar-players/)

## Notes
* Data is subsetted to `>= 27 games` played and `>= 450` minutes played. The intention was to reduce noise from players who contributed very little to the season.
* I outputted 8 similar player seasons because some of them are unsurprisingly similar to themselves. I chose to only keep up to 5 total similar players in the final tables.
* **Recent** season is defined any season after 2010-11.
* I chose to drop totals and per 100p statistics because they'd output similar players that are themselves too often.

## Possible Improvements
* In addition to the statistics already available, gathering about shot distance, freqency based on distance, and volume would create better and more accurate data. 
* Perhaps I should have also included height, but I think this is good too. Going from traditional positions to new age small ball is an interesting look into the seasons. 

## Technology Used
* **Python**
* **Pandas**
* **Jupyter Notebook**
* **NumPy**
* **Scikit-Learn**
* **Microsoft Excel**