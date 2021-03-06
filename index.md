---
title       : Developing Data Products Project
subtitle    : Slidify Presentation
author      : Kevin Clifford
job         : myproj
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Table Of Contents

1. Compound Interest - Overview
2. Shiny Application Usage 
3. R Code Example

--- .class #id 

## Compound Interest - Overview


The Compound Interest Equation


P = C (1 + r/n)$^n$ $^t$


where:

    P = future value
    
    C = initial deposit
    
    r = interest rate (expressed as a fraction: eg. 0.06)
    
    n = number of times per year interest is compounded
    
    t = number of years invested


--- .class #id 

## Shiny Application Usage


1. Enter 'Initail Deposit': The amount that is deposited. This is C in the formula

2. Enter 'Number Of Years Invested': The total number of years the deposit will remain invested. This is 't' in the formula

3. Enter 'Interest Rate': The percentage at which interest is calculated. This is r/100 in the formula

Note: The number of times per year interest is compounded is fixed at 1 i.e. yearly


--- .class #id 

## R Code Example


```r
deposit<-100   #Initial Deposit
nyears<-2      #Number Of Years Invested
irate<-10      #Interest Rate (Percentage)

#FUTURE VALUE
deposit*(1+(irate/100))^nyears
```

```
## [1] 121
```
---
