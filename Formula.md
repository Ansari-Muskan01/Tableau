# Tableau Basic Functions

## 1. Logical Functions

**IF, ELSEIF, ELSE :** Used to check conditions and return results.<br>
**Syntax :** <br>
IF condition THEN result<br>
ELSEIF condition THEN result<br>
ELSE result<br>
END<br>

**CASE :** Used to compare a field with different values.<br>
**Syntax:**
CASE [Field Name]<br>
WHEN "Value 1" THEN "Result 1"<br>
WHEN "Value 2" THEN "Result 2"<br>
ELSE "Default Result"<br>
END<br>

**IIF() :** Used to check a condition and return one result if the condition is TRUE and another result if it is FALSE.<br>
**Syntax:** IIF(condition, result_if_true, result_if_false)<br>

**IFNULL() :** Returns an alternative value if the original value is Null.<br>
**Syntax:** IFNULL([Profit], 0)  -- (Note : If Profit is Null, it returns 0. Otherwise, it returns the original Profit value.)<br>

**ISNULL() :** Checks whether a value is Null.<br>
**Syntax:** ISNULL([Profit])   -- (Note :  Returns TRUE if Profit is Null and FALSE if Profit is not Null.)<br>

**ZN() :** Replaces Null numeric values with zero.<br>
**Syntax:** ZN([Profit])<br>

## 2. Number Functions

**ABS() :** Returns the absolute value of a number.<br>
**ROUND() :** Rounds a number to the specified decimal places.<br>
**CEILING() :** Rounds a number up to the next integer.<br>
**FLOOR() :** Rounds a number down to the previous integer.<br>

| Function | Example Value | Formula | Output |
|---|---:|---|---:|
| `ABS()` | -150.75 | `ABS(-150.75)` | 150.75 |
| `ROUND()` | 1200.567 | `ROUND(1200.567, 2)` | 1200.57 |
| `CEILING()` | 12.3 | `CEILING(12.3)` | 13 |
| `FLOOR()` | 12.8 | `FLOOR(12.8)` | 12 |

## 3. String Functions

**UPPER() :** Converts text to uppercase.<br>
**LOWER() :** Converts text to lowercase.<br>
**PROPER() :** Converts the first letter of each word to uppercase.<br>
**TRIM() :** Removes extra spaces from the beginning and end of text.<br>
**LEN() :** Returns the number of characters in a string.<br>
**LEFT() :** Returns characters from the left side.<br>
**RIGHT() :** Returns characters from the right side.<br>
**CONTAINS() :** Checks whether text contains a particular word or character.<br>
**REPLACE() :** Replaces matching text with new text.<br>

## 3. String Functions

| Function | Example Value | Formula | Output |
|---|---|---|---|
| `UPPER()` | riya shah | `UPPER("riya shah")` | RIYA SHAH |
| `LOWER()` | RIYA SHAH | `LOWER("RIYA SHAH")` | riya shah |
| `PROPER()` | riya shah | `PROPER("riya shah")` | Riya Shah |
| `TRIM()` | "  Riya Shah  " | `TRIM("  Riya Shah  ")` | Riya Shah |
| `LEN()` | Riya Shah | `LEN("Riya Shah")` | 9 |
| `LEFT()` | iPhone 14 | `LEFT("iPhone 14", 3)` | iPh |
| `RIGHT()` | iPhone 14 | `RIGHT("iPhone 14", 2)` | 14 |
| `CONTAINS()` | Samsung Phone | `CONTAINS("Samsung Phone", "Phone")` | True |
| `REPLACE()` | Office Supplies | `REPLACE("Office Supplies", "Supplies", "Products")` | Office Products |

## 4. Date Functions

TODAY() : Returns the current date.
NOW() : Returns the current date and time.
YEAR() : Returns the year from a date.
MONTH() : Returns the month number from a date.
DAY() : Returns the day of the month.
DATEDIFF() : Calculates the difference between two dates.
DATEADD() : Adds an interval to a date.


## 5. Basic Aggregate Functions

SUM() : Returns the total of values.
AVG() : Returns the average value.
MIN() : Returns the minimum value.
MAX() : Returns the maximum value.
COUNT() : Counts non-Null values.
COUNTD() : Counts unique, non-Null values.





Questions : 

1. Replace Null Profit values with zero using IFNULL().
2. Create a calculated field to categorize orders based on profit using the following conditions:
- If Profit is greater than 200, return "High Profit".
- If Profit is greater than 0 and less than or equal to 200, return "Low Profit".
- Otherwise, return "No Profit".
3. Use CASE to group Technology as Electronics, Furniture as Home Products, and Office Supplies as Office Products.
4. Use IIF() to return High Sales if Sales is greater than 1000, otherwise Low Sales.
5. Use ZN() to replace Null numeric Profit values with zero.
6. Round Sales to two decimal places.
7.Convert Customer Name to uppercase.
8.Convert Customer Name to lowercase.
9.Convert the first letter of each word to uppercase.
10.Find the number of characters in each Customer Name.
11.Extract the first three characters of Product Name.
12.Extract the last three characters of Product Name.
13.Check whether Product Name contains the word "Phone".
14.Replace "Office Supplies" with "Office" in Category.
15.Extract the first character of Customer Name.
16.Display the current date.
17.Display the current date and time.
18.Extract the year from Order Date.
19.Extract the month number from Order Date.
20.Extract the day of the month from Order Date.
21.Calculate how many days each order took to ship.
22.Calculate a date one month after Order Date.
23.Calculate a date seven days after Order Date.

