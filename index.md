---
title       : Chance of Esophageal Cancer
subtitle    : How likely are you to have Esophageal Cancer?
author      : Kenneth Kihara
job         : Programmer
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Usage
This shiny app calculates the chance that a person will have esophageal 
cancer given age, alcohol consumption, and tobacco consumption. Choose 
the inputs by moving the appropriate slider. The output is printed under 
"Predicted Chance of Esophageal Cancer:"

## Data
The data used for predicting esophageal cancer was taken from the esoph 
dataset in the R datasets package. The predictors used are:

- Age Group
- Daily Alcohol Consumption
- Daily Tobacco Consumption

---

## Why use this application?

1. Promote awareness of esophageal cancer
2. Diagnose and seek treatment sooner
3. Supporting evidence that alchol and tobacco causes cancer
4. Determine a quick prediction of your chance of cancer
5. Show the dangers of alcohol and tobacco consumption

---

## Accuracy
The model was trained with a 10-fold cross validation. Giving an accuracy 
and standard deviation of:



```r
fit$results$Accuracy
```

```
## [1] 0.8164296
```

```r
fit$results$AccuracySD
```

```
## [1] 0.03069731
```

---

## Plots

Plots of frequency of age vs alcohol consumption and age vs tobacco 
consumption.
![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3-1.png) 
