025 - The Minion Game
Problem
Kevin and Stuart want to play the The Minion Game.

Game Rules

Both players are given the same string S.
Both players have to make substrings using the letters of the string S.
Stuart has to make words starting with consonants.
Kevin has to make words starting with wovels.
The game ends when both players have made all possible substrings.


Scoring

A player gets +1 point for each occurrence of the substring in the string S.


For Example

String S = BANANA
Kevin's wovel beginning word = ANA
Here, ANA occurs twice in BANANA. Hence, Kevin will get 2 points.


For better understanding, see the image below :




Input Format
A single line of input containing the full name, S.

Note : The string S will contain only uppercase letters: [A - Z].


Constraints
0 < len(S) < 106


Output Format
Print one line : the name of the winner and their score separated by a space.

If the game is a draw, print Draw


Sample Input

BANANA

Sample Output

Stuart 12

Note: Vowels are only defined as AEIOU. In this problem, Y is not considered a vowel.


Given Code
def minion_game(string):
    # your code goes here

if __name__ == '__main__':
    s = input()
    minion_game(s)
Solution
def minion_game(string):
    wovels = "AEIOU"

    kev = 0
    stu = 0

    for i in range(len(string)):
        if s[i] in wovels:
            kev += len(string)-i
        else:
            stu += len(string)-i

    if kev > stu:
        print("Kevin", kev)
    elif kev < stu:
        print("Stuart", stu)
    else:
        print("Draw")
