003 - Arithmetic Operators
Task
Read two integers from STDIN and print three lines where:

The first line contains the sum of the two numbers.
The second line contains the difference of the two numbers (first - second).
The third line contains the product of the two numbers.
Input Format
The first line contains the first integer, a . The second line contains the second integer,b .

Constraints
1 <= a <= 1010

1 <= b <= 1010

Output Format
Print the three lines as explained above.

Sample Inputs
3
2
Sample Output
5
1
6
Explanation
3 + 2 => 5 3 - 2 => 1 3 * 2 => 6

Given Code
if __name__ == '__main__':
    a = int(input())
    b = int(input())
Solution 1
if __name__ == '__main__':
    a = int(input())
    b = int(input())

    print(a + b)
    print(a - b)
    print(a * b)
Solution 2
if __name__ == '__main__':
    a = int(input())
    b = int(input())

    def add_two(x,y):
        return x + y

    def ext_two(x,y):
        return x - y

    def mul_two(x,y):
        return x * y

    print(add_two(a,b))
    print(ext_two(a,b))
    print(mul_two(a,b))
