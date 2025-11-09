Airbnb – Homework  
 

1\. **Dataset Overview**

| Item | Description |
| :---- | :---- |
| Dataset name | Airbnb Dataset |
| Number of rows |  51707 |
| Number of columns |  22 |
| Format file (.csv, .txt, etc) |  Excel |
| Authors of the dataset |  Kristóf Gyódi, Łukasz Nawaro |
| Source (name) |  Google Spreadsheet |
| Source (link) | https://docs.google.com/spreadsheets/d/1ecopK6oyyb4d\_7-QLrCr8YlgFrCetHU7-VQfnYej7JY/edit?gid=1950822222\#gid=1950822222 |

 

 

2\. **Dataset Structure**

| Feature/variable | Data type | Description | Number of Unique values | Example values |
| :---- | :---- | :---- | :---- | :---- |
|  price |  float64 |   |  10497 |  194.033698, 344.245776, 264.101422, 433.529398 |
|  room\_type |  object |   |  3 |  Private room, Entire home/apt, Shared room |
|  room\_shared |  bool |   |  2 |  True, False |
| room\_private | bool |   | 2 | True, False |
| person\_capacity | int64 |   | 5 | 2,3,4,5,6 |
| host\_is\_superhost | bool |   | 2 | True, False |
| multi | int64 |   | 2 | True, False |
| biz | int64 |   | 2 | True, False |
| cleanliness\_rating | int64 |   | 9 | 2, 3, 4, 5, 6, 7, 8, 9, 10 |
| guest\_satisfaction\_overall | int64 |   | 53 | 85, 86, 88, 89, 99, 100 |
| bedrooms | int64 |   | 10 | 1, 2, 3, 5, 4, |
| Dist | float64 |   | 51707 | 5.0229638, 0.48838929, 5.74831192, |
| metro\_dist | float64 |   | 51707 | 2.53938, 0.23940392, 3.65162129 |
| attr\_index | float64 |   | 51707 | 78.69037927, 631.17637825, 75.27587691, |
| attr\_index\_norm | float64 |   | 51688 | 4.16670787, 33.42120862, 3.9859077 |
| rest\_index | float64 |   | 51707 | 98.25389587, 837.28075674, 95.38695493, |
| rest\_index\_norm | float64 |   | 51688 | 6.84647282, 58.34292774, 6.64670025 |
| lng | float64 |   | 23600 | 4.90569, 4.90005, 4.97512, |
| lat | float64 |   | 21484 | 52.41772, 52.37432, 52.36103, |
| city | object |   | 10 | Amsterdam, athens, berlin, barcelona |
| day | object |   | 2 | 'weekdays', 'weekends' |
| country | object |   | 9 | 'Netherlands', 'Greece', 'Germany', 'Spain', |

 

3\. **Data cleaning**

| Issue | Names of Columns affected | Description of the Issue | Action Taken |
| :---- | :---- | :---- | :---- |
| Inconsistent column labeling |   |   |   |
| Wrong data types |   |   |   |
| Missing values |   |   |   |
| Duplicates |   |   |   |
| Inconsistent categories |   |   |   |
| Other |   |   |   |

 

 

 

 

 

 

4\. **Descriptive statistics**

Numeric columns

 

|  | count | mean | std | min | 25% | 50% | 75% | max |
| :---- | ----- | ----- | ----- | ----: | ----: | ----: | ----- | ----- |
| price | 51707 | 279.8796 | 327.948 | 34.779 | 148.7522 | 211.3431 | 319.694 | 18545.45 |
| person\_capacity | 51707 | 3.161661 | 1.29855 | 2 | 2 | 3 | 4 | 6 |
| multi | 51707 | 0.291353 | 0.45439 | 0 | 0 | 0 | 1 | 1 |
| biz | 51707 | 0.350204 | 0.47704 | 0 | 0 | 0 | 1 | 1 |
| cleanliness\_rating | 51707 | 9.390624 | 0.95487 | 2 | 9 | 10 | 10 | 10 |
| guest\_satisfaction\_overall | 51707 | 92.62823 | 8.94553 | 20 | 90 | 95 | 99 | 100 |
| bedrooms | 51707 | 1.15876 | 0.62741 | 0 | 1 | 1 | 1 | 10 |
| dist | 51707 | 3.191285 | 2.3938 | 0.015 | 1.453142 | 2.613538 | 4.26308 | 25.284557 |
| metro\_dist | 51707 | 0.68154 | 0.85802 | 0.0023 | 0.24848 | 0.413269 | 0.73784 | 14.273577 |
| attr\_index | 51707 | 294.2041 | 224.754 | 15.152 | 136.7974 | 234.3317 | 385.756 | 4513.5635 |
| attr\_index\_norm | 51707 | 13.42379 | 9.80799 | 0.9263 | 6.380926 | 11.46831 | 17.4151 | 100 |
| rest\_index | 51707 | 626.8567 | 497.92 | 19.577 | 250.8541 | 522.0528 | 832.629 | 6696.1568 |
| rest\_index\_norm | 51707 | 22.78618 | 17.8041 | 0.5928 | 8.75148 | 17.54224 | 32.9646 | 100 |
| lng | 51707 | 7.426068 | 9.79973 | \-9.226 | \-0.0725 | 4.873 | 13.5188 | 23.78602 |
| lat | 51707 | 45.67113 | 5.24926 | 37.953 | 41.39951 | 47.50669 | 51.4719 | 52.64141 |

 

 

 

 

 

 

 

Category columns

 

|  | room\_type | city | day | country |
| :---- | ----- | ----- | ----- | ----- |
| count | 51707 | 51707 | 51707 | 47685 |
| unique | 3 | 10 | 2 | 9 |
| top | Entire home/apt | london | weekends | United Kingdom |
| freq | 32648 | 9993 | 26207 | 9993 |
| Most frequent value (frequency) | Entire home/apt | London | weekends | United Kingdom |
| Least frequent value | Shared room | amsterdam | weekdays | Netherlands |

 

 

 

