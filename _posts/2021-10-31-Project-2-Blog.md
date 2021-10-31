2021-10-31-Project-2-Blog
================
Aries Zhou
10/31/2021

#### Project 1 Backgrounds

The purpose of this repository is to create predictive models and
automating Markdown reports. Analysis are done on the **Online News
Popularity Data Set**. Further information about this data can be
accessed
[here](https://archive.ics.uci.edu/ml/datasets/Online+News+Popularity).

In this project, subsets by channel type were produced for automating
Markdown reports. Variables were selected from each subset by the best
subset and stepwise selection methods. Predictive models including the
linear regression models, lasso models, random forest models and boosted
tree models were constructed using 5-fold cross-validation. These models
were first constructed on training data set and than tested on test data
set. The best model were selected based on lowest RMSE.

#### Reflections

For large-dimension data like the data used in this project, instead of
considering all variables for precision, I would select a subset for
later analysis in the further Project. Those relevant variables in the
subset would be selected based on prior knowledge or the point of
interest. Next, exploratory data analysis would be performed on the
chosen subset and filter the relevant variables again to improve
efficiency in the modeling process.

The most difficult part for me is the random forest regression. Due to
the large-scale input, the random forest computation was really slow. My
teammate and I both tried ways to shorten the computation time, such as
reduce the number of parameters, use a subset data, and apply parallel
computing.

My big take-aways from this project is that there is trade-offs between
precision and manageable computing timing. Although accounts for all
variables and using larger number for parameters in the regression
process helps to improve precision in predictive models. It is not too
applicable in practice due to the higher cost in computation. (excessive
timing and problem of over-fitting) Therefore, I found that we sometimes
need to compromise and find a best intermediary decision. In addition,
even though the parallel computing helps to improve the timing a little,
it does not significantly enhance the computing efficiency.

#### [Link](https://ywzhou33.github.io/ST558-Project-2/) to the Github Pages repo and [link](https://github.com/ywzhou33/ywzhou33.github.io.git) to Github Blog repo.

``` r
rmarkdown::render("2021-10-31-Project-2-Blog.Rmd", 
                  output_format = "github_document", 
                  output_dir = "../_posts/",
                  output_options = list(html_preview = FALSE, keep_html=FALSE))
```
