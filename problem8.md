# Special String

## Question
Alice has a string A consisting of lowercase English letters. Her friend gives her another string S and asks 
her to modify string A and replace its characters with the characters present in string S. 
But, to achieve the above task, Alice must follow the below steps: 
1. Choose a character from string S that has the minimum ASCII distance from the ith character in string A 
2. Replace the ith character in string A with the chosen character in string S 
Your task is to find and return an integer value, representing minimum total ASCII distance that is required 
to modify string A to the characters in string S. Return 0, if all the characters in string S are already present 
in string A 

## Sample Input
 - abcd
 - xyz 
## Sample Output
- 86

## Code:
      A=list(input())
      S=list(input())
      L=[]
      sum=0
      for i in range(len(A)):
           for j in range(len(S)):
              a=ord(A[i])-ord(S[j])
              L.append(abs(a))
              break
           b=min(L)
           sum+=b
           L.clear()
      print(sum) 

## Output

![Screenshot 2024-06-30 101943](https://github.com/ChaithraDgitub/python-codes/assets/160298555/79ce589f-c498-48ee-9feb-5c594aab8f8e)


