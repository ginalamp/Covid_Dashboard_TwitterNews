# Assignment 2: Twitter Media Outlet Analysis

For a report on the data analysis done in this repo, you can view our report on Overleaf [here](https://www.overleaf.com/read/vsyrhcwznshb)

## Usage
To run this code, simply
1. Open the `.Rmd` you wish to run
2. Select 'Run'
3. Select 'Run all'

## File description
* `number_of_x`: computes the total number of followers, tweets, and retweets of all media outlets and visualises them using a table.
* `relevant_tweets`: computes the tweet frequency of the overall tweets and tweets relevant to COVID-19 and visualises the data using graphs. Additional analysis is also available at the bottom of the file (not available in the report).
* `sentiment_analysis`: applies *Vader* sentiment analysis to the overall tweets and visualises them using graphs.
* `topic_modelling`: applies *LDA* topic modelling to the overall tweets and visualises them. Selects the number of topics using *ldatuning*. Applies sentiment analysis on the extracted topics and visualises the results.

## Extra features
* Global media outlet analysis
* General numerical analysis
* LDA tuning to get the optimal amount of topics per topic modelling analysis
* Microsoft's SharePoint colour palette is used to visualise the data
* Functions used to reduce code

## Error handling
### Topic modelling Ubuntu running notes
If running the code using Linux (Ubuntu), you might need to install additional packages in order to install some of the libraries (such as `topicmodels`, `ldatuning`, `reshape2`, and `vader`)

As always, try googling how to install the package they suggest and install it using their instructions. Here are some packages that I needed to intially install on my Ubuntu device that you can try:

```
sudo apt-get install libgsl0-dev
sudo apt-get install -y r-cran-slam 
sudo apt-get install -y r-cran-xml2 
sudo apt-get install libgmp-dev
sudo apt-get install libmpfr-dev
```
