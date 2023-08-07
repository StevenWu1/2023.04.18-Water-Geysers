# 2023.04.18-Water-Geysers
Marlin and Nemo are trapped in a aquarium and need to get out to help Dory. They see water geysers shooting out of the ground, and they think about what Dory would do (she'd jump out of the aquarium and bounce on the geysers!). Before making the leap, they decide to calculate the biggest strictly decreasing drop or biggest strictly increasing jump they will be making between consecutive geysers along their path. For example, if the heights of the geysers were 1, 3, 6, 4, 8, then the biggest change in height along consecutive geysers would be from 1 to 6 (so 5). If the heights were 1, 3, 6, 4, 8, 1, then the biggest change in height be from 8 to 1 (so 7). But if the heights were 1, 3, 3, 7, then the biggest change in height would be from the second 3 to the 7 (a gap of 4) - it would not be from 1 to 7, as that path is not strictly increasing!

Your goal will be to write a program that calculates this value.

https://drive.google.com/file/d/0BxxolsFkwnDqTFRscmN4dGpHdjA/view?usp=sharing

##### Input Format
There will be one line of input. The line will begin with a single positive integer n, followed by n non-negative integers Ai, all separated by spaces.

##### Constraints
2 <= n <= 1000 0 <= Ai <= 1000

##### Output Format
A single number m, representing the largest absolute difference along a strictly increasing or decreasing subsequence.

##### Sample Input 0
5 1 3 6 4 8

##### Sample Output 0
5

##### Sample Input 1
6 1 3 6 4 8 1

##### Sample Output 1
7

##### Sample Input 2
4 1 3 3 7

##### Sample Output 2
4
