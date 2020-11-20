# -Matrix-Multiplication-Python-DunamicProgramming-


M1 = [[11,3],[7,11]] # Dimension 2x2
M2 = [[8,0,1],[0,3,5]] # Dimension 2x3
M3 = [[1],[3],[2]] # Dimension 3x1
arr = 2 x 2 x 2 x 3 x 3 x 1 = [2 x 2 x 3 x 1]

m	 0	1	  2
0	 0	12	10
1	    0	  6
2			    0

M1(M2.M3) = m[0,1] , m[1,2], m[0,2]
[0,1] = > 0,12  2x2x3 =12
[1,2] = > 0,6  2x3x1 =6
[0,2] => 12+ 6 =18

## Result : 
Array that chain multiplication from matrices : M(2x2) M(2x3) M(3x1) -->  [2, 2, 3, 1]
0 1 [(0, 12)]
1 2 [(0, 6)]
0 2 [(0, 10), (1, 18)]
( M1 ( M2 M3 ) )

