# Excel Formulas and Functions for Data Analysts

## Overview

Excel formulas and functions are essential for performing calculations, analyzing data, and automating repetitive tasks. Whether you're working with financial reports, sales data, customer information, or operational metrics, understanding Excel formulas can significantly improve your productivity and analytical capabilities.

This guide covers the core Excel formulas that every Data Analyst should know. The functions are organized into categories with syntax, explanations, and practical examples to help you build a strong foundation.

---

# Table of Contents

- Mathematical Functions
- Statistical Functions
- Logical Functions
- Lookup Functions

---

# Mathematical Functions

Mathematical functions are used to perform basic calculations on numerical data.

| Function | Syntax | Description | Example |
|----------|--------|-------------|---------|
| SUM | `=SUM(A1:A10)` | Adds all numbers in a range | Total monthly sales |
| AVERAGE | `=AVERAGE(A1:A10)` | Returns the average value | Average customer spend |
| MIN | `=MIN(A1:A10)` | Returns the smallest value | Lowest sales value |
| MAX | `=MAX(A1:A10)` | Returns the largest value | Highest revenue |
| ROUND | `=ROUND(A1,2)` | Rounds a number to a specified number of decimal places | Round profit to 2 decimals |
| ABS | `=ABS(A1)` | Returns the absolute value | Remove negative signs |
| MOD | `=MOD(A1,2)` | Returns the remainder after division | Identify odd and even numbers |
| POWER | `=POWER(A1,2)` | Raises a number to a specified power | Square a value |

### Example

| Product | Sales |
|---------|------:|
| Laptop | 1200 |
| Monitor | 650 |
| Keyboard | 150 |

**Formula**

```excel
=SUM(B2:B4)
```

**Result**

```
2000
```

---

# Statistical Functions

Statistical functions help summarize and analyze datasets.

| Function | Syntax | Description | Example |
|----------|--------|-------------|---------|
| COUNT | `=COUNT(A:A)` | Counts cells containing numbers | Count sales transactions |
| COUNTA | `=COUNTA(A:A)` | Counts non-empty cells | Count customer records |
| COUNTBLANK | `=COUNTBLANK(A:A)` | Counts blank cells | Identify missing values |
| COUNTIF | `=COUNTIF(A:A,">100")` | Counts cells matching a condition | Sales greater than 100 |
| COUNTIFS | `=COUNTIFS(A:A,">100",B:B,"East")` | Counts using multiple conditions | Regional sales count |

### Example

```excel
=COUNTIF(B2:B20,">500")
```

This formula counts how many sales values are greater than **500**.

---

# Logical Functions

Logical functions evaluate conditions and return different results based on whether the conditions are true or false.

| Function | Syntax | Description | Example |
|----------|--------|-------------|---------|
| IF | `=IF(A1>100,"Yes","No")` | Returns one value if a condition is true and another if false | Pass or Fail |
| IFS | `=IFS(A1>90,"A",A1>80,"B")` | Evaluates multiple conditions | Student grades |
| AND | `=AND(A1>0,B1<100)` | Returns TRUE if all conditions are met | Multiple validations |
| OR | `=OR(A1>0,B1>0)` | Returns TRUE if any condition is met | At least one condition |
| NOT | `=NOT(A1>100)` | Reverses a logical result | Negate a condition |

### Example

```excel
=IF(B2>=1000,"High","Low")
```

If the sales amount is **1000 or greater**, the result will be **High**; otherwise, it will return **Low**.

---

# Lookup Functions

Lookup functions are among the most important Excel functions for Data Analysts. They are used to retrieve data from another table based on a matching value.

| Function | Syntax | Description | Example |
|----------|--------|-------------|---------|
| XLOOKUP | `=XLOOKUP(A2,D:D,E:E)` | Looks up a value in a range and returns a corresponding result | Find product price |
| VLOOKUP | `=VLOOKUP(A2,D:E,2,FALSE)` | Searches vertically for a value | Retrieve employee department |
| HLOOKUP | `=HLOOKUP(A2,D1:H2,2,FALSE)` | Searches horizontally for a value | Lookup monthly targets |
| INDEX | `=INDEX(B:B,5)` | Returns a value from a specified position | Retrieve data by row number |
| MATCH | `=MATCH(A2,D:D,0)` | Returns the position of a value | Locate record position |
| INDEX + MATCH | `=INDEX(B:B,MATCH(A2,A:A,0))` | Flexible alternative to VLOOKUP | Advanced lookups |

### Example

```excel
=XLOOKUP(A2,D:D,E:E)
```

This formula searches for the value in **A2** within column **D** and returns the matching value from column **E**.

---

## Summary

The formulas covered in this guide form the foundation of Excel-based data analysis. Mastering these functions will help you perform calculations, summarize information, apply business logic, and retrieve data efficiently.

In the next section, you'll learn additional Excel functions for working with text, dates, dynamic arrays, and financial calculations.