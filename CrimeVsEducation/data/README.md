* How to process fixed-length-input.

    1. Replace "," in numerical values, if any.
    2. Replace " {2,}" (ie. two or more spaces) with ","

* How to join two csv by states or state abbrev.s fast.

    1. Keep another csv of state name and abbrev pairs.
    2. Sort one files by abbrev, add the full names as a new column, sort by full name
    3. Sort the other files by full name
    4. Merge the two files.

* How to swap row/colum.

  * In Excel, copy, and then "paste with tranpose"
  * In R, `t()`
  * In Python, `pandas.dataframe.transpose()`

* How to process data in excel

    * Use `ROW()`, `$A$1` for absolute reference, use `OFFSET` for relative
    * Use another row to write formula
    * Copy the formula row, and "special paste" the result with "formula" turned off.
    * Use `INDEX()` to get cell of calculated row/column indices. eg. `=INDEX(A:A,FLOOR((ROW()-1)/10)+1,1)`
