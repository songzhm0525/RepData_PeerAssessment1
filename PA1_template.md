# Reproducible Research: Peer Assessment 1


## Loading and preprocessing the data

```r
data = read.table("activity.csv", sep = ",", header = T)
head(data)
```

```
##   steps       date interval
## 1    NA 2012-10-01        0
## 2    NA 2012-10-01        5
## 3    NA 2012-10-01       10
## 4    NA 2012-10-01       15
## 5    NA 2012-10-01       20
## 6    NA 2012-10-01       25
```


## What is mean total number of steps taken per day?

```r
# Make histogram of steps data that is not NA
steps = data$steps[!is.na(data$steps)]
hist(steps, xlab = "steps")
```

![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2.png) 


```r
# calculate mean
mean(steps)
```

```
## [1] 37.38
```

```r
# calculate median
median(steps)
```

```
## [1] 0
```



## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
