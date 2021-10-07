
## Choosing the Topic

There were 6 APIs to choose from, and the first thing I did was to click
through all the links and see which one has the best documentation and
support. I found that the Financial data API was the most intuitive. And
as I was browsing the reference API, I saw that they also support
cryptocurrency API, and because I have personal interest in crypto, I
decided to use this API and focus on cryptocurrency.

## Data Exploration

After listing out the requirements and defining the functions, I started
to play around with the data to see what kind of exploratory data
analysis I wanted to do. First I looked at 6 of the top cryptocurrencies
by market cap and looked at their YTD price change. Next, I looked at
Bitcoin data in detail, comparing the volume and the price. And lastly,
I looked at Bitcoin vs Ethereum, comparing the performances over the
past year.

## Interesting Findings

I had a couple of interesting findings when comparing Bitcoin with
Ethereum. First, for Ethereum, the number of days of gains and losses
over the past year is consistent in each quarter, with around 13-15 more
days of gains than losses in each quarter. Another finding is the
correlation between Bitcoin and Ethereum prices. I was aware that the
crypto market moves as a whole but the correlation was much stronger
than I had expected.

## Difficulties

One issue I encountered was exceeding the API limit of 5 API calls /
minute when rendering the file. I had written multiple functions, and
for each function, I wanted to show the function call and output as
examples. This became an issue when I also needed to call the API
functions when doing the exploratory data analysis. So I added a line of
code that pauses the document rendering for 60 seconds after having
called the API 5 times, and the issue was resolved.

## Project Approach

I think my overall project approach was good. I first got the functions
working then started to do the exploratory data analysis, and improve
the code along the way. One issue I had was the lack of time. Had the
deadline not been extended I would have felt really rushed. So for
future projects I definitely want to start early.

## Conclusion

I have learned very much from this project. Before taking this course,
the term “API” sounded very technical and difficult. However, I have
learned how to use R to retrieve data from APIs and conduct data
analysis. I will be able to utilize this skill in the future both
personally and professionally.

## Links

Link to the Github page repo:
<https://srlmt.github.io/Crypto-API-Vignette/>

Link to the usual project repo:
<https://github.com/Srlmt/Crypto-API-Vignette>
