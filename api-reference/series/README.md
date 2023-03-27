---
description: One-dimensional ndarray with axis labels (including time series).
---

# Series

> `Series`(data, {**columns:** \[ Array ], **dtypes:** \[ Array ], **index:** \[Array]}) \[[source](https://github.com/javascriptdata/danfojs/blob/master/src/danfojs-base/core/series.ts#L50)]

### Attributes

| [`Series.index`](series.index.md) | The index (axis labels) of the Series. |
| --------------------------------- | -------------------------------------- |

| [`Series.tensor`](series.tensor.md) | The Tensorflow tensor of the data backing this Series or Index.  |
| ----------------------------------- | ---------------------------------------------------------------- |
| [`Series.values`](series.values.md) | Return Series as ndarray or ndarray-like depending on the dtype. |
| [`Series.dtype`](series.dtype.md)   | Return the dtype object of the underlying data.                  |
| [`Series.shape`](series.shape.md)   | Return a tuple of the shape of the underlying data.              |
| [`Series.ndim`](series.ndim.md)     | Number of dimensions of the underlying data, by definition 1.    |
| [`Series.size`](broken-reference/)  | Return the number of elements in the underlying data.            |

### Conversion

| [`Series.asType`](../dataframe/dataframe.astype.md) | Cast a Series object to a specified dtype      |
| --------------------------------------------------- | ---------------------------------------------- |
| [`Series.copy`](series.copy.md)                     | Make a copy of this object’s indices and data. |

### Indexing, iteration

|                                     |                                                                    |
| ----------------------------------- | ------------------------------------------------------------------ |
| `` [`Series.loc`](series.loc.md) `` | Access a group of rows and columns by label(s) or a boolean array. |
| [`Series.iloc`](series.iloc.md)     | Purely integer-location based indexing for selection by position.  |

### Binary operator functions

| [`Series.add`](series.add.md)     | Return Addition of series and other, element-wise (binary operator add).                |
| --------------------------------- | --------------------------------------------------------------------------------------- |
| [`Series.sub`](series.sub.md)     | Return Subtraction of series and other, element-wise (binary operator sub).             |
| [`Series.mul`](series.mul.md)     | Return Multiplication of series and other, element-wise (binary operator mul).          |
| [`Series.div`](series.div.md)     | Return Floating division of series and other, element-wise (binary operator truediv).   |
| [`Series.mod`](series.mod.md)     | Return Modulo of series and other, element-wise (binary operator mod).                  |
| [`Series.pow`](series.pow.md)     | Return Exponential power of series and other, element-wise (binary operator pow).       |
| [`Series.round`](series.round.md) | Round each value in a Series to the given number of decimals.                           |
| [`Series.lt`](series.lt.md)       | Return Less than of series and other, element-wise (binary operator lt).                |
| [`Series.gt`](series.gt.md)       | Return Greater than of series and other, element-wise (binary operator gt).             |
| [`Series.le`](series.le.md)       | Return Less than or equal to of series and other, element-wise (binary operator le).    |
| [`Series.ge`](series.ge.md)       | Return Greater than or equal to of series and other, element-wise (binary operator ge). |
| [`Series.ne`](series.ne.md)       | Return Not equal to of series and other, element-wise (binary operator ne).             |
| [`Series.eq`](series.eq.md)       | Return Equal to of series and other, element-wise (binary operator eq).                 |

### Function application&#x20;

| [`Series.apply`](series.apply.md) | Invoke function on values of Series.                    |
| --------------------------------- | ------------------------------------------------------- |
| [`Series.map`](series.map.md)     | Map values of Series according to input correspondence. |

### Computations / descriptive stats

| [`Series.abs`](series.abs.md)                               | Return a Series with absolute numeric value of each element.     |
| ----------------------------------------------------------- | ---------------------------------------------------------------- |
| [`Series.corr`](broken-reference/)                          | Compute correlation with other Series, excluding missing values. |
| [`Series.count`](series.count.md)                           | Return number of non-NaN observations in the Series.             |
| [`Series.cumMax`](../dataframe/danfo.dataframe.cummax.md)   | Return cumulative maximum over a DataFrame or Series axis.       |
| [`Series.cumMin`](../dataframe/danfo.dataframe.cummin.md)   | Return cumulative minimum over a DataFrame or Series axis.       |
| [`Series.cumProd`](../dataframe/danfo.dataframe.cumprod.md) | Return cumulative product over a DataFrame or Series axis.       |
| [`Series.cumSum`](../dataframe/danfo.dataframe.cumsum.md)   | Return cumulative sum over a DataFrame or Series axis.           |
| [`Series.describe`](series.describe.md)                     | Generate descriptive statistics.                                 |
| [`Series.max`](series.max.md)                               | Return the maximum of the values for the requested axis.         |
| [`Series.mean`](series.mean.md)                             | Return the mean of the values for the requested axis.            |
| [`Series.median`](series.median.md)                         | Return the median of the values for the requested axis.          |
| [`Series.min`](series.min.md)                               | Return the minimum of the values for the requested axis.         |
| [`Series.mode`](series.mode.md)                             | Return the mode(s) of the dataset.                               |
| [`Series.std`](series.std.md)                               | Return sample standard deviation over requested axis.            |
| [`Series.sum`](series.sum.md)                               | Return the sum of the values for the requested axis.             |
| [`Series.var`](series.var.md)                               | Return unbiased variance over requested axis.                    |
| [`Series.unique`](series.unique.md)                         | Return unique values of Series object.                           |
| [`Series.nUnique`](series.nunique.md)                       | Return number of unique elements in the object.                  |
| [`Series.valueCounts`](series.value_counts.md)              | Return a Series containing counts of unique values.              |

### Reindexing / selection / label manipulation

|                                                      |                                                          |
| ---------------------------------------------------- | -------------------------------------------------------- |
| [`Series.dropDuplicates`](series.drop_duplicates.md) | Return Series with duplicate values removed.             |
| [`Series.head`](series.head.md)                      | Return the first n rows.                                 |
| [`Series.resetIndex`](series.reset_index.md)         | Generate a new DataFrame or Series with the index reset. |
| [`Series.sample`](series.sample.md)                  | Return a random sample of items from an axis of object.  |
| [`Series.tail`](series.tail.md)                      | Return the last n rows.                                  |

### Missing data handling

|                                       |                                                  |
| ------------------------------------- | ------------------------------------------------ |
| [`Series.droNa`](series.dropna.md)    | Return a new Series with missing values removed. |
| [`Series.fillNa`](series.fillna.md)   | Fill NaN values using the specified method.      |
| [`Series.isNa`](series.isna.md)       | Detect missing values.                           |
| [`Series.replace`](series.replace.md) | Replace values given in to_replace with value.   |

### Logical Comparison

|                               |                                                                                                      |
| ----------------------------- | ---------------------------------------------------------------------------------------------------- |
| [`Series.or`](series.or.md)   | Returns the logical OR between Series and other. Supports element-wise operations and broadcasting.  |
| [`Series.and`](series.and.md) | Returns the logical AND between Series and other. Supports element-wise operations and broadcasting. |

### Reshaping, sorting

| [`Series.argSort`](series.argsort.md)        | Return the integer indices that would sort the Series values. |
| -------------------------------------------- | ------------------------------------------------------------- |
| [`Series.argMin`](series.argmin.md)          | Return int position of the smallest value in the Series.      |
| [`Series.argMax`](series.argmax.md)          | Return int position of the largest value in the Series.       |
| [`Series.sortValues`](series.sort_values.md) | Sort by the values.                                           |

### Accessors

Danfo provides dtype-specific methods under various accessors. These are separate namespaces within [`Series`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.html#pandas.Series) that only apply to specific data types.

| Data Type                                    | Accessor |
| -------------------------------------------- | -------- |
| [Datetime](../general-functions/danfo.dt.md) | dt       |
| [String](../general-functions/danfo.str.md)  | str      |

#### Datetimelike properties

`Series.dt` can be used to access the values of the series as datetime and return several properties. These can be accessed like `Series.dt.<property>`.

**Datetime methods**

|                                                    |                                                                         |
| -------------------------------------------------- | ----------------------------------------------------------------------- |
| [`Series.dt.year`](series.dt.year.md)              | The year of the datetime.                                               |
| [`Series.dt.month`](series.dt.month.md)            | Returns a numeric representation of the month. January=0 - December=11. |
| [Series.dt.monthName](series.dt.month_name.md)     |                                                                         |
| [`Series.dt.dayOfWeek`](series.dt.day.md)          | Returns the day of the week, in local time                              |
| [`Series.dt.hour`](series.dt.hour.md)              | The hours of the datetime.                                              |
| [`Series.dt.minute`](series.dt.minute.md)          | The minutes of the datetime.                                            |
| [`Series.dt.second`](series.dt.second.md)          | The seconds of the datetime.                                            |
| [`Series.dt.dayOfWeekName`](series.dt.weekdays.md) | Returns the name of the day, of the week, in local time                 |
| [`Series.dt.dayOfMonth`](series.dt.month_name.md)  | Returns the day of the month, in local time                             |

#### String handling

`Series.str` can be used to access the values of the series as strings and apply several methods to it. These can be accessed like `Series.str.<function/property>`.

| [`Series.str.capitalize`](series.str.capitalize.md)   | Capitalize the first character of each string                                                                                  |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| [`Series.str.toUpperCase`](series.str.touppercase.md) | Converts all characters to uppercase.                                                                                          |
| [`Series.str.toLowerCase`](series.str.tolowercase.md) | Converts all characters to lowercase.                                                                                          |
| [`Series.str.charAt`](series.str.charat.md)           | Returns the character at the specified index (position).                                                                       |
| [`Series.str.concat`](series.str.concat.md)           | Joins two or more strings/arrays.                                                                                              |
| [`Series.str.startsWith`](series.str.startswith.md)   | Checks whether a string begins with specified characters.                                                                      |
| [`Series.str.endsWith`](series.str.endswith.md)       | Checks whether a string ends with specified characters                                                                         |
| [`Series.str.includes`](series.str.includes.md)       | Checks whether a string contains the specified string/characters.                                                              |
| [`Series.str.indexOf`](series.str.indexof.md)         | Returns the position of the first found occurrence of a specified value in a string.                                           |
| [`Series.str.lastIndexOf`](series.str.lastindexof.md) | Returns the position of the last found occurrence of a specified value in a string.                                            |
| [`Series.str.repeat`](series.str.repeat.md)           | Returns a new string with a specified number of copies of an existing string.                                                  |
| [`Series.str.search`](series.str.search.md)           | Searches a string for a specified value, or regular expression, and returns the position of the match.                         |
| [`Series.str.slice`](series.str.slice.md)             | Extracts a part of a string and returns a new string.                                                                          |
| [`Series.str.split`](series.str.split.md)             | Splits a string into an array of substrings.                                                                                   |
| [`Series.str.substr`](series.str.substr.md)           | Extracts the characters from a string, beginning at a specified start position, and through the specified number of character. |
| [`Series.str.substring`](series.str.substring.md)     | Extracts the characters from a string, between two specified indices.                                                          |
| [`Series.str.len`](series.str.len.md)                 | Counts the number of characters in each string.                                                                                |
| [`Series.str.trim`](series.str.trim.md)               | Removes whitespace from both ends of a string.                                                                                 |
| [`Series.str.join`](series.str.join.md)               | Joins strings to specified value.                                                                                              |
| [`Series.str.replace`](series.str.replace.md)         | Replace each occurrence of pattern/regex in the Series/Index.                                                                  |

### Plotting

`Series.plot` is both a callable method and a namespace attribute for specific plotting methods of the form `Series.plot.<kind>`.

|                                                       |                                                               |
| ----------------------------------------------------- | ------------------------------------------------------------- |
| [`Series.plot.bar`](../plotting/bar-charts.md)        | Vertical bar plot.                                            |
| [`Series.plot.box`](../plotting/box-plots.md)         | Make a box plot of the DataFrame columns.                     |
| [`Series.plot.violin`](../plotting/box-plots.md)      | Make a violin plot of the DataFrame columns.                  |
| [`Series.plot.hist`](../plotting/histograms.md)       | Draw one histogram of the DataFrame’s columns.                |
| [`Series.plot.scatter`](../plotting/scatter-plots.md) | Generate Kernel Density Estimate plot using Gaussian kernels. |
| [`Series.plot.line`](../plotting/line-charts.md)      | Plot Series or DataFrame as lines.                            |
| [`Series.plot.pie`](../plotting/pie-charts.md)        | Generate a pie plot.                                          |
| [`Timeseries Plots`](../plotting/timeseries-plots.md) | Time series plots                                             |
| [`Table`](../plotting/tables.md)                      | Display Series as Interactive table in a Div                  |

### Serialization / IO / conversion

|                                                      |                                              |
| ---------------------------------------------------- | -------------------------------------------- |
| [`Series.toCSV`](../dataframe/dataframe.to_csv.md)   | Convert DataFrame or Series to CSV.          |
| [`Series.toJSON`](../dataframe/dataframe.to_json.md) | Convert DataFrame or Series to a JSON.       |
| Series.toExcel                                       | Convert DataFrame or Series to an excel file |
