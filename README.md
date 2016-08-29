Assignments
================
Sihle

Assignment 2
============

``` r
data("anscombe")
dim(anscombe)
```

    ## [1] 11  8

``` r
names(anscombe)
```

    ## [1] "x1" "x2" "x3" "x4" "y1" "y2" "y3" "y4"

``` r
head(anscombe)
```

    ##   x1 x2 x3 x4   y1   y2    y3   y4
    ## 1 10 10 10  8 8.04 9.14  7.46 6.58
    ## 2  8  8  8  8 6.95 8.14  6.77 5.76
    ## 3 13 13 13  8 7.58 8.74 12.74 7.71
    ## 4  9  9  9  8 8.81 8.77  7.11 8.84
    ## 5 11 11 11  8 8.33 9.26  7.81 8.47
    ## 6 14 14 14  8 9.96 8.10  8.84 7.04

``` r
tail(anscombe)
```

    ##    x1 x2 x3 x4    y1   y2   y3    y4
    ## 6  14 14 14  8  9.96 8.10 8.84  7.04
    ## 7   6  6  6  8  7.24 6.13 6.08  5.25
    ## 8   4  4  4 19  4.26 3.10 5.39 12.50
    ## 9  12 12 12  8 10.84 9.13 8.15  5.56
    ## 10  7  7  7  8  4.82 7.26 6.42  7.91
    ## 11  5  5  5  8  5.68 4.74 5.73  6.89

``` r
summary(anscombe)
```

    ##        x1             x2             x3             x4    
    ##  Min.   : 4.0   Min.   : 4.0   Min.   : 4.0   Min.   : 8  
    ##  1st Qu.: 6.5   1st Qu.: 6.5   1st Qu.: 6.5   1st Qu.: 8  
    ##  Median : 9.0   Median : 9.0   Median : 9.0   Median : 8  
    ##  Mean   : 9.0   Mean   : 9.0   Mean   : 9.0   Mean   : 9  
    ##  3rd Qu.:11.5   3rd Qu.:11.5   3rd Qu.:11.5   3rd Qu.: 8  
    ##  Max.   :14.0   Max.   :14.0   Max.   :14.0   Max.   :19  
    ##        y1               y2              y3              y4        
    ##  Min.   : 4.260   Min.   :3.100   Min.   : 5.39   Min.   : 5.250  
    ##  1st Qu.: 6.315   1st Qu.:6.695   1st Qu.: 6.25   1st Qu.: 6.170  
    ##  Median : 7.580   Median :8.140   Median : 7.11   Median : 7.040  
    ##  Mean   : 7.501   Mean   :7.501   Mean   : 7.50   Mean   : 7.501  
    ##  3rd Qu.: 8.570   3rd Qu.:8.950   3rd Qu.: 7.98   3rd Qu.: 8.190  
    ##  Max.   :10.840   Max.   :9.260   Max.   :12.74   Max.   :12.500

Assignment 3
============

<img src="./figures/xy_plot-1.svg" style="display: block; margin: auto;" />

Assignment 4
============

Chunk 1
-------

``` r
analgesicdf <- read.csv('analgesic.csv')
analgesicdf
```

    ##    ID     Group Measurement_1 Measurement_2 Measurement_3
    ## 1   1 Analgesic            26            26            21
    ## 2   2 Analgesic            29            26            23
    ## 3   3 Analgesic            24            28            22
    ## 4   4 Analgesic            25            22            24
    ## 5   5 Analgesic            24            28            23
    ## 6   6 Analgesic            22            23            26
    ## 7   7 Analgesic            25            25            30
    ## 8   8 Analgesic            28            21            21
    ## 9   9 Analgesic            22            26            20
    ## 10 10 Analgesic            18            25            29
    ## 11 11 Analgesic            25            29            28
    ## 12 12 Analgesic            26            25            23
    ## 13 13 Analgesic            26            25            26
    ## 14 14 Analgesic            19            30            27
    ## 15 15 Analgesic            24            20            24
    ## 16 16 Analgesic            23            24            27
    ## 17 17 Analgesic            24            32            28
    ## 18 18 Analgesic            24            17            25
    ## 19 19 Analgesic            23            25            23
    ## 20 20 Analgesic            30            18            25
    ## 21 21   Placebo            19            12            18
    ## 22 22   Placebo            10            16            18
    ## 23 23   Placebo            12            11            20
    ## 24 24   Placebo            17            17            18
    ## 25 25   Placebo            18            18            20
    ## 26 26   Placebo            12            16            16
    ## 27 27   Placebo            14            17            17
    ## 28 28   Placebo            20            19            18
    ## 29 29   Placebo            16            19            15
    ## 30 30   Placebo            17            15            13
    ## 31 31   Placebo            18            21            14
    ## 32 32   Placebo            20            13            16
    ## 33 33   Placebo            12             8            21
    ## 34 34   Placebo            20            17            16
    ## 35 35   Placebo            17            21            15
    ## 36 36   Placebo            19            17            15
    ## 37 37   Placebo            14            19            13
    ## 38 38   Placebo            17            19            13
    ## 39 39   Placebo            11            20            18
    ## 40 40   Placebo            15            18            12

Chunk 2
-------

``` r
analgesicdf
```

    ##    ID     Group Measurement_1 Measurement_2 Measurement_3
    ## 1   1 Analgesic            26            26            21
    ## 2   2 Analgesic            29            26            23
    ## 3   3 Analgesic            24            28            22
    ## 4   4 Analgesic            25            22            24
    ## 5   5 Analgesic            24            28            23
    ## 6   6 Analgesic            22            23            26
    ## 7   7 Analgesic            25            25            30
    ## 8   8 Analgesic            28            21            21
    ## 9   9 Analgesic            22            26            20
    ## 10 10 Analgesic            18            25            29
    ## 11 11 Analgesic            25            29            28
    ## 12 12 Analgesic            26            25            23
    ## 13 13 Analgesic            26            25            26
    ## 14 14 Analgesic            19            30            27
    ## 15 15 Analgesic            24            20            24
    ## 16 16 Analgesic            23            24            27
    ## 17 17 Analgesic            24            32            28
    ## 18 18 Analgesic            24            17            25
    ## 19 19 Analgesic            23            25            23
    ## 20 20 Analgesic            30            18            25
    ## 21 21   Placebo            19            12            18
    ## 22 22   Placebo            10            16            18
    ## 23 23   Placebo            12            11            20
    ## 24 24   Placebo            17            17            18
    ## 25 25   Placebo            18            18            20
    ## 26 26   Placebo            12            16            16
    ## 27 27   Placebo            14            17            17
    ## 28 28   Placebo            20            19            18
    ## 29 29   Placebo            16            19            15
    ## 30 30   Placebo            17            15            13
    ## 31 31   Placebo            18            21            14
    ## 32 32   Placebo            20            13            16
    ## 33 33   Placebo            12             8            21
    ## 34 34   Placebo            20            17            16
    ## 35 35   Placebo            17            21            15
    ## 36 36   Placebo            19            17            15
    ## 37 37   Placebo            14            19            13
    ## 38 38   Placebo            17            19            13
    ## 39 39   Placebo            11            20            18
    ## 40 40   Placebo            15            18            12

``` r
dim(analgesicdf)
```

    ## [1] 40  5

``` r
names(analgesicdf)
```

    ## [1] "ID"            "Group"         "Measurement_1" "Measurement_2"
    ## [5] "Measurement_3"

``` r
head(analgesicdf)
```

    ##   ID     Group Measurement_1 Measurement_2 Measurement_3
    ## 1  1 Analgesic            26            26            21
    ## 2  2 Analgesic            29            26            23
    ## 3  3 Analgesic            24            28            22
    ## 4  4 Analgesic            25            22            24
    ## 5  5 Analgesic            24            28            23
    ## 6  6 Analgesic            22            23            26

``` r
tail(analgesicdf)
```

    ##    ID   Group Measurement_1 Measurement_2 Measurement_3
    ## 35 35 Placebo            17            21            15
    ## 36 36 Placebo            19            17            15
    ## 37 37 Placebo            14            19            13
    ## 38 38 Placebo            17            19            13
    ## 39 39 Placebo            11            20            18
    ## 40 40 Placebo            15            18            12

``` r
summary(analgesicdf)
```

    ##        ID              Group    Measurement_1   Measurement_2 
    ##  Min.   : 1.00   Analgesic:20   Min.   :10.00   Min.   : 8.0  
    ##  1st Qu.:10.75   Placebo  :20   1st Qu.:17.00   1st Qu.:17.0  
    ##  Median :20.50                  Median :20.00   Median :20.0  
    ##  Mean   :20.50                  Mean   :20.12   Mean   :20.7  
    ##  3rd Qu.:30.25                  3rd Qu.:24.00   3rd Qu.:25.0  
    ##  Max.   :40.00                  Max.   :30.00   Max.   :32.0  
    ##  Measurement_3  
    ##  Min.   :12.00  
    ##  1st Qu.:16.00  
    ##  Median :20.50  
    ##  Mean   :20.52  
    ##  3rd Qu.:24.25  
    ##  Max.   :30.00

Chunk 3
-------

``` r
library(dplyr)
```

    ## 
    ## Attaching package: 'dplyr'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     filter, lag

    ## The following objects are masked from 'package:base':
    ## 
    ##     intersect, setdiff, setequal, union

