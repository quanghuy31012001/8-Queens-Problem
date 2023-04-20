# 8-Queens-Problem
The idea is to place queens one by one in different columns, starting from the 
leftmost column. When we place a queen in a column, we check for clashes with 
already placed queens. In the current column, if we find a row for which there is no 
clash, we mark this row and column as part of the solution. If we do not find such a 
row due to clashes then we backtrack and return false
1. begin from the leftmost column
2. if all the queens are placed,return true/ print configuration
3. check for all rows in the current column
 a) if queen placed safely, mark row and column; and recursively check if we 
approach in the current configuration, do we obtain a solution or not
 b) if placing yields a solution, return true
4
 c) if placing does not yield a solution, unmark and try other rows
4. if all rows tried and solution not obtained, return false and backtrack
