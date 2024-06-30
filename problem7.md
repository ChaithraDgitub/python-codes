#  Minimum Number of Key Presses

## Question

George has a setup which includes a special keyboard and a monitor , that initially displays 
0. The special keyboard has 11 numeric keys (0,1,2,3,4,5,6,7,8,9,00). If he presses 00, the 
previously displayed value will be multiplied by 100. Whereas, if he presses any other 
numeric key, the previously displayed value will be firstly multiplied by 10 and then the 
number on the key will be added to it. 
You are given a numeric string S. Your task is to help George find and return an integer value, 
representing the minimum number of key presses to reach the number. 
## Input Specification:
### input:
A numeric string s. representing the final number, 

## Output Specification:
Return an integer value, representing the minimum number of key presses to reach the 
number. 
### Sample Input:
100 
### Sample Output:
2

## Code:
      s=input()
      i=0
      res=0
      while i<len(s):
         if i<len(s)-1 and s[i]=='0' and s[i+1]=='0':
            i+=2
         else:
            i+=1
         res+=1
      print(res)

## Output
![Screenshot 2024-06-30 100944](https://github.com/ChaithraDgitub/python-codes/assets/160298555/eed773cc-1493-4550-b13d-4ab0a59b3a75)


      