``` r
library(tidyr)

df1<-gather(analgesicdf, key = One, value = Two, Measurement_1, Measurement_2, Measurement_3)
df2<-group_by(df1, ID, Group)
df3<-summarise(df2, mean(Two))
print(df1)
```

    ##     ID     Group           One Two
    ## 1    1 Analgesic Measurement_1  26
    ## 2    2 Analgesic Measurement_1  29
    ## 3    3 Analgesic Measurement_1  24
    ## 4    4 Analgesic Measurement_1  25
    ## 5    5 Analgesic Measurement_1  24
    ## 6    6 Analgesic Measurement_1  22
    ## 7    7 Analgesic Measurement_1  25
    ## 8    8 Analgesic Measurement_1  28
    ## 9    9 Analgesic Measurement_1  22
    ## 10  10 Analgesic Measurement_1  18
    ## 11  11 Analgesic Measurement_1  25
    ## 12  12 Analgesic Measurement_1  26
    ## 13  13 Analgesic Measurement_1  26
    ## 14  14 Analgesic Measurement_1  19
    ## 15  15 Analgesic Measurement_1  24
    ## 16  16 Analgesic Measurement_1  23
    ## 17  17 Analgesic Measurement_1  24
    ## 18  18 Analgesic Measurement_1  24
    ## 19  19 Analgesic Measurement_1  23
    ## 20  20 Analgesic Measurement_1  30
    ## 21  21   Placebo Measurement_1  19
    ## 22  22   Placebo Measurement_1  10
    ## 23  23   Placebo Measurement_1  12
    ## 24  24   Placebo Measurement_1  17
    ## 25  25   Placebo Measurement_1  18
    ## 26  26   Placebo Measurement_1  12
    ## 27  27   Placebo Measurement_1  14
    ## 28  28   Placebo Measurement_1  20
    ## 29  29   Placebo Measurement_1  16
    ## 30  30   Placebo Measurement_1  17
    ## 31  31   Placebo Measurement_1  18
    ## 32  32   Placebo Measurement_1  20
    ## 33  33   Placebo Measurement_1  12
    ## 34  34   Placebo Measurement_1  20
    ## 35  35   Placebo Measurement_1  17
    ## 36  36   Placebo Measurement_1  19
    ## 37  37   Placebo Measurement_1  14
    ## 38  38   Placebo Measurement_1  17
    ## 39  39   Placebo Measurement_1  11
    ## 40  40   Placebo Measurement_1  15
    ## 41   1 Analgesic Measurement_2  26
    ## 42   2 Analgesic Measurement_2  26
    ## 43   3 Analgesic Measurement_2  28
    ## 44   4 Analgesic Measurement_2  22
    ## 45   5 Analgesic Measurement_2  28
    ## 46   6 Analgesic Measurement_2  23
    ## 47   7 Analgesic Measurement_2  25
    ## 48   8 Analgesic Measurement_2  21
    ## 49   9 Analgesic Measurement_2  26
    ## 50  10 Analgesic Measurement_2  25
    ## 51  11 Analgesic Measurement_2  29
    ## 52  12 Analgesic Measurement_2  25
    ## 53  13 Analgesic Measurement_2  25
    ## 54  14 Analgesic Measurement_2  30
    ## 55  15 Analgesic Measurement_2  20
    ## 56  16 Analgesic Measurement_2  24
    ## 57  17 Analgesic Measurement_2  32
    ## 58  18 Analgesic Measurement_2  17
    ## 59  19 Analgesic Measurement_2  25
    ## 60  20 Analgesic Measurement_2  18
    ## 61  21   Placebo Measurement_2  12
    ## 62  22   Placebo Measurement_2  16
    ## 63  23   Placebo Measurement_2  11
    ## 64  24   Placebo Measurement_2  17
    ## 65  25   Placebo Measurement_2  18
    ## 66  26   Placebo Measurement_2  16
    ## 67  27   Placebo Measurement_2  17
    ## 68  28   Placebo Measurement_2  19
    ## 69  29   Placebo Measurement_2  19
    ## 70  30   Placebo Measurement_2  15
    ## 71  31   Placebo Measurement_2  21
    ## 72  32   Placebo Measurement_2  13
    ## 73  33   Placebo Measurement_2   8
    ## 74  34   Placebo Measurement_2  17
    ## 75  35   Placebo Measurement_2  21
    ## 76  36   Placebo Measurement_2  17
    ## 77  37   Placebo Measurement_2  19
    ## 78  38   Placebo Measurement_2  19
    ## 79  39   Placebo Measurement_2  20
    ## 80  40   Placebo Measurement_2  18
    ## 81   1 Analgesic Measurement_3  21
    ## 82   2 Analgesic Measurement_3  23
    ## 83   3 Analgesic Measurement_3  22
    ## 84   4 Analgesic Measurement_3  24
    ## 85   5 Analgesic Measurement_3  23
    ## 86   6 Analgesic Measurement_3  26
    ## 87   7 Analgesic Measurement_3  30
    ## 88   8 Analgesic Measurement_3  21
    ## 89   9 Analgesic Measurement_3  20
    ## 90  10 Analgesic Measurement_3  29
    ## 91  11 Analgesic Measurement_3  28
    ## 92  12 Analgesic Measurement_3  23
    ## 93  13 Analgesic Measurement_3  26
    ## 94  14 Analgesic Measurement_3  27
    ## 95  15 Analgesic Measurement_3  24
    ## 96  16 Analgesic Measurement_3  27
    ## 97  17 Analgesic Measurement_3  28
    ## 98  18 Analgesic Measurement_3  25
    ## 99  19 Analgesic Measurement_3  23
    ## 100 20 Analgesic Measurement_3  25
    ## 101 21   Placebo Measurement_3  18
    ## 102 22   Placebo Measurement_3  18
    ## 103 23   Placebo Measurement_3  20
    ## 104 24   Placebo Measurement_3  18
    ## 105 25   Placebo Measurement_3  20
    ## 106 26   Placebo Measurement_3  16
    ## 107 27   Placebo Measurement_3  17
    ## 108 28   Placebo Measurement_3  18
    ## 109 29   Placebo Measurement_3  15
    ## 110 30   Placebo Measurement_3  13
    ## 111 31   Placebo Measurement_3  14
    ## 112 32   Placebo Measurement_3  16
    ## 113 33   Placebo Measurement_3  21
    ## 114 34   Placebo Measurement_3  16
    ## 115 35   Placebo Measurement_3  15
    ## 116 36   Placebo Measurement_3  15
    ## 117 37   Placebo Measurement_3  13
    ## 118 38   Placebo Measurement_3  13
    ## 119 39   Placebo Measurement_3  18
    ## 120 40   Placebo Measurement_3  12

``` r
print(df2)
```

    ## Source: local data frame [120 x 4]
    ## Groups: ID, Group [40]
    ## 
    ##       ID     Group           One   Two
    ##    <int>    <fctr>         <chr> <int>
    ## 1      1 Analgesic Measurement_1    26
    ## 2      2 Analgesic Measurement_1    29
    ## 3      3 Analgesic Measurement_1    24
    ## 4      4 Analgesic Measurement_1    25
    ## 5      5 Analgesic Measurement_1    24
    ## 6      6 Analgesic Measurement_1    22
    ## 7      7 Analgesic Measurement_1    25
    ## 8      8 Analgesic Measurement_1    28
    ## 9      9 Analgesic Measurement_1    22
    ## 10    10 Analgesic Measurement_1    18
    ## # ... with 110 more rows

``` r
print(df3)
```

    ## Source: local data frame [40 x 3]
    ## Groups: ID [?]
    ## 
    ##       ID     Group mean(Two)
    ##    <int>    <fctr>     <dbl>
    ## 1      1 Analgesic  24.33333
    ## 2      2 Analgesic  26.00000
    ## 3      3 Analgesic  24.66667
    ## 4      4 Analgesic  23.66667
    ## 5      5 Analgesic  25.00000
    ## 6      6 Analgesic  23.66667
    ## 7      7 Analgesic  26.66667
    ## 8      8 Analgesic  23.33333
    ## 9      9 Analgesic  22.66667
    ## 10    10 Analgesic  24.00000
    ## # ... with 30 more rows

Assignment 5
============

Chicken weights
---------------

-   Null Hypothesis: The chicks' weights are not dependent on the feed.
-   Alternative Hypothesisi: The chicks' weights are dependent on the feed.

``` r
chw <- read.csv('chick-weights (1).csv')
chw
```

    ##    weight      feed
    ## 1     179 horsebean
    ## 2     160 horsebean
    ## 3     136 horsebean
    ## 4     227 horsebean
    ## 5     217 horsebean
    ## 6     168 horsebean
    ## 7     108 horsebean
    ## 8     124 horsebean
    ## 9     143 horsebean
    ## 10    140 horsebean
    ## 11    309   linseed
    ## 12    229   linseed
    ## 13    181   linseed
    ## 14    141   linseed
    ## 15    260   linseed
    ## 16    203   linseed
    ## 17    148   linseed
    ## 18    169   linseed
    ## 19    213   linseed
    ## 20    257   linseed
    ## 21    244   linseed
    ## 22    271   linseed
    ## 23    243   soybean
    ## 24    230   soybean
    ## 25    248   soybean
    ## 26    327   soybean
    ## 27    329   soybean
    ## 28    250   soybean
    ## 29    193   soybean
    ## 30    271   soybean
    ## 31    316   soybean
    ## 32    267   soybean
    ## 33    199   soybean
    ## 34    171   soybean
    ## 35    158   soybean
    ## 36    248   soybean
    ## 37    423 sunflower
    ## 38    340 sunflower
    ## 39    392 sunflower
    ## 40    339 sunflower
    ## 41    341 sunflower
    ## 42    226 sunflower
    ## 43    320 sunflower
    ## 44    295 sunflower
    ## 45    334 sunflower
    ## 46    322 sunflower
    ## 47    297 sunflower
    ## 48    318 sunflower
    ## 49    325  meatmeal
    ## 50    257  meatmeal
    ## 51    303  meatmeal
    ## 52    315  meatmeal
    ## 53    380  meatmeal
    ## 54    153  meatmeal
    ## 55    263  meatmeal
    ## 56    242  meatmeal
    ## 57    206  meatmeal
    ## 58    344  meatmeal
    ## 59    258  meatmeal
    ## 60    368    casein
    ## 61    390    casein
    ## 62    379    casein
    ## 63    260    casein
    ## 64    404    casein
    ## 65    318    casein
    ## 66    352    casein
    ## 67    359    casein
    ## 68    216    casein
    ## 69    222    casein
    ## 70    283    casein
    ## 71    332    casein

