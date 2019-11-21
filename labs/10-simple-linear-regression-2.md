Lab 10: Simple Linear Regression II
================

## Twins and IQ

In the mid 20th century, a study was conducted that tracked down
identical twins that were separated at birth: one child was raised in
the home of their biological parents and the other in a foster home. In
an attempt to answer the question of whether intelligence is the result
of nature or nurture, both children were given IQ tests.

This data is in a `.csv` file, which is a very general format for data.
You can load our usual packages as well as the data (into the `twins`
data frame) with the following commands:

``` r
library(tidyverse)
twins <- read.csv("http://andrewpbray.github.io/data/twins.csv")
options(scipen = 99)
```

To reduce scientific notation appearing in the output, we can also
specify the option `scipen` to be a large positive value. More info is
available via `?options`.

Since this data was read in from a `.csv` file, there is no help file
associated with it, so I’ll just tell you that the IQ of the foster
child is recorded in `Foster` and the IQ of the biologically-raised
child in `Biological`. The socieoeconomic status of the biological
family was also recorded in `Social`.

1.  Create a plot of the relationship between the IQs of the two
    children and describe the relationship in words (there is no clear
    independent variable here, so just put `Biological` on the x-axis).

2.  Fit a linear model to this data and have a look at the summary of
    the model. Which one of the following is *false* and why?
    
      - For each 10 point increase in the biological twin’s IQ, we
        expect the foster twin’s IQ to increase on average by roughly 9
        points.
      - The linear model (the estimated mean function) is approximately
        ŷ=9.2+0.9x.
      - Foster children with higher than average IQs (average of the
        foster children) will have biological twins with higher than
        average IQs as well (average of the biological children).

3.  Is it reasonable to draw conclusions from this model? Assess the
    conditions for a valid model based on the context of this problem
    using appropriate plots.

4.  This study was used to weigh in on the question of whether IQ is a
    result of nature (your genes) or nurture (your environment). If IQ
    was purely a result of nurture, what slope would you expect to see
    in your linear model? Phrase that hypothetical question in terms of
    a hypothesis test and interpret the p-value in the context of this
    problem.

5.  At the other end of the argument, the distribution of IQ might be
    entirely determined by genes. Use a 95% confidence interval on your
    slope to assess whether this claim is reasonable given your data
    set. (`?confint` may be helpful here or you can build a bootstrap
    interval using `infer`.)

6.  Now consider how the association between IQs would change if social
    class were taken into account. Create a plot to illustrate the
    relationship between all three variables (recall the use of the
    `color` argument in `aes()`). Just by looking at the plot and
    without fitting any models, does it appear that the relationship
    between the IQs is the same for high social class children as it is
    for low social class children?

**Endnote**: The researcher that collected this data was named Cyril
Burt, and his work was the subject of some controversy.

-----

# Problem Set

Please work through problems 24, 25, 30, 31, and 32 in the Exercises at
the end of Chapter 5. Note that with the information provided, the
inferential questions are most easily done using the mathematical
approximation method.
