# Lab-7_202001028
## Previous Date Problem

**Test Cases**
| Test Case ID | Day | Month | Year | Expected Output |
| -------------|-----|-------|------|-----------------|
| 1 | 1 | 6 | 2000 | 31-5-2000 |
| 2 | 2 | 6 | 2015 | 1-6-2015 |
| 3 | 2 | 6 | 2016 | Invalid |
| 4 | 1 | 1 | 1900 | 31-12-1899 |
| 5 | 31 | 12 | 1899 | Invalid |
| 6 | 31 | 12 | 1900 | 30-12-1900 |
| 7 | 29 | 2 | 2012 | 28-2-2012 |
| 8 | 1 | 3 | 2012 | 29-2-2012 | 
| 9 | 29 | 2 | 2011 | Invalid |
| 10 | 30 | 2 | 2020 | Invalid |


**Equivalence Class Partitions** <br/>
Day:
| Partition ID | Range | Status |
|----------------------|-------|--------|
| E1 | Between 1 and 28 | Valid |
| E2 | Less than 1 | Invalid |
| E3 | Greater than 31 | Invalid |
| E4 | Equals 30 | Valid |
| E5 | Equals 29 | Valid for leap year |
| E6 | Equals 31 | Valid |

Month:
| Partition ID | Range | Status |
|----------------------|-------|--------|
| E7 | Between 1 and 12 | Valid |
| E8 | Less than 1 | Invalid |
| E9 | Greater than 12 | Invalid |

Year: 
| Partition ID | Range | Status |
|----------------------|-------|--------|
| E10 | Between 1900 and 2015 | Valid |
| E11 | Less than 1 | Invalid |
| E12 | Greater than 2015 | Invalid |

### Eclipse Code
