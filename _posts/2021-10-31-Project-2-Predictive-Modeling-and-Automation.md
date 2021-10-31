
# Project Outline

For this project we worked as a group of two to construct predictive
models and we utilized automation in R-Markdown to generate six
different reports. We used the [Online News Popularity Data
Set](https://archive.ics.uci.edu/ml/datasets/Online+News+Popularity),
which has 61 attributes (58 predictive attributes, 2 non-predictive, and
1 response). The response variable is `shares`, which is the number of
shares for a given article, but after doing analysis on the data, we
decided to fit the models on `log(shares)`, which had a much better fit
because there were some extreme values in `shares`.

For the process, We first did exploratory data analysis, then
constructed 2 linear models and 2 ensemble tree-based models, and then
we compared the models and chose the best one for the test set. We used
automation in R-markdown to partition the data to six different data
channels and went through the entire process to generate six individual
documents.

# Links

Link to Project 2 page repo: <https://srlmt.github.io/Project-2/>

Link to the Project 2 Github repo:
<https://github.com/Srlmt/Crypto-API-Vignette>

# Project Reflection

## What I would do Differently

I would not do anything differently. This is my first time collaborating
with someone on Github, so great communication and clean version control
becomes essential. Early in the project my partner and I set up
individual time blocks to update the code and push to the repo. We also
had great communications via daily emails to track the progress. I had a
really great experience working with my partner and I would want to
replicate the same communication and work style for future collaboration
projects.

## Difficulties

I was responsible for the Random Forest model, and it took 40 minutes to
run the model, so I had to find a way to reduce the render time. First I
tried reducing the number of predictors and changing the tuning
parameters. But at the end I decided to use `cache=TRUE` option in the
code chunk so the model is stored and can be accessed in future renders.
Another challenge was trying to display different titles for each of the
six documents, but my partner and I eventually figured it out.

## Big Takeaways

We first fit the models with `shares` as the response variable, but we
found better fit with `log(shares)` and decided to update the models. I
learned that when dealing with a response variable that has extreme
values, doing a log-transformation can reduce the impact of those values
and lead to less variability and a better fit. Also, I learned that even
though the ensemble methods such as the random forest model and the
boosted tree model take longer to run, they often have better fit and
prediction.

# Code to Render this Blog

``` r
# Run this part in the console to render the output
rmarkdown::render("_Rmd/2021-10-31-Project-2-Reflection.Rmd", 
          output_format = "github_document", 
          output_dir = "_posts/",
          output_options = list(html_preview = FALSE)
          )
```
