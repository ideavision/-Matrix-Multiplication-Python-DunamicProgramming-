# -Matrix-Multiplication-Python-DynamicProgramming-

optimized matrix multiplication Dynamic Programming - Python<br>

## Description:
Input: a chain of matrices to be multiplied that read from txt files.<br>
Output: a parenthesizing of the chain and process calculation and calculation steps <br>
Objective: minimize number of steps needs for the multiplication and calculation steps<br>

## Requirements:
Python 3.x interpreter<br>

## Run:
This is consule Python application , you only need enter this command to run result from txt matrices files.<br>
> python mat1.py<br>

- if you have problem for run problem please check file path or use os module to set path of txt files.<br>

## Short explanation about calculation process in DP approach
M1 = [[11,3],[7,11]] # Dimension 2x2<br>
M2 = [[8,0,1],[0,3,5]] # Dimension 2x3<br>
M3 = [[1],[3],[2]] # Dimension 3x1<br>
arr = 2 x 2 x 2 x 3 x 3 x 1 = [2 x 2 x 3 x 1]<br>

m	 0	1	  2<br>
0	 0	12	10<br>
1	    0	  6<br>
2			    0<br>

M1(M2.M3) = m[0,1] , m[1,2], m[0,2]<br>
[0,1] = > 0,12  2x2x3 =12<br>
[1,2] = > 0,6  2x3x1 =6<br>
[0,2] => 12+ 6 =18<br>

## Result : <br>
Array that chain multiplication from matrices : M(2x2) M(2x3) M(3x1) -->  [2, 2, 3, 1]<br>
0 1 [(0, 12)]<br>
1 2 [(0, 6)]<br>
0 2 [(0, 10), (1, 18)]<br>
( M1 ( M2 M3 ) )<br>

