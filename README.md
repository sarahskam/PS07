PS07 - Sarah Kam
================

## A Wicked Awesome Title

Woo!! This is the section of text under the title in my README.Rmd!

## CODE ALERT! THERE’S CODE HERE!

Here is a little bit of R code displaying the numbers 1 to 5 and their
values multiplied by 2!

``` r
x <- c(1:5)
y <- c(2*x)
xy_dataframe <- data.frame(
  x_col = x,
  y_col = y
)
xy_dataframe
```

    ##   x_col y_col
    ## 1     1     2
    ## 2     2     4
    ## 3     3     6
    ## 4     4     8
    ## 5     5    10

## Evil Plotting Lies Ahead

Here is a plot of x and y from the previous bit of code!

``` r
library(ggplot2)
ggplot(data=xy_dataframe, mapping=aes(x = x_col, y = y_col)) +
  geom_line() + 
  geom_point() +
  labs(title="A straight line with slope = 2")
```

![](README_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->
