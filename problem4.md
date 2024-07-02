# Elections

## Questions

You are the head of the election committee in your village. Each Political party is associated 
with a unique number and the votes are represented as an integer array A. where each 
element contains the party number voted for by the villagers. For a party to win, they must 
have a majority of votes. our task is to find and return an integer value denoting the winning 
party's number. Return -1 if there is no party with a majority.

### Note: If only one vote is there he is the winner. 
## Input Format :
### input1:
An integer value representing the number the number of voters 
### input2: 
An integer array A representing the votes of the 
voters. 
## output Format: 
Return an integer value denoting the winning party's number.Return -1 there is no party 
with a majority 
### Example 1:
## Input
- 6 
- 1 1 2 2 2 3
 ## Output:
- 2 
### Explanation:
As 2 got the most number of votes i.e 3. 
### Example 2:
##  Input:
- 6
- 1 2 3 2 1
## Output:
- -1 
### Explanation:
- As both the contestants got same votes there is no majority.

# Code:

      dict={}
      N=int(input("enter the number of votes:"))
      votes=list(map(int,input().split()))
      for i in votes:
         if i in dict:
           dict[i]+=1
         else:
           dict[i]=1  
      print(dict) 
      b=list(dict.values())
      r=b.copy()
      c=(max(b))
      (b.remove(c))
      print(b)
      print(r)
      if c in b:
          print(-1)
      else:
          print(b.index((max(b)))+1) 

 # Output 1

![Screenshot 2024-06-28 222550](https://github.com/ChaithraDgitub/python-codes/assets/160298555/0ca259e3-5d89-4931-bcdd-52c47d088a80)
       
        
 # Output 2
 ![Screenshot 2024-06-28 221915](https://github.com/ChaithraDgitub/python-codes/assets/160298555/60c8a20b-249e-404a-a854-ca2aa337440a)