``` r
#boxplot
plot(chw$feed, chw$weight)
```

![](README_files/figure-markdown_github/unnamed-chunk-1-1.png)

``` r
#One-way anova
chw1 <- aov(chw$weight ~ chw$feed, data = chw)
summary(chw1)
```

    ##             Df Sum Sq Mean Sq F value   Pr(>F)    
    ## chw$feed     5 231129   46226   15.37 5.94e-10 ***
    ## Residuals   65 195556    3009                     
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

-   Test Assumptions- there are more than 2 groups and the data is parametric.

-   df=5
-   p value =5.94e-10
-   we reject the null hypothesis. The chicks' weights are dependent on the type of feed.

------------------------------------------------------------------------

The Hot Zone
------------

-   Null Hypothesis-The gastroenteritis is not caused by drinking contaminated water.
-   Alternative Hypothesis- Gatroenteritis is caused by drinking contaminated water.

``` r
gast<- read.csv('gastroenteritis (2).CSV')
gast
```

    ##             Consumption Outcome
    ## 1       < 1 glasses/day     ill
    ## 2       < 1 glasses/day     ill
    ## 3       < 1 glasses/day     ill
    ## 4       < 1 glasses/day     ill
    ## 5       < 1 glasses/day     ill
    ## 6       < 1 glasses/day     ill
    ## 7       < 1 glasses/day     ill
    ## 8       < 1 glasses/day     ill
    ## 9       < 1 glasses/day     ill
    ## 10      < 1 glasses/day     ill
    ## 11      < 1 glasses/day     ill
    ## 12      < 1 glasses/day     ill
    ## 13      < 1 glasses/day     ill
    ## 14      < 1 glasses/day     ill
    ## 15      < 1 glasses/day     ill
    ## 16      < 1 glasses/day     ill
    ## 17      < 1 glasses/day     ill
    ## 18      < 1 glasses/day     ill
    ## 19      < 1 glasses/day     ill
    ## 20      < 1 glasses/day     ill
    ## 21      < 1 glasses/day     ill
    ## 22      < 1 glasses/day     ill
    ## 23      < 1 glasses/day     ill
    ## 24      < 1 glasses/day     ill
    ## 25      < 1 glasses/day     ill
    ## 26      < 1 glasses/day     ill
    ## 27      < 1 glasses/day     ill
    ## 28      < 1 glasses/day     ill
    ## 29      < 1 glasses/day     ill
    ## 30      < 1 glasses/day     ill
    ## 31      < 1 glasses/day     ill
    ## 32      < 1 glasses/day     ill
    ## 33      < 1 glasses/day     ill
    ## 34      < 1 glasses/day     ill
    ## 35      < 1 glasses/day     ill
    ## 36      < 1 glasses/day     ill
    ## 37      < 1 glasses/day     ill
    ## 38      < 1 glasses/day     ill
    ## 39      < 1 glasses/day     ill
    ## 40      < 1 glasses/day not ill
    ## 41      < 1 glasses/day not ill
    ## 42      < 1 glasses/day not ill
    ## 43      < 1 glasses/day not ill
    ## 44      < 1 glasses/day not ill
    ## 45      < 1 glasses/day not ill
    ## 46      < 1 glasses/day not ill
    ## 47      < 1 glasses/day not ill
    ## 48      < 1 glasses/day not ill
    ## 49      < 1 glasses/day not ill
    ## 50      < 1 glasses/day not ill
    ## 51      < 1 glasses/day not ill
    ## 52      < 1 glasses/day not ill
    ## 53      < 1 glasses/day not ill
    ## 54      < 1 glasses/day not ill
    ## 55      < 1 glasses/day not ill
    ## 56      < 1 glasses/day not ill
    ## 57      < 1 glasses/day not ill
    ## 58      < 1 glasses/day not ill
    ## 59      < 1 glasses/day not ill
    ## 60      < 1 glasses/day not ill
    ## 61      < 1 glasses/day not ill
    ## 62      < 1 glasses/day not ill
    ## 63      < 1 glasses/day not ill
    ## 64      < 1 glasses/day not ill
    ## 65      < 1 glasses/day not ill
    ## 66      < 1 glasses/day not ill
    ## 67      < 1 glasses/day not ill
    ## 68      < 1 glasses/day not ill
    ## 69      < 1 glasses/day not ill
    ## 70      < 1 glasses/day not ill
    ## 71      < 1 glasses/day not ill
    ## 72      < 1 glasses/day not ill
    ## 73      < 1 glasses/day not ill
    ## 74      < 1 glasses/day not ill
    ## 75      < 1 glasses/day not ill
    ## 76      < 1 glasses/day not ill
    ## 77      < 1 glasses/day not ill
    ## 78      < 1 glasses/day not ill
    ## 79      < 1 glasses/day not ill
    ## 80      < 1 glasses/day not ill
    ## 81      < 1 glasses/day not ill
    ## 82      < 1 glasses/day not ill
    ## 83      < 1 glasses/day not ill
    ## 84      < 1 glasses/day not ill
    ## 85      < 1 glasses/day not ill
    ## 86      < 1 glasses/day not ill
    ## 87      < 1 glasses/day not ill
    ## 88      < 1 glasses/day not ill
    ## 89      < 1 glasses/day not ill
    ## 90      < 1 glasses/day not ill
    ## 91      < 1 glasses/day not ill
    ## 92      < 1 glasses/day not ill
    ## 93      < 1 glasses/day not ill
    ## 94      < 1 glasses/day not ill
    ## 95      < 1 glasses/day not ill
    ## 96      < 1 glasses/day not ill
    ## 97      < 1 glasses/day not ill
    ## 98      < 1 glasses/day not ill
    ## 99      < 1 glasses/day not ill
    ## 100     < 1 glasses/day not ill
    ## 101     < 1 glasses/day not ill
    ## 102     < 1 glasses/day not ill
    ## 103     < 1 glasses/day not ill
    ## 104     < 1 glasses/day not ill
    ## 105     < 1 glasses/day not ill
    ## 106     < 1 glasses/day not ill
    ## 107     < 1 glasses/day not ill
    ## 108     < 1 glasses/day not ill
    ## 109     < 1 glasses/day not ill
    ## 110     < 1 glasses/day not ill
    ## 111     < 1 glasses/day not ill
    ## 112     < 1 glasses/day not ill
    ## 113     < 1 glasses/day not ill
    ## 114     < 1 glasses/day not ill
    ## 115     < 1 glasses/day not ill
    ## 116     < 1 glasses/day not ill
    ## 117     < 1 glasses/day not ill
    ## 118     < 1 glasses/day not ill
    ## 119     < 1 glasses/day not ill
    ## 120     < 1 glasses/day not ill
    ## 121     < 1 glasses/day not ill
    ## 122     < 1 glasses/day not ill
    ## 123     < 1 glasses/day not ill
    ## 124     < 1 glasses/day not ill
    ## 125     < 1 glasses/day not ill
    ## 126     < 1 glasses/day not ill
    ## 127     < 1 glasses/day not ill
    ## 128     < 1 glasses/day not ill
    ## 129     < 1 glasses/day not ill
    ## 130     < 1 glasses/day not ill
    ## 131     < 1 glasses/day not ill
    ## 132     < 1 glasses/day not ill
    ## 133     < 1 glasses/day not ill
    ## 134     < 1 glasses/day not ill
    ## 135     < 1 glasses/day not ill
    ## 136     < 1 glasses/day not ill
    ## 137     < 1 glasses/day not ill
    ## 138     < 1 glasses/day not ill
    ## 139     < 1 glasses/day not ill
    ## 140     < 1 glasses/day not ill
    ## 141     < 1 glasses/day not ill
    ## 142     < 1 glasses/day not ill
    ## 143     < 1 glasses/day not ill
    ## 144     < 1 glasses/day not ill
    ## 145     < 1 glasses/day not ill
    ## 146     < 1 glasses/day not ill
    ## 147     < 1 glasses/day not ill
    ## 148     < 1 glasses/day not ill
    ## 149     < 1 glasses/day not ill
    ## 150     < 1 glasses/day not ill
    ## 151     < 1 glasses/day not ill
    ## 152     < 1 glasses/day not ill
    ## 153     < 1 glasses/day not ill
    ## 154     < 1 glasses/day not ill
    ## 155     < 1 glasses/day not ill
    ## 156     < 1 glasses/day not ill
    ## 157     < 1 glasses/day not ill
    ## 158     < 1 glasses/day not ill
    ## 159     < 1 glasses/day not ill
    ## 160     < 1 glasses/day not ill
    ## 161  1 to 4 glasses/day     ill
    ## 162  1 to 4 glasses/day     ill
    ## 163  1 to 4 glasses/day     ill
    ## 164  1 to 4 glasses/day     ill
    ## 165  1 to 4 glasses/day     ill
    ## 166  1 to 4 glasses/day     ill
    ## 167  1 to 4 glasses/day     ill
    ## 168  1 to 4 glasses/day     ill
    ## 169  1 to 4 glasses/day     ill
    ## 170  1 to 4 glasses/day     ill
    ## 171  1 to 4 glasses/day     ill
    ## 172  1 to 4 glasses/day     ill
    ## 173  1 to 4 glasses/day     ill
    ## 174  1 to 4 glasses/day     ill
    ## 175  1 to 4 glasses/day     ill
    ## 176  1 to 4 glasses/day     ill
    ## 177  1 to 4 glasses/day     ill
    ## 178  1 to 4 glasses/day     ill
    ## 179  1 to 4 glasses/day     ill
    ## 180  1 to 4 glasses/day     ill
    ## 181  1 to 4 glasses/day     ill
    ## 182  1 to 4 glasses/day     ill
    ## 183  1 to 4 glasses/day     ill
    ## 184  1 to 4 glasses/day     ill
    ## 185  1 to 4 glasses/day     ill
    ## 186  1 to 4 glasses/day     ill
    ## 187  1 to 4 glasses/day     ill
    ## 188  1 to 4 glasses/day     ill
    ## 189  1 to 4 glasses/day     ill
    ## 190  1 to 4 glasses/day     ill
    ## 191  1 to 4 glasses/day     ill
    ## 192  1 to 4 glasses/day     ill
    ## 193  1 to 4 glasses/day     ill
    ## 194  1 to 4 glasses/day     ill
    ## 195  1 to 4 glasses/day     ill
    ## 196  1 to 4 glasses/day     ill
    ## 197  1 to 4 glasses/day     ill
    ## 198  1 to 4 glasses/day     ill
    ## 199  1 to 4 glasses/day     ill
    ## 200  1 to 4 glasses/day     ill
    ## 201  1 to 4 glasses/day     ill
    ## 202  1 to 4 glasses/day     ill
    ## 203  1 to 4 glasses/day     ill
    ## 204  1 to 4 glasses/day     ill
    ## 205  1 to 4 glasses/day     ill
    ## 206  1 to 4 glasses/day     ill
    ## 207  1 to 4 glasses/day     ill
    ## 208  1 to 4 glasses/day     ill
    ## 209  1 to 4 glasses/day     ill
    ## 210  1 to 4 glasses/day     ill
    ## 211  1 to 4 glasses/day     ill
    ## 212  1 to 4 glasses/day     ill
    ## 213  1 to 4 glasses/day     ill
    ## 214  1 to 4 glasses/day     ill
    ## 215  1 to 4 glasses/day     ill
    ## 216  1 to 4 glasses/day     ill
    ## 217  1 to 4 glasses/day     ill
    ## 218  1 to 4 glasses/day     ill
    ## 219  1 to 4 glasses/day     ill
    ## 220  1 to 4 glasses/day     ill
    ## 221  1 to 4 glasses/day     ill
    ## 222  1 to 4 glasses/day     ill
    ## 223  1 to 4 glasses/day     ill
    ## 224  1 to 4 glasses/day     ill
    ## 225  1 to 4 glasses/day     ill
    ## 226  1 to 4 glasses/day     ill
    ## 227  1 to 4 glasses/day     ill
    ## 228  1 to 4 glasses/day     ill
    ## 229  1 to 4 glasses/day     ill
    ## 230  1 to 4 glasses/day     ill
    ## 231  1 to 4 glasses/day     ill
    ## 232  1 to 4 glasses/day     ill
    ## 233  1 to 4 glasses/day     ill
    ## 234  1 to 4 glasses/day     ill
    ## 235  1 to 4 glasses/day     ill
    ## 236  1 to 4 glasses/day     ill
    ## 237  1 to 4 glasses/day     ill
    ## 238  1 to 4 glasses/day     ill
    ## 239  1 to 4 glasses/day     ill
    ## 240  1 to 4 glasses/day     ill
    ## 241  1 to 4 glasses/day     ill
    ## 242  1 to 4 glasses/day     ill
    ## 243  1 to 4 glasses/day     ill
    ## 244  1 to 4 glasses/day     ill
    ## 245  1 to 4 glasses/day     ill
    ## 246  1 to 4 glasses/day     ill
    ## 247  1 to 4 glasses/day     ill
    ## 248  1 to 4 glasses/day     ill
    ## 249  1 to 4 glasses/day     ill
    ## 250  1 to 4 glasses/day     ill
    ## 251  1 to 4 glasses/day     ill
    ## 252  1 to 4 glasses/day     ill
    ## 253  1 to 4 glasses/day     ill
    ## 254  1 to 4 glasses/day     ill
    ## 255  1 to 4 glasses/day     ill
    ## 256  1 to 4 glasses/day     ill
    ## 257  1 to 4 glasses/day     ill
    ## 258  1 to 4 glasses/day     ill
    ## 259  1 to 4 glasses/day     ill
    ## 260  1 to 4 glasses/day     ill
    ## 261  1 to 4 glasses/day     ill
    ## 262  1 to 4 glasses/day     ill
    ## 263  1 to 4 glasses/day     ill
    ## 264  1 to 4 glasses/day     ill
    ## 265  1 to 4 glasses/day     ill
    ## 266  1 to 4 glasses/day     ill
    ## 267  1 to 4 glasses/day     ill
    ## 268  1 to 4 glasses/day     ill
    ## 269  1 to 4 glasses/day     ill
    ## 270  1 to 4 glasses/day     ill
    ## 271  1 to 4 glasses/day     ill
    ## 272  1 to 4 glasses/day     ill
    ## 273  1 to 4 glasses/day     ill
    ## 274  1 to 4 glasses/day     ill
    ## 275  1 to 4 glasses/day     ill
    ## 276  1 to 4 glasses/day     ill
    ## 277  1 to 4 glasses/day     ill
    ## 278  1 to 4 glasses/day     ill
    ## 279  1 to 4 glasses/day     ill
    ## 280  1 to 4 glasses/day     ill
    ## 281  1 to 4 glasses/day     ill
    ## 282  1 to 4 glasses/day     ill
    ## 283  1 to 4 glasses/day     ill
    ## 284  1 to 4 glasses/day     ill
    ## 285  1 to 4 glasses/day     ill
    ## 286  1 to 4 glasses/day     ill
    ## 287  1 to 4 glasses/day     ill
    ## 288  1 to 4 glasses/day     ill
    ## 289  1 to 4 glasses/day     ill
    ## 290  1 to 4 glasses/day     ill
    ## 291  1 to 4 glasses/day     ill
    ## 292  1 to 4 glasses/day     ill
    ## 293  1 to 4 glasses/day     ill
    ## 294  1 to 4 glasses/day     ill
    ## 295  1 to 4 glasses/day     ill
    ## 296  1 to 4 glasses/day     ill
    ## 297  1 to 4 glasses/day     ill
    ## 298  1 to 4 glasses/day     ill
    ## 299  1 to 4 glasses/day     ill
    ## 300  1 to 4 glasses/day     ill
    ## 301  1 to 4 glasses/day     ill
    ## 302  1 to 4 glasses/day     ill
    ## 303  1 to 4 glasses/day     ill
    ## 304  1 to 4 glasses/day     ill
    ## 305  1 to 4 glasses/day     ill
    ## 306  1 to 4 glasses/day     ill
    ## 307  1 to 4 glasses/day     ill
    ## 308  1 to 4 glasses/day     ill
    ## 309  1 to 4 glasses/day     ill
    ## 310  1 to 4 glasses/day     ill
    ## 311  1 to 4 glasses/day     ill
    ## 312  1 to 4 glasses/day     ill
    ## 313  1 to 4 glasses/day     ill
    ## 314  1 to 4 glasses/day     ill
    ## 315  1 to 4 glasses/day     ill
    ## 316  1 to 4 glasses/day     ill
    ## 317  1 to 4 glasses/day     ill
    ## 318  1 to 4 glasses/day     ill
    ## 319  1 to 4 glasses/day     ill
    ## 320  1 to 4 glasses/day     ill
    ## 321  1 to 4 glasses/day     ill
    ## 322  1 to 4 glasses/day     ill
    ## 323  1 to 4 glasses/day     ill
    ## 324  1 to 4 glasses/day     ill
    ## 325  1 to 4 glasses/day     ill
    ## 326  1 to 4 glasses/day     ill
    ## 327  1 to 4 glasses/day     ill
    ## 328  1 to 4 glasses/day     ill
    ## 329  1 to 4 glasses/day     ill
    ## 330  1 to 4 glasses/day     ill
    ## 331  1 to 4 glasses/day     ill
    ## 332  1 to 4 glasses/day     ill
    ## 333  1 to 4 glasses/day     ill
    ## 334  1 to 4 glasses/day     ill
    ## 335  1 to 4 glasses/day     ill
    ## 336  1 to 4 glasses/day     ill
    ## 337  1 to 4 glasses/day     ill
    ## 338  1 to 4 glasses/day     ill
    ## 339  1 to 4 glasses/day     ill
    ## 340  1 to 4 glasses/day     ill
    ## 341  1 to 4 glasses/day     ill
    ## 342  1 to 4 glasses/day     ill
    ## 343  1 to 4 glasses/day     ill
    ## 344  1 to 4 glasses/day     ill
    ## 345  1 to 4 glasses/day     ill
    ## 346  1 to 4 glasses/day     ill
    ## 347  1 to 4 glasses/day     ill
    ## 348  1 to 4 glasses/day     ill
    ## 349  1 to 4 glasses/day     ill
    ## 350  1 to 4 glasses/day     ill
    ## 351  1 to 4 glasses/day     ill
    ## 352  1 to 4 glasses/day     ill
    ## 353  1 to 4 glasses/day     ill
    ## 354  1 to 4 glasses/day     ill
    ## 355  1 to 4 glasses/day     ill
    ## 356  1 to 4 glasses/day     ill
    ## 357  1 to 4 glasses/day     ill
    ## 358  1 to 4 glasses/day     ill
    ## 359  1 to 4 glasses/day     ill
    ## 360  1 to 4 glasses/day     ill
    ## 361  1 to 4 glasses/day     ill
    ## 362  1 to 4 glasses/day     ill
    ## 363  1 to 4 glasses/day     ill
    ## 364  1 to 4 glasses/day     ill
    ## 365  1 to 4 glasses/day     ill
    ## 366  1 to 4 glasses/day     ill
    ## 367  1 to 4 glasses/day     ill
    ## 368  1 to 4 glasses/day     ill
    ## 369  1 to 4 glasses/day     ill
    ## 370  1 to 4 glasses/day     ill
    ## 371  1 to 4 glasses/day     ill
    ## 372  1 to 4 glasses/day     ill
    ## 373  1 to 4 glasses/day     ill
    ## 374  1 to 4 glasses/day     ill
    ## 375  1 to 4 glasses/day     ill
    ## 376  1 to 4 glasses/day     ill
    ## 377  1 to 4 glasses/day     ill
    ## 378  1 to 4 glasses/day     ill
    ## 379  1 to 4 glasses/day     ill
    ## 380  1 to 4 glasses/day     ill
    ## 381  1 to 4 glasses/day     ill
    ## 382  1 to 4 glasses/day     ill
    ## 383  1 to 4 glasses/day     ill
    ## 384  1 to 4 glasses/day     ill
    ## 385  1 to 4 glasses/day     ill
    ## 386  1 to 4 glasses/day     ill
    ## 387  1 to 4 glasses/day     ill
    ## 388  1 to 4 glasses/day     ill
    ## 389  1 to 4 glasses/day     ill
    ## 390  1 to 4 glasses/day     ill
    ## 391  1 to 4 glasses/day     ill
    ## 392  1 to 4 glasses/day     ill
    ## 393  1 to 4 glasses/day     ill
    ## 394  1 to 4 glasses/day     ill
    ## 395  1 to 4 glasses/day     ill
    ## 396  1 to 4 glasses/day     ill
    ## 397  1 to 4 glasses/day     ill
    ## 398  1 to 4 glasses/day     ill
    ## 399  1 to 4 glasses/day     ill
    ## 400  1 to 4 glasses/day     ill
    ## 401  1 to 4 glasses/day     ill
    ## 402  1 to 4 glasses/day     ill
    ## 403  1 to 4 glasses/day     ill
    ## 404  1 to 4 glasses/day     ill
    ## 405  1 to 4 glasses/day     ill
    ## 406  1 to 4 glasses/day     ill
    ## 407  1 to 4 glasses/day     ill
    ## 408  1 to 4 glasses/day     ill
    ## 409  1 to 4 glasses/day     ill
    ## 410  1 to 4 glasses/day     ill
    ## 411  1 to 4 glasses/day     ill
    ## 412  1 to 4 glasses/day     ill
    ## 413  1 to 4 glasses/day     ill
    ## 414  1 to 4 glasses/day     ill
    ## 415  1 to 4 glasses/day     ill
    ## 416  1 to 4 glasses/day     ill
    ## 417  1 to 4 glasses/day     ill
    ## 418  1 to 4 glasses/day     ill
    ## 419  1 to 4 glasses/day     ill
    ## 420  1 to 4 glasses/day     ill
    ## 421  1 to 4 glasses/day     ill
    ## 422  1 to 4 glasses/day     ill
    ## 423  1 to 4 glasses/day     ill
    ## 424  1 to 4 glasses/day     ill
    ## 425  1 to 4 glasses/day     ill
    ## 426  1 to 4 glasses/day not ill
    ## 427  1 to 4 glasses/day not ill
    ## 428  1 to 4 glasses/day not ill
    ## 429  1 to 4 glasses/day not ill
    ## 430  1 to 4 glasses/day not ill
    ## 431  1 to 4 glasses/day not ill
    ## 432  1 to 4 glasses/day not ill
    ## 433  1 to 4 glasses/day not ill
    ## 434  1 to 4 glasses/day not ill
    ## 435  1 to 4 glasses/day not ill
    ## 436  1 to 4 glasses/day not ill
    ## 437  1 to 4 glasses/day not ill
    ## 438  1 to 4 glasses/day not ill
    ## 439  1 to 4 glasses/day not ill
    ## 440  1 to 4 glasses/day not ill
    ## 441  1 to 4 glasses/day not ill
    ## 442  1 to 4 glasses/day not ill
    ## 443  1 to 4 glasses/day not ill
    ## 444  1 to 4 glasses/day not ill
    ## 445  1 to 4 glasses/day not ill
    ## 446  1 to 4 glasses/day not ill
    ## 447  1 to 4 glasses/day not ill
    ## 448  1 to 4 glasses/day not ill
    ## 449  1 to 4 glasses/day not ill
    ## 450  1 to 4 glasses/day not ill
    ## 451  1 to 4 glasses/day not ill
    ## 452  1 to 4 glasses/day not ill
    ## 453  1 to 4 glasses/day not ill
    ## 454  1 to 4 glasses/day not ill
    ## 455  1 to 4 glasses/day not ill
    ## 456  1 to 4 glasses/day not ill
    ## 457  1 to 4 glasses/day not ill
    ## 458  1 to 4 glasses/day not ill
    ## 459  1 to 4 glasses/day not ill
    ## 460  1 to 4 glasses/day not ill
    ## 461  1 to 4 glasses/day not ill
    ## 462  1 to 4 glasses/day not ill
    ## 463  1 to 4 glasses/day not ill
    ## 464  1 to 4 glasses/day not ill
    ## 465  1 to 4 glasses/day not ill
    ## 466  1 to 4 glasses/day not ill
    ## 467  1 to 4 glasses/day not ill
    ## 468  1 to 4 glasses/day not ill
    ## 469  1 to 4 glasses/day not ill
    ## 470  1 to 4 glasses/day not ill
    ## 471  1 to 4 glasses/day not ill
    ## 472  1 to 4 glasses/day not ill
    ## 473  1 to 4 glasses/day not ill
    ## 474  1 to 4 glasses/day not ill
    ## 475  1 to 4 glasses/day not ill
    ## 476  1 to 4 glasses/day not ill
    ## 477  1 to 4 glasses/day not ill
    ## 478  1 to 4 glasses/day not ill
    ## 479  1 to 4 glasses/day not ill
    ## 480  1 to 4 glasses/day not ill
    ## 481  1 to 4 glasses/day not ill
    ## 482  1 to 4 glasses/day not ill
    ## 483  1 to 4 glasses/day not ill
    ## 484  1 to 4 glasses/day not ill
    ## 485  1 to 4 glasses/day not ill
    ## 486  1 to 4 glasses/day not ill
    ## 487  1 to 4 glasses/day not ill
    ## 488  1 to 4 glasses/day not ill
    ## 489  1 to 4 glasses/day not ill
    ## 490  1 to 4 glasses/day not ill
    ## 491  1 to 4 glasses/day not ill
    ## 492  1 to 4 glasses/day not ill
    ## 493  1 to 4 glasses/day not ill
    ## 494  1 to 4 glasses/day not ill
    ## 495  1 to 4 glasses/day not ill
    ## 496  1 to 4 glasses/day not ill
    ## 497  1 to 4 glasses/day not ill
    ## 498  1 to 4 glasses/day not ill
    ## 499  1 to 4 glasses/day not ill
    ## 500  1 to 4 glasses/day not ill
    ## 501  1 to 4 glasses/day not ill
    ## 502  1 to 4 glasses/day not ill
    ## 503  1 to 4 glasses/day not ill
    ## 504  1 to 4 glasses/day not ill
    ## 505  1 to 4 glasses/day not ill
    ## 506  1 to 4 glasses/day not ill
    ## 507  1 to 4 glasses/day not ill
    ## 508  1 to 4 glasses/day not ill
    ## 509  1 to 4 glasses/day not ill
    ## 510  1 to 4 glasses/day not ill
    ## 511  1 to 4 glasses/day not ill
    ## 512  1 to 4 glasses/day not ill
    ## 513  1 to 4 glasses/day not ill
    ## 514  1 to 4 glasses/day not ill
    ## 515  1 to 4 glasses/day not ill
    ## 516  1 to 4 glasses/day not ill
    ## 517  1 to 4 glasses/day not ill
    ## 518  1 to 4 glasses/day not ill
    ## 519  1 to 4 glasses/day not ill
    ## 520  1 to 4 glasses/day not ill
    ## 521  1 to 4 glasses/day not ill
    ## 522  1 to 4 glasses/day not ill
    ## 523  1 to 4 glasses/day not ill
    ## 524  1 to 4 glasses/day not ill
    ## 525  1 to 4 glasses/day not ill
    ## 526  1 to 4 glasses/day not ill
    ## 527  1 to 4 glasses/day not ill
    ## 528  1 to 4 glasses/day not ill
    ## 529  1 to 4 glasses/day not ill
    ## 530  1 to 4 glasses/day not ill
    ## 531  1 to 4 glasses/day not ill
    ## 532  1 to 4 glasses/day not ill
    ## 533  1 to 4 glasses/day not ill
    ## 534  1 to 4 glasses/day not ill
    ## 535  1 to 4 glasses/day not ill
    ## 536  1 to 4 glasses/day not ill
    ## 537  1 to 4 glasses/day not ill
    ## 538  1 to 4 glasses/day not ill
    ## 539  1 to 4 glasses/day not ill
    ## 540  1 to 4 glasses/day not ill
    ## 541  1 to 4 glasses/day not ill
    ## 542  1 to 4 glasses/day not ill
    ## 543  1 to 4 glasses/day not ill
    ## 544  1 to 4 glasses/day not ill
    ## 545  1 to 4 glasses/day not ill
    ## 546  1 to 4 glasses/day not ill
    ## 547  1 to 4 glasses/day not ill
    ## 548  1 to 4 glasses/day not ill
    ## 549  1 to 4 glasses/day not ill
    ## 550  1 to 4 glasses/day not ill
    ## 551  1 to 4 glasses/day not ill
    ## 552  1 to 4 glasses/day not ill
    ## 553  1 to 4 glasses/day not ill
    ## 554  1 to 4 glasses/day not ill
    ## 555  1 to 4 glasses/day not ill
    ## 556  1 to 4 glasses/day not ill
    ## 557  1 to 4 glasses/day not ill
    ## 558  1 to 4 glasses/day not ill
    ## 559  1 to 4 glasses/day not ill
    ## 560  1 to 4 glasses/day not ill
    ## 561  1 to 4 glasses/day not ill
    ## 562  1 to 4 glasses/day not ill
    ## 563  1 to 4 glasses/day not ill
    ## 564  1 to 4 glasses/day not ill
    ## 565  1 to 4 glasses/day not ill
    ## 566  1 to 4 glasses/day not ill
    ## 567  1 to 4 glasses/day not ill
    ## 568  1 to 4 glasses/day not ill
    ## 569  1 to 4 glasses/day not ill
    ## 570  1 to 4 glasses/day not ill
    ## 571  1 to 4 glasses/day not ill
    ## 572  1 to 4 glasses/day not ill
    ## 573  1 to 4 glasses/day not ill
    ## 574  1 to 4 glasses/day not ill
    ## 575  1 to 4 glasses/day not ill
    ## 576  1 to 4 glasses/day not ill
    ## 577  1 to 4 glasses/day not ill
    ## 578  1 to 4 glasses/day not ill
    ## 579  1 to 4 glasses/day not ill
    ## 580  1 to 4 glasses/day not ill
    ## 581  1 to 4 glasses/day not ill
    ## 582  1 to 4 glasses/day not ill
    ## 583  1 to 4 glasses/day not ill
    ## 584  1 to 4 glasses/day not ill
    ## 585  1 to 4 glasses/day not ill
    ## 586  1 to 4 glasses/day not ill
    ## 587  1 to 4 glasses/day not ill
    ## 588  1 to 4 glasses/day not ill
    ## 589  1 to 4 glasses/day not ill
    ## 590  1 to 4 glasses/day not ill
    ## 591  1 to 4 glasses/day not ill
    ## 592  1 to 4 glasses/day not ill
    ## 593  1 to 4 glasses/day not ill
    ## 594  1 to 4 glasses/day not ill
    ## 595  1 to 4 glasses/day not ill
    ## 596  1 to 4 glasses/day not ill
    ## 597  1 to 4 glasses/day not ill
    ## 598  1 to 4 glasses/day not ill
    ## 599  1 to 4 glasses/day not ill
    ## 600  1 to 4 glasses/day not ill
    ## 601  1 to 4 glasses/day not ill
    ## 602  1 to 4 glasses/day not ill
    ## 603  1 to 4 glasses/day not ill
    ## 604  1 to 4 glasses/day not ill
    ## 605  1 to 4 glasses/day not ill
    ## 606  1 to 4 glasses/day not ill
    ## 607  1 to 4 glasses/day not ill
    ## 608  1 to 4 glasses/day not ill
    ## 609  1 to 4 glasses/day not ill
    ## 610  1 to 4 glasses/day not ill
    ## 611  1 to 4 glasses/day not ill
    ## 612  1 to 4 glasses/day not ill
    ## 613  1 to 4 glasses/day not ill
    ## 614  1 to 4 glasses/day not ill
    ## 615  1 to 4 glasses/day not ill
    ## 616  1 to 4 glasses/day not ill
    ## 617  1 to 4 glasses/day not ill
    ## 618  1 to 4 glasses/day not ill
    ## 619  1 to 4 glasses/day not ill
    ## 620  1 to 4 glasses/day not ill
    ## 621  1 to 4 glasses/day not ill
    ## 622  1 to 4 glasses/day not ill
    ## 623  1 to 4 glasses/day not ill
    ## 624  1 to 4 glasses/day not ill
    ## 625  1 to 4 glasses/day not ill
    ## 626  1 to 4 glasses/day not ill
    ## 627  1 to 4 glasses/day not ill
    ## 628  1 to 4 glasses/day not ill
    ## 629  1 to 4 glasses/day not ill
    ## 630  1 to 4 glasses/day not ill
    ## 631  1 to 4 glasses/day not ill
    ## 632  1 to 4 glasses/day not ill
    ## 633  1 to 4 glasses/day not ill
    ## 634  1 to 4 glasses/day not ill
    ## 635  1 to 4 glasses/day not ill
    ## 636  1 to 4 glasses/day not ill
    ## 637  1 to 4 glasses/day not ill
    ## 638  1 to 4 glasses/day not ill
    ## 639  1 to 4 glasses/day not ill
    ## 640  1 to 4 glasses/day not ill
    ## 641  1 to 4 glasses/day not ill
    ## 642  1 to 4 glasses/day not ill
    ## 643  1 to 4 glasses/day not ill
    ## 644  1 to 4 glasses/day not ill
    ## 645  1 to 4 glasses/day not ill
    ## 646  1 to 4 glasses/day not ill
    ## 647  1 to 4 glasses/day not ill
    ## 648  1 to 4 glasses/day not ill
    ## 649  1 to 4 glasses/day not ill
    ## 650  1 to 4 glasses/day not ill
    ## 651  1 to 4 glasses/day not ill
    ## 652  1 to 4 glasses/day not ill
    ## 653  1 to 4 glasses/day not ill
    ## 654  1 to 4 glasses/day not ill
    ## 655  1 to 4 glasses/day not ill
    ## 656  1 to 4 glasses/day not ill
    ## 657  1 to 4 glasses/day not ill
    ## 658  1 to 4 glasses/day not ill
    ## 659  1 to 4 glasses/day not ill
    ## 660  1 to 4 glasses/day not ill
    ## 661  1 to 4 glasses/day not ill
    ## 662  1 to 4 glasses/day not ill
    ## 663  1 to 4 glasses/day not ill
    ## 664  1 to 4 glasses/day not ill
    ## 665  1 to 4 glasses/day not ill
    ## 666  1 to 4 glasses/day not ill
    ## 667  1 to 4 glasses/day not ill
    ## 668  1 to 4 glasses/day not ill
    ## 669  1 to 4 glasses/day not ill
    ## 670  1 to 4 glasses/day not ill
    ## 671  1 to 4 glasses/day not ill
    ## 672  1 to 4 glasses/day not ill
    ## 673  1 to 4 glasses/day not ill
    ## 674  1 to 4 glasses/day not ill
    ## 675  1 to 4 glasses/day not ill
    ## 676  1 to 4 glasses/day not ill
    ## 677  1 to 4 glasses/day not ill
    ## 678  1 to 4 glasses/day not ill
    ## 679  1 to 4 glasses/day not ill
    ## 680  1 to 4 glasses/day not ill
    ## 681  1 to 4 glasses/day not ill
    ## 682  1 to 4 glasses/day not ill
    ## 683  1 to 4 glasses/day not ill
    ## 684     > 4 glasses/day     ill
    ## 685     > 4 glasses/day     ill
    ## 686     > 4 glasses/day     ill
    ## 687     > 4 glasses/day     ill
    ## 688     > 4 glasses/day     ill
    ## 689     > 4 glasses/day     ill
    ## 690     > 4 glasses/day     ill
    ## 691     > 4 glasses/day     ill
    ## 692     > 4 glasses/day     ill
    ## 693     > 4 glasses/day     ill
    ## 694     > 4 glasses/day     ill
    ## 695     > 4 glasses/day     ill
    ## 696     > 4 glasses/day     ill
    ## 697     > 4 glasses/day     ill
    ## 698     > 4 glasses/day     ill
    ## 699     > 4 glasses/day     ill
    ## 700     > 4 glasses/day     ill
    ## 701     > 4 glasses/day     ill
    ## 702     > 4 glasses/day     ill
    ## 703     > 4 glasses/day     ill
    ## 704     > 4 glasses/day     ill
    ## 705     > 4 glasses/day     ill
    ## 706     > 4 glasses/day     ill
    ## 707     > 4 glasses/day     ill
    ## 708     > 4 glasses/day     ill
    ## 709     > 4 glasses/day     ill
    ## 710     > 4 glasses/day     ill
    ## 711     > 4 glasses/day     ill
    ## 712     > 4 glasses/day     ill
    ## 713     > 4 glasses/day     ill
    ## 714     > 4 glasses/day     ill
    ## 715     > 4 glasses/day     ill
    ## 716     > 4 glasses/day     ill
    ## 717     > 4 glasses/day     ill
    ## 718     > 4 glasses/day     ill
    ## 719     > 4 glasses/day     ill
    ## 720     > 4 glasses/day     ill
    ## 721     > 4 glasses/day     ill
    ## 722     > 4 glasses/day     ill
    ## 723     > 4 glasses/day     ill
    ## 724     > 4 glasses/day     ill
    ## 725     > 4 glasses/day     ill
    ## 726     > 4 glasses/day     ill
    ## 727     > 4 glasses/day     ill
    ## 728     > 4 glasses/day     ill
    ## 729     > 4 glasses/day     ill
    ## 730     > 4 glasses/day     ill
    ## 731     > 4 glasses/day     ill
    ## 732     > 4 glasses/day     ill
    ## 733     > 4 glasses/day     ill
    ## 734     > 4 glasses/day     ill
    ## 735     > 4 glasses/day     ill
    ## 736     > 4 glasses/day     ill
    ## 737     > 4 glasses/day     ill
    ## 738     > 4 glasses/day     ill
    ## 739     > 4 glasses/day     ill
    ## 740     > 4 glasses/day     ill
    ## 741     > 4 glasses/day     ill
    ## 742     > 4 glasses/day     ill
    ## 743     > 4 glasses/day     ill
    ## 744     > 4 glasses/day     ill
    ## 745     > 4 glasses/day     ill
    ## 746     > 4 glasses/day     ill
    ## 747     > 4 glasses/day     ill
    ## 748     > 4 glasses/day     ill
    ## 749     > 4 glasses/day     ill
    ## 750     > 4 glasses/day     ill
    ## 751     > 4 glasses/day     ill
    ## 752     > 4 glasses/day     ill
    ## 753     > 4 glasses/day     ill
    ## 754     > 4 glasses/day     ill
    ## 755     > 4 glasses/day     ill
    ## 756     > 4 glasses/day     ill
    ## 757     > 4 glasses/day     ill
    ## 758     > 4 glasses/day     ill
    ## 759     > 4 glasses/day     ill
    ## 760     > 4 glasses/day     ill
    ## 761     > 4 glasses/day     ill
    ## 762     > 4 glasses/day     ill
    ## 763     > 4 glasses/day     ill
    ## 764     > 4 glasses/day     ill
    ## 765     > 4 glasses/day     ill
    ## 766     > 4 glasses/day     ill
    ## 767     > 4 glasses/day     ill
    ## 768     > 4 glasses/day     ill
    ## 769     > 4 glasses/day     ill
    ## 770     > 4 glasses/day     ill
    ## 771     > 4 glasses/day     ill
    ## 772     > 4 glasses/day     ill
    ## 773     > 4 glasses/day     ill
    ## 774     > 4 glasses/day     ill
    ## 775     > 4 glasses/day     ill
    ## 776     > 4 glasses/day     ill
    ## 777     > 4 glasses/day     ill
    ## 778     > 4 glasses/day     ill
    ## 779     > 4 glasses/day     ill
    ## 780     > 4 glasses/day     ill
    ## 781     > 4 glasses/day     ill
    ## 782     > 4 glasses/day     ill
    ## 783     > 4 glasses/day     ill
    ## 784     > 4 glasses/day     ill
    ## 785     > 4 glasses/day     ill
    ## 786     > 4 glasses/day     ill
    ## 787     > 4 glasses/day     ill
    ## 788     > 4 glasses/day     ill
    ## 789     > 4 glasses/day     ill
    ## 790     > 4 glasses/day     ill
    ## 791     > 4 glasses/day     ill
    ## 792     > 4 glasses/day     ill
    ## 793     > 4 glasses/day     ill
    ## 794     > 4 glasses/day     ill
    ## 795     > 4 glasses/day     ill
    ## 796     > 4 glasses/day     ill
    ## 797     > 4 glasses/day     ill
    ## 798     > 4 glasses/day     ill
    ## 799     > 4 glasses/day     ill
    ## 800     > 4 glasses/day     ill
    ## 801     > 4 glasses/day     ill
    ## 802     > 4 glasses/day     ill
    ## 803     > 4 glasses/day     ill
    ## 804     > 4 glasses/day     ill
    ## 805     > 4 glasses/day     ill
    ## 806     > 4 glasses/day     ill
    ## 807     > 4 glasses/day     ill
    ## 808     > 4 glasses/day     ill
    ## 809     > 4 glasses/day     ill
    ## 810     > 4 glasses/day     ill
    ## 811     > 4 glasses/day     ill
    ## 812     > 4 glasses/day     ill
    ## 813     > 4 glasses/day     ill
    ## 814     > 4 glasses/day     ill
    ## 815     > 4 glasses/day     ill
    ## 816     > 4 glasses/day     ill
    ## 817     > 4 glasses/day     ill
    ## 818     > 4 glasses/day     ill
    ## 819     > 4 glasses/day     ill
    ## 820     > 4 glasses/day     ill
    ## 821     > 4 glasses/day     ill
    ## 822     > 4 glasses/day     ill
    ## 823     > 4 glasses/day     ill
    ## 824     > 4 glasses/day     ill
    ## 825     > 4 glasses/day     ill
    ## 826     > 4 glasses/day     ill
    ## 827     > 4 glasses/day     ill
    ## 828     > 4 glasses/day     ill
    ## 829     > 4 glasses/day     ill
    ## 830     > 4 glasses/day     ill
    ## 831     > 4 glasses/day     ill
    ## 832     > 4 glasses/day     ill
    ## 833     > 4 glasses/day     ill
    ## 834     > 4 glasses/day     ill
    ## 835     > 4 glasses/day     ill
    ## 836     > 4 glasses/day     ill
    ## 837     > 4 glasses/day     ill
    ## 838     > 4 glasses/day     ill
    ## 839     > 4 glasses/day     ill
    ## 840     > 4 glasses/day     ill
    ## 841     > 4 glasses/day     ill
    ## 842     > 4 glasses/day     ill
    ## 843     > 4 glasses/day     ill
    ## 844     > 4 glasses/day     ill
    ## 845     > 4 glasses/day     ill
    ## 846     > 4 glasses/day     ill
    ## 847     > 4 glasses/day     ill
    ## 848     > 4 glasses/day     ill
    ## 849     > 4 glasses/day     ill
    ## 850     > 4 glasses/day     ill
    ## 851     > 4 glasses/day     ill
    ## 852     > 4 glasses/day     ill
    ## 853     > 4 glasses/day     ill
    ## 854     > 4 glasses/day     ill
    ## 855     > 4 glasses/day     ill
    ## 856     > 4 glasses/day     ill
    ## 857     > 4 glasses/day     ill
    ## 858     > 4 glasses/day     ill
    ## 859     > 4 glasses/day     ill
    ## 860     > 4 glasses/day     ill
    ## 861     > 4 glasses/day     ill
    ## 862     > 4 glasses/day     ill
    ## 863     > 4 glasses/day     ill
    ## 864     > 4 glasses/day     ill
    ## 865     > 4 glasses/day     ill
    ## 866     > 4 glasses/day     ill
    ## 867     > 4 glasses/day     ill
    ## 868     > 4 glasses/day     ill
    ## 869     > 4 glasses/day     ill
    ## 870     > 4 glasses/day     ill
    ## 871     > 4 glasses/day     ill
    ## 872     > 4 glasses/day     ill
    ## 873     > 4 glasses/day     ill
    ## 874     > 4 glasses/day     ill
    ## 875     > 4 glasses/day     ill
    ## 876     > 4 glasses/day     ill
    ## 877     > 4 glasses/day     ill
    ## 878     > 4 glasses/day     ill
    ## 879     > 4 glasses/day     ill
    ## 880     > 4 glasses/day     ill
    ## 881     > 4 glasses/day     ill
    ## 882     > 4 glasses/day     ill
    ## 883     > 4 glasses/day     ill
    ## 884     > 4 glasses/day     ill
    ## 885     > 4 glasses/day     ill
    ## 886     > 4 glasses/day     ill
    ## 887     > 4 glasses/day     ill
    ## 888     > 4 glasses/day     ill
    ## 889     > 4 glasses/day     ill
    ## 890     > 4 glasses/day     ill
    ## 891     > 4 glasses/day     ill
    ## 892     > 4 glasses/day     ill
    ## 893     > 4 glasses/day     ill
    ## 894     > 4 glasses/day     ill
    ## 895     > 4 glasses/day     ill
    ## 896     > 4 glasses/day     ill
    ## 897     > 4 glasses/day     ill
    ## 898     > 4 glasses/day     ill
    ## 899     > 4 glasses/day     ill
    ## 900     > 4 glasses/day     ill
    ## 901     > 4 glasses/day     ill
    ## 902     > 4 glasses/day     ill
    ## 903     > 4 glasses/day     ill
    ## 904     > 4 glasses/day     ill
    ## 905     > 4 glasses/day     ill
    ## 906     > 4 glasses/day     ill
    ## 907     > 4 glasses/day     ill
    ## 908     > 4 glasses/day     ill
    ## 909     > 4 glasses/day     ill
    ## 910     > 4 glasses/day     ill
    ## 911     > 4 glasses/day     ill
    ## 912     > 4 glasses/day     ill
    ## 913     > 4 glasses/day     ill
    ## 914     > 4 glasses/day     ill
    ## 915     > 4 glasses/day     ill
    ## 916     > 4 glasses/day     ill
    ## 917     > 4 glasses/day     ill
    ## 918     > 4 glasses/day     ill
    ## 919     > 4 glasses/day     ill
    ## 920     > 4 glasses/day     ill
    ## 921     > 4 glasses/day     ill
    ## 922     > 4 glasses/day     ill
    ## 923     > 4 glasses/day     ill
    ## 924     > 4 glasses/day     ill
    ## 925     > 4 glasses/day     ill
    ## 926     > 4 glasses/day     ill
    ## 927     > 4 glasses/day     ill
    ## 928     > 4 glasses/day     ill
    ## 929     > 4 glasses/day     ill
    ## 930     > 4 glasses/day     ill
    ## 931     > 4 glasses/day     ill
    ## 932     > 4 glasses/day     ill
    ## 933     > 4 glasses/day     ill
    ## 934     > 4 glasses/day     ill
    ## 935     > 4 glasses/day     ill
    ## 936     > 4 glasses/day     ill
    ## 937     > 4 glasses/day     ill
    ## 938     > 4 glasses/day     ill
    ## 939     > 4 glasses/day     ill
    ## 940     > 4 glasses/day     ill
    ## 941     > 4 glasses/day     ill
    ## 942     > 4 glasses/day     ill
    ## 943     > 4 glasses/day     ill
    ## 944     > 4 glasses/day     ill
    ## 945     > 4 glasses/day     ill
    ## 946     > 4 glasses/day     ill
    ## 947     > 4 glasses/day     ill
    ## 948     > 4 glasses/day     ill
    ## 949     > 4 glasses/day not ill
    ## 950     > 4 glasses/day not ill
    ## 951     > 4 glasses/day not ill
    ## 952     > 4 glasses/day not ill
    ## 953     > 4 glasses/day not ill
    ## 954     > 4 glasses/day not ill
    ## 955     > 4 glasses/day not ill
    ## 956     > 4 glasses/day not ill
    ## 957     > 4 glasses/day not ill
    ## 958     > 4 glasses/day not ill
    ## 959     > 4 glasses/day not ill
    ## 960     > 4 glasses/day not ill
    ## 961     > 4 glasses/day not ill
    ## 962     > 4 glasses/day not ill
    ## 963     > 4 glasses/day not ill
    ## 964     > 4 glasses/day not ill
    ## 965     > 4 glasses/day not ill
    ## 966     > 4 glasses/day not ill
    ## 967     > 4 glasses/day not ill
    ## 968     > 4 glasses/day not ill
    ## 969     > 4 glasses/day not ill
    ## 970     > 4 glasses/day not ill
    ## 971     > 4 glasses/day not ill
    ## 972     > 4 glasses/day not ill
    ## 973     > 4 glasses/day not ill
    ## 974     > 4 glasses/day not ill
    ## 975     > 4 glasses/day not ill
    ## 976     > 4 glasses/day not ill
    ## 977     > 4 glasses/day not ill
    ## 978     > 4 glasses/day not ill
    ## 979     > 4 glasses/day not ill
    ## 980     > 4 glasses/day not ill
    ## 981     > 4 glasses/day not ill
    ## 982     > 4 glasses/day not ill
    ## 983     > 4 glasses/day not ill
    ## 984     > 4 glasses/day not ill
    ## 985     > 4 glasses/day not ill
    ## 986     > 4 glasses/day not ill
    ## 987     > 4 glasses/day not ill
    ## 988     > 4 glasses/day not ill
    ## 989     > 4 glasses/day not ill
    ## 990     > 4 glasses/day not ill
    ## 991     > 4 glasses/day not ill
    ## 992     > 4 glasses/day not ill
    ## 993     > 4 glasses/day not ill
    ## 994     > 4 glasses/day not ill
    ## 995     > 4 glasses/day not ill
    ## 996     > 4 glasses/day not ill
    ## 997     > 4 glasses/day not ill
    ## 998     > 4 glasses/day not ill
    ## 999     > 4 glasses/day not ill
    ## 1000    > 4 glasses/day not ill
    ## 1001    > 4 glasses/day not ill
    ## 1002    > 4 glasses/day not ill
    ## 1003    > 4 glasses/day not ill
    ## 1004    > 4 glasses/day not ill
    ## 1005    > 4 glasses/day not ill
    ## 1006    > 4 glasses/day not ill
    ## 1007    > 4 glasses/day not ill
    ## 1008    > 4 glasses/day not ill
    ## 1009    > 4 glasses/day not ill
    ## 1010    > 4 glasses/day not ill
    ## 1011    > 4 glasses/day not ill
    ## 1012    > 4 glasses/day not ill
    ## 1013    > 4 glasses/day not ill
    ## 1014    > 4 glasses/day not ill
    ## 1015    > 4 glasses/day not ill
    ## 1016    > 4 glasses/day not ill
    ## 1017    > 4 glasses/day not ill
    ## 1018    > 4 glasses/day not ill
    ## 1019    > 4 glasses/day not ill
    ## 1020    > 4 glasses/day not ill
    ## 1021    > 4 glasses/day not ill
    ## 1022    > 4 glasses/day not ill
    ## 1023    > 4 glasses/day not ill
    ## 1024    > 4 glasses/day not ill
    ## 1025    > 4 glasses/day not ill
    ## 1026    > 4 glasses/day not ill
    ## 1027    > 4 glasses/day not ill
    ## 1028    > 4 glasses/day not ill
    ## 1029    > 4 glasses/day not ill
    ## 1030    > 4 glasses/day not ill
    ## 1031    > 4 glasses/day not ill
    ## 1032    > 4 glasses/day not ill
    ## 1033    > 4 glasses/day not ill
    ## 1034    > 4 glasses/day not ill
    ## 1035    > 4 glasses/day not ill
    ## 1036    > 4 glasses/day not ill
    ## 1037    > 4 glasses/day not ill
    ## 1038    > 4 glasses/day not ill
    ## 1039    > 4 glasses/day not ill
    ## 1040    > 4 glasses/day not ill
    ## 1041    > 4 glasses/day not ill
    ## 1042    > 4 glasses/day not ill
    ## 1043    > 4 glasses/day not ill
    ## 1044    > 4 glasses/day not ill
    ## 1045    > 4 glasses/day not ill
    ## 1046    > 4 glasses/day not ill
    ## 1047    > 4 glasses/day not ill
    ## 1048    > 4 glasses/day not ill
    ## 1049    > 4 glasses/day not ill
    ## 1050    > 4 glasses/day not ill
    ## 1051    > 4 glasses/day not ill
    ## 1052    > 4 glasses/day not ill
    ## 1053    > 4 glasses/day not ill
    ## 1054    > 4 glasses/day not ill
    ## 1055    > 4 glasses/day not ill
    ## 1056    > 4 glasses/day not ill
    ## 1057    > 4 glasses/day not ill
    ## 1058    > 4 glasses/day not ill
    ## 1059    > 4 glasses/day not ill
    ## 1060    > 4 glasses/day not ill
    ## 1061    > 4 glasses/day not ill
    ## 1062    > 4 glasses/day not ill
    ## 1063    > 4 glasses/day not ill
    ## 1064    > 4 glasses/day not ill
    ## 1065    > 4 glasses/day not ill
    ## 1066    > 4 glasses/day not ill
    ## 1067    > 4 glasses/day not ill
    ## 1068    > 4 glasses/day not ill
    ## 1069    > 4 glasses/day not ill
    ## 1070    > 4 glasses/day not ill
    ## 1071    > 4 glasses/day not ill
    ## 1072    > 4 glasses/day not ill
    ## 1073    > 4 glasses/day not ill
    ## 1074    > 4 glasses/day not ill
    ## 1075    > 4 glasses/day not ill
    ## 1076    > 4 glasses/day not ill
    ## 1077    > 4 glasses/day not ill
    ## 1078    > 4 glasses/day not ill
    ## 1079    > 4 glasses/day not ill
    ## 1080    > 4 glasses/day not ill
    ## 1081    > 4 glasses/day not ill
    ## 1082    > 4 glasses/day not ill
    ## 1083    > 4 glasses/day not ill
    ## 1084    > 4 glasses/day not ill
    ## 1085    > 4 glasses/day not ill
    ## 1086    > 4 glasses/day not ill
    ## 1087    > 4 glasses/day not ill
    ## 1088    > 4 glasses/day not ill
    ## 1089    > 4 glasses/day not ill
    ## 1090    > 4 glasses/day not ill
    ## 1091    > 4 glasses/day not ill
    ## 1092    > 4 glasses/day not ill
    ## 1093    > 4 glasses/day not ill
    ## 1094    > 4 glasses/day not ill

