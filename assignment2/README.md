# Assignment 2

[Graph Allocation spreadsheet](https://docs.google.com/spreadsheets/d/1thUrLAOECz5pQ8OlmwxMl1a2i2PxGF3Oj1CnxEZAU8g/edit?usp=sharing)

## Twitter connection resources
* [TwitterScraper](https://github.com/MatthewWolff/TwitterScraper)
    - gets tweets for a longer time period (get more than 3200 tweets)
    - in order to run:
        - add keys to `api_keys.example.py` and then rename to `api_keys.py`
        - Change code in `init_chrome()` from chrome web driver to firefox webdriver
        - Make sure to explicitly set the path to the geckodriver
            - [Intall geckodriver and set path Ubuntu](https://askubuntu.com/questions/870530/how-to-install-geckodriver-in-ubuntu)
            - [Set gecko path in script explicitly](https://stackoverflow.com/questions/45992670/geckodriver-not-being-found)
        - run script with parameters as specified in the github "Using the Scraper" section.
        - convert JSON to R vector:
        - `library(rjson) vect <- names(fromJSON(file="<jsonFileName>"))`
* [Getting access to the Twitter API | Docs](https://developer.twitter.com/en/docs/twitter-api/getting-started/getting-access-to-the-twitter-api)
* rtweet - R package as well
* [Twitter Object V1 API docs](https://developer.twitter.com/en/docs/twitter-api/v1/data-dictionary/object-model/tweet)

## Report resources
* [Creating Reports with R Markdown - pdf and word](https://towardsdatascience.com/creating-reports-with-r-markdown-c6031ecdd65c)
* [Create HTML report](https://jozef.io/r913-spin-with-style/)

## Analysis resources
* [TidyTextMining Ch7 Case study: comparing Twitter archives](https://www.tidytextmining.com/twitter.html)
    - currently following this for a basic exploratory analysis
* [Passing a variable name to a function in R](https://stackoverflow.com/questions/19133980/passing-a-variable-name-to-a-function-in-r)

## Notes

- Collect dataset of different media agencies over last 6 months
- Topics, sentiments
- Define some own lexicons
- Example graphs: frequencies, Network interaction metrics
    - Contain pandemic, vaccination, lockdown
    - How topics increase/decrease over time vs media company
    - How compare between topics
    - Topic modelling
    - Sentiment analysis of tweets
    - Sentiment of topics
    - Filter tweets not on pandemic out
        - Use topic modelling or dictionary analysis
    - Additional marks (20%) - without this you’re capped at 80%
        - Identify additional sources and apply analysis
            - Pandaguys
            - Polititians
- Expectations: process
    - Data collection
    - Store data
    - Read in
    - Analyse
- Expectations: presentation (15%)
    - Figures, analysis, statistics, reports
- Define set of media agencies/accounts
    - Collect tweets
        - Tell about what’s up with tweets
- Twitter API V1
- Twitter API package (rtweet)
    - Limitation: only 2 weeks search
    - Specify timeline of specific accounts

