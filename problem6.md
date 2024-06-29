#  Encode The Number

## Question
You work in the message encoding department of a national security agency. Every message 
that is sent from or received in your office is encoded. You have an integer N, and each digit 
of N is squared and the squares are concatenated together to encode the original number. 
Your task is to find and return an integer value representing the encoded value of the 
number. 
## Input:
An integer value N representing the number to be encoded. 
## Output :
Return an integer value representing the encoded value of the number. 
## Sample Input:
167 
## Sample Output:
13649 

## code1:
       L=[]
       a=input()
       b=list(a)
       c=len(b)
      for i in range(c):
         L.append(int(b[i]))
      for i in L:
         print(i**2,end='')
## code 2:
      num=str(input())
      res=''
      for i in num:
         res+=str(int(i)*int(i))
      print(res) 
## Output
![Screenshot 2024-06-29 153954](https://github.com/ChaithraDgitub/python-codes/assets/160298555/a65494fe-25b4-4838-b323-5a328839e4d6)

      
         
    
