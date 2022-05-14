### Week 3
**Subsetting and Sorting**
- subsetting using the operator ``[]`` (inside can be column name or index number)
- subsetting with logical statement
- dealing with missing values
    - does not return NA if ``X[which(condition), ...]``
- sorting using ``sort(column, decreasing = TRUE, na.last = TRUE)``
- ordering using ``X[order(column), ]``
- adding new rows and columns
- using ``rbind`` and ``cbind``


**Ordering with plyr**
```
library(plyr)
arange(x, desc(var1))
```

**Summarizing Data**
1. ``head(df, n = m)``
2. ``tail(df, n = m)``
3. ``summary(df)``
4. ``str(df)``: with datatype being printed
5. ``quantile(df, probs = c(0.25, 0.5, 0.75), na.rm=TRUE)``
6. ``table(df, useNA = "ifany")``

**Checking for missing values**
1. ``sum(is.na(column))``
2. ``any(is.na(collumn))``
3. ``all(is.na(condition))``
4. ``colSums(is.na(column))``
5. ``all(colSums(is.na(column))=0)``

**Finding certain values**
1. ``table(column %in% c("1", "2"))``: return logical tatement

**Cross Tabs + Flat Table**
1. ``xt <- xtabs(Freq ~ Gender + Admit, data=DF)``
2. ``ftable(xy)``

**Size of Dataset**
- ``object.size(df)``

**Creating New Variables**
1. ``seq(start, to, by, length)``

**Creating Binary Variable**
- ``ifelse(column < 0, TRUE, FALSE)``
- ``sample(c("yes", "no"), size = n, replace = TRUE)``

**Reshaping Data**
1. ``melt``
2. ``dcast``
3. ``tapply``
4. ``split``
5. ``lapply``
6. ``unlist``
7. ``sapply``
8. ``ddply``

### dplyr packages
- managing data frame in R

<img src = "dplyrimg.png" alt = "Dplyr Packages Functions">

- the results is always a dataframe
- ``names(df)``
- ``match()``
- ``filter()``
- ``arrange(desc = )``
- ``rename()``
- ``mutate()``
- ``groupby()``
- ``merge(x, y, by.x, by.y, all=TRUE)``
    - default merge column with the same / common name
- ``join()``
- ``list()``
- ``joinall()``