``` r
#cross tabulating
gast1 <- table(gast$Consumption, gast$Outcome)
gast2 <- xtabs(~Consumption + Outcome, data =gast)

#barplot
gast3 <- barplot(gast2, beside = TRUE)
```

![](README_files/figure-markdown_github/unnamed-chunk-2-1.png)

``` r
#chi squared test
gast4 <- chisq.test(gast2, correct = TRUE)
gast4
```

    ## 
    ##  Pearson's Chi-squared test
    ## 
    ## data:  gast2
    ## X-squared = 74.925, df = 2, p-value < 2.2e-16

-   Test Assumptions- There was random sampling, the observations are independent and the sample is large.

-   x-squared=0.23
-   df=2
-   p-value=2.2e-16
-   We reject the null hypothesis. There is a correlation between drinking contaminated water and falling ill.

------------------------------------------------------------------------

Nausea
------

-   Null Hypothesis-The chemotherapy does not cause nausea.
-   Alternative Hypothesis- Chemotherapy causes nausea.

``` r
naus <- read.csv('nausea (1).csv')
naus
```

    ##   Patient Nausea_before Nausea_after
    ## 1       1             3            2
    ## 2       2             4            0
    ## 3       3             6            1
    ## 4       4             2            3
    ## 5       5             2            1
    ## 6       6             4            1
    ## 7       7             5            0
    ## 8       8             6           40

``` r
#line graph
plot(naus$Nausea_before~ naus$Patient, type = 'l',  col = 'blue', ylim = c(0,6))
lines(naus$Nausea_after~ naus$Patient, col = 'red')
legend("top", c('Nausea Before', 'Nausea after'), fill = c('blue', 'red'))
```

![](README_files/figure-markdown_github/unnamed-chunk-3-1.png)

``` r
#wilcox
wilcox.test(naus$Nausea_before, naus$Nausea_after, data = naus)
```

    ## Warning in wilcox.test.default(naus$Nausea_before, naus$Nausea_after, data
    ## = naus): cannot compute exact p-value with ties

    ## 
    ##  Wilcoxon rank sum test with continuity correction
    ## 
    ## data:  naus$Nausea_before and naus$Nausea_after
    ## W = 52.5, p-value = 0.03407
    ## alternative hypothesis: true location shift is not equal to 0

\*Test Assumptions- We are comparing 2 groups and the data is ordinal.

-   W=52.5
-   p-value=0.034
-   We reject the null hypothesis. Chemotherapy does cause nausea.
