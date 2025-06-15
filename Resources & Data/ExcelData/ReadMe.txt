README: Excel Functions - IF, Nested IF, and IFS

1. IF Function:
The IF function is used to make logical comparisons between a value and what you expect.
Syntax:
    =IF(logical_test, value_if_true, value_if_false)

Example:
    =IF(A1>10, "Greater", "Smaller or Equal")
This formula checks if the value in cell A1 is greater than 10. If true, it returns "Greater"; otherwise, it returns "Smaller or Equal".

2. Nested IF Function:
Nested IF functions are used when you need to test multiple conditions.
Syntax:
    =IF(condition1, value_if_true1, IF(condition2, value_if_true2, value_if_false2))

Example:
    =IF(A1>90, "A", IF(A1>80, "B", IF(A1>70, "C", "F")))
This formula assigns grades based on the value in A1.

3. IFS Function:
The IFS function checks whether one or more conditions are met and returns a value corresponding to the first TRUE condition.
Syntax:
    =IFS(condition1, value1, condition2, value2, ...)

Example:
    =IFS(A1>90, "A", A1>80, "B", A1>70, "C", A1<=70, "F")
This formula is a cleaner alternative to nested IFs for assigning grades.

Note:
- The IF function is available in all versions of Excel.
- The IFS function is available in Excel 2016 and later.

