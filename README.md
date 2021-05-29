# Quality4Dataset
This is a project evaluating quality for dataset.
### Author: Hao-Ying Cheng, Nickname: MaskerTim

## Data Format of Quality
This will output the two dataset, quality_issues.json and quality_score.json.
This section tells you about the data format for both.
### Quality Issues
Quality isssues tell that what quality issues are concerned.
There are five issues classified by three classes.
#### Three classes:
* Column Issue
    * issue: the name of issue
    * metric: prevalence
    * count: tell what amounts of data for this issue in column.
* Row Issue
    * issue: the name of issue
    * metric: confidence
    * count: tell what amounts of data for this issue in row.
* Cell Issue
    * issue: the name of issue
    * metric: confidence
    * count: tell what amounts of cells for this issue in dataset.
> Issues means that it is expected or not in dataset. 
> Column, Row, Cell mean the type that occurs in dataset.
> prevalence means what portion of datas that occur the issue in dataset.
> conference means what belief to the extent about the issue in dataset .
#### Five Issues:
1. Uniqueness Violation:
    * type: colume issue
    * description: not expected duplicated value in column.
2. distinct format
    * type: colume issue
    * description: not expected distinct data format in column.
3. missing value
    * type: cell issue
    * description: not expected missing value in cell.
4. outlier
    * type: cell issue
    * description: not expected outlier value in cell.
5. duplicated row
    * type: row issue
    * description: not expected duplicated data in row.
### Quality Scores
Quality scores tell that what quality scores per column.
We have four keys for this dataset.
#### Keys:
* id: identity for column
* colName: what column name is
* issues: what issues the column owns
* score: what score the column gains (unit:%)

## Reference
* [How to quantify Data Quality?](https://towardsdatascience.com/how-to-quantify-data-quality-743721bdba03)



