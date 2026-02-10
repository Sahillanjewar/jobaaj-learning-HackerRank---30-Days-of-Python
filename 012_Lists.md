012 - Lists
Problem
Consider a list (list = []). You can perform the following commands:

insert i e : Insert integer e at position i
print : Print the list
remove e : Delete the first occurrence of integer e
append e : Insert integer e at the end of the list
sort : Sort the list
pop : Pop the last element from the list
reverse : Reverse the list
Initialize your list and read in the value of n followed by n lines of commands where each command will be of the 7 types listed above. Iterate through each command in order and perform the corresponding operation on your list.

Input Format
The first line contains an integer, n, denoting the number of commands.

Each line i of the n subsequent lines contains one of the commands described above.

Constraints
The elements added to the list must be integers

Output Format
For each command of type print, print the list on a new line.

Sample Input 0

12
insert 0 5
insert 1 10
insert 0 6
print
remove 6
append 9
append 1
sort
print
pop
reverse
print
Sample Output 0

[6, 5, 10]
[1, 5, 9, 10]
[9, 5, 1]

Given Code
if __name__ == '__main__':
    N = int(input())
Solution
if __name__ == '__main__':
    N = int(input())
    the_list = list()

    for _ in range(N):
        query = input().split()
        if query[0] == "print":
            print(the_list)
        elif query[0] == "insert":
            the_list.insert(int(query[1]), int(query[2]))
        elif query[0] == "remove":
            the_list.remove(int(query[1]))
        elif query[0] == "append":
            the_list.append(int(query[1]))
        elif query[0] == "sort":
            the_list = sorted(the_list)
        elif query[0] == "pop":
            the_list.pop()
        elif query[0] == "reverse":
            the_list.reverse()
