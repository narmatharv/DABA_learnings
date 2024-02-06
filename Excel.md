## VLOOKUP
```
The VLOOKUP function is a premade function in Excel, which allows searches across columns.

It is typed =VLOOKUP and has the following parts:

=VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])

Lookup_value: Select the cell where search values will be entered.
Table_array: The table range, including all cells in the table.
Col_index_num: The data which is being looked up. The input is the number of the column, counted from the left.
Range_lookup: TRUE if numbers (1) or FALSE if text (0).

How to use VLOOKUP function:
Select a cell (H4)
Type =VLOOKUP
Double click the VLOOKUP command
Select the cell where search value will be entered (H3)
Type (,)
Mark table range (A2:E21)
Type (,)
Type the number of the column, counted from the left (2)
Type True (1) or False (0) (1)
Hit enter
Enter a value in the cell selected for the Lookup_value H3(7)
```

## HLOOKUP
```
HLOOKUP in Excel stands for ‘Horizontal Lookup’. It is a function that makes Excel search for a certain value in a row (the so called ‘table array’), in order to return a value from a different row in the same column.

A HLOOKUP function in Excel exists of 4 components:
1. The value you want to look up;
2. The range in which you want to find the value and the return value;
3, The number of the row within your defined range, that contains the return value;
4. 0 or FALSE for an exact match with the value your are looking for; 1 or TRUE for an approximate match.
Syntax: HLOOKUP([value], [range], [row number], [false or true])


NOTE:  video link:  https://youtu.be/8okA22yMwTs?si=thg-QaSbwH-Z_Phz
```

## XLOOKUP
```
The Excel XLOOKUP function is a modern and flexible replacement for older functions like VLOOKUP, HLOOKUP, and LOOKUP.  XLOOKUP supports approximate and exact matching, wildcards (* ?) for partial matches, and lookups in vertical or horizontal ranges.

Syntax
=XLOOKUP(lookup,lookup_array,return_array,[not_found],[match_mode],[search_mode])
lookup - The lookup value.
lookup_array - The array or range to search.
return_array - The array or range to return.
not_found - [optional] Value to return if no match found.
match_mode - [optional] 0 = exact match (default), -1 = exact match or next smallest, 1 = exact match or next larger, 2 = wildcard match.
search_mode - [optional] 1 = search from first (default), -1 = search from last, 2 = binary search ascending, -2 = binary search descending.

NOTE: video link: https://exceljet.net/functions/xlookup-function

https://youtu.be/Gfu26nNvrsk?si=vDUpO53FXYkwneBO
```
