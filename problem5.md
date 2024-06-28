# Minimum Array sum

## Question
Paul is given an array A of length N. He must perform the following Operations on the array 
sequentially: 
* Choose any two integers from the array and calculate their average. 
* If an element is less than the average, update it to 0. However, if the element is greater 
  than or equal to the average, he need not update it. 
Your task is to help Paul find and return an integer value, representing the minimum possible 
sum of all the elements in the array by performing the above operations. 
### Note: An exact average should be calculated, even if it results in a decimal. 
## Input Format:
### input1:
An integer value N, representing the size of the array A. 
### input2:
An integer array A. 
## Output Format:
Return an integer value, representing the minimum possible sum of all the elements in the 
array by 
### Sample Input
5 
1 2 3 4 5 
### Sample Output
5
## Code:
       N=int(input("enter the length of array:"))
       arr=list(map(int,input("enter the values:").split()))
       max1=max(arr)
       arr.remove(max1)
       max2=max(arr)
       arr.append(max1)
       avg=(max1+max2)/2
       for i in range(len(arr)):
          if arr[i]<avg:
             arr[i]=0
       print(sum(arr))
## Output

![Screenshot 2024-06-28 223536](https://github.com/ChaithraDgitub/python-codes/assets/160298555/d3080abe-a6a7-4f4f-a68a-d5c375c1fc27)


       
