ST558 Reflection
================
Aries Zhou
11/29/2021

Q1.What (if anything) has changed about what you think a data scientist
is and what they do

I originally thought that data scientist were more focusing on exploring
already-exist data, but that was not true. I understand now that data
scientist does not care too much about those known; they put more
emphasis on prediction about the unknown.

Q2.What your current thoughts are in terms of using R for data science -
do you think you’ll continue to use R going forward? Why or why not?

I will continue using R in the future. After this semester of studying,
I further experienced and enjoyed the advantages of R programming. My
current thoughts about R are similar to thoughts in the beginning of the
semester. R is a such powerful tool that are so flexible and easy to
access for data analysis and model prediction. Its diverse database and
packages are great resources for my future studying. However, its
efficiency improvement is still a big challenge. When facing missive
computation, R is quit slow and dose not improve much using parallel
computing.

Q3.What things are you going to do differently in practice now that
you’ve had this course?

In this course, I realize that the Rmarkdwon is very useful as digital
notebook. I had switched to taking notes using Rmarkdwon and had been
using it to generate files for homework in other classes.

``` r
rmarkdown::render("2021-11-29-Reflection-Blog.Rmd", 
                  output_format = "github_document", 
                  output_dir = "../_posts/",
                  output_options = list(html_preview = FALSE, keep_html=FALSE))
```
