# Best Grade

## Question
Andrew has a string N consisting of lowercase English letters representing respective grades of N students 
in his class. His grade is at Pth index. He can swap any two adjacent grades. 
Your task is to help Andrew find and return a string value, representing maximized grade by bringing 
lexicographically smallest character on the Pth index after doing at most K swaps 

## Sample Input:
- abcdefg 
- 3 
- 2 
## Sample Output:
a

## Code:
      s=input()
      p=int(input())
      k=int(input())
      start=max(0,p-k-1)
      end=min(len(s),p+k)
      print(min(list(s[start:end])))

## Output

![Screenshot 2024-06-30 104741](https://github.com/ChaithraDgitub/python-codes/assets/160298555/7757f3f8-f6f9-4441-9f30-249957c95e12)
