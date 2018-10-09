| Description |  A step by step guide to start on R |
| :------------- | :------------- | :------------- | :------------- |
| Authors | christine Tranchant-Dubreuil (christine.tranchant@ird.fr)  |
| Creation Date | 21/09/2018 |
| Last Modified Date | 22/09/2018 |



### Summary

<!-- TOC depthFrom:2 depthTo:2 withLinks:1 updateOnSave:1 orderedList:0 -->
- [Starting slowly on R](#start)
  - [Installing new packages `install.packages(packages)`](#install)
  - [Loading library`library`](#library)
  - [Setting a working directory](#setwd)
  - [Getting the current working directory `getwd`](#getwd)
  
- [Importing Data From `csv` File Into a `Dataframe`](#importCsv)
  - [Storing the content of a file *allGenomeVersion.csv* into a dataframe *myGenome* - `read.csv2()` (french format)](#readCsv)
  - [Displaying the whole dataframe](#printDF)
  - [Getting the type - `class(dataframe)`](#getType)
  - [Getting the structure of the dataframe (data type, number of levels) - `str(dataframe)`](#structureDF)
  - [Getting basic stats about te content of a dataframe - `summary(dataframe)`](#statDF)

- [Displaying basic informations about the dataframe structure](#info)
  - [Column names - `names(dataframe)` or  `colnames(dataframe)`](#colnames)
  - [Lines and columns number - `dim(dataframe)`](#dim)
  - [Lines number - `nrow(dataframe)`](#nrow)
  - [Columns number - `ncol(dataframe)`](#ncol)

- [Displaying the dataframe content](#print)
  - [Printing the first lines - `head(dataframe)`](#head)
  - [Printing the last lines - `last(dataframe)`](#last)
  - [Printing a column - `dataframe[colNum|colName]` or  `dataframe$colName`](#df0)
  - [Printing one whole line - `dataframe[lineNum,]`](#df)
  - [Printing one line, one column - `dataframe[lineNum,colNum]`](#df2)
  - [Printing some lines - `dataframe[LineStart:LineEnd,]`](#df3)
  - [Printing one column of some lines - `dataframe[c(line1,line2,line3),colNum]`](#df4)
  
- [Manipulating the content of a dataframe](#manipulating)
  - [Adding a new column](#add)
  - [Extracting unique values of a column - `unique(dataframe$colName)`](#unique)
  - [Extracting one part of a dataframe - `subset(dataframe)`](#extract)
  - [Calculating a sum - `sum(dataframe)` with filtering on an other column](#cal)
  - [ Getting the number of elements in a dataframe - `length(dataframe)` with filtering on an other column](#length)
  - [Ordering dataframe on one column](#order)
  - [Getting summaries of values of a column  - `summary`](#summary)
  
- [Plotting data from a dataframe with `ggplot` library](#plot)
  - [Creating a barplot with `geom_bar(stat = "identity")`](#barplot)
  - [Distinct plot - `position=position_dodge()` and flip plot with `coord_flip()`](#flip)<a name="dodge"></a>
  - [Save into a file`](#savePng)
  - [Creating a barplot with `geom_bar(stat = "count")`](#count)
  - [ Plotting a violin plot  - `geom_violin()`](#violinPlot)
  

- [License](#license) 

-----------------------

<a name="start"></a>
### Starting slowly on R

<a name="install"></a>
##### Installing New Packages/libraries - `install.packages(package) `

{% highlight bash %}
>install.packages('ggplot2')
{% endhighlight %}

<a name="library"></a>
##### Loading libraries  - `library(package)`
