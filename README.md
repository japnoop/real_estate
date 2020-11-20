---
title: "RealEstate"
author: "Andy"
date: "16/11/2020"
output: html_document
---

```{r}
library(tidyverse)
library(faraway)
```


```{r}
real_estate_df=read_csv("Real estate.csv")
```

```{r}
head(real_estate_df)
```

#Questions we may want to answer
```{r}
#What factors determine a house's price of unit area

#

```






#possible new data points
```{r}
#House price per unit / # convienent stores = the effect of nearby convienant stores to residence property value

#lets say we go with this...


convenience_store_difference = real_estate_df$`Y house price of unit area`/real_estate_df$`X4 number of convenience stores`
#we are assuming that every convenience store suits a households need equally.

real_estate_df=cbind(real_estate_df,convenience_store_difference)

head(real_estate_df)

```


#Is a Linear Regression even appropriate?
```{r}
pairs(real_estate_df)
```

#Model Selection 
```{r}

```

