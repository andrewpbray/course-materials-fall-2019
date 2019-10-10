Lab 6: The Building Blocks of Inference
================

In this lab you will use the following three packages:

``` r
library(tidyverse)
library(oilabs)
library(infer)
```

## Examples, revisited

In lecture we’ve gone through several examples of hypothesis tests on
the blackboard. Now you’ll get the chance to get your hands on the data
and construct those tests.

1.  Using the `promote` data set,
      - Write the null and alternative hypothesis in symbolic notation
        (in markdown).
      - Compute the observed test statistic.
      - Construct and save the null distribution using `infer`.
      - Visualize the null distribution.
      - Compute the p-value.
2.  Using the `millenials` data set,
      - Write the null and alternative hypothesis in symbolic notation.
      - Compute the observed test statistic.
      - Construct and save the null distribution.
      - Visualize the null distribution.
      - Compute the p-value.
3.  Using the `curry` data set,
      - Write the null and alternative hypothesis in symbolic notation.
      - Compute the observed test statistic.
      - Construct and save the null distribution.
      - Visualize the null distribution.
      - Compute the p-value.

## Synthesizing the process

4.  How would you expect the plots of your null distribution to change
    if `reps` were increased to 1000? Give it a try.

5.  In which of the examples above would you be comfortable using the
    Normal curve to describe the null distribution?

## Survey Inference

6.  Return to the `survey141` data and select one or two columns to
    study. Conduct a hypothesis test in the form that you’ve seen in
    this lab and be explicit about each of the 5 steps that you went
    through for previous examples. Additionally, please interpret the
    p-value: what does this mean in the context of our sample of Reedies
    and the population of Reedies in general?

Note that you may need to dust off your `dplyr` skills in order work
with variables that have only two levels. One approach is to `filter`
the data but the other is to use `fct_recode` or `fct_collapse` in the
`forcats` package.

-----

# Problem Set

Please work through problems 10, 13, 16, 18, 20, and 24 in the Exercises
at the end of Chapter 2.
