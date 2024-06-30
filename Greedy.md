## 1.Knapscak problem:
      p=[20,10,6,9,18,12,16,30,15]
      w=[4,5,6,3,2,5,4,6,6]
      p=[5,10,15,7,8,9,4]
      w=[1,3,5,4,1,3,2]
      d=[]
      c=15
      sum=0
      total=0
      dict={}
      for i in range(len(p)):
         a=p[i]/w[i]
         dict[i]=a   
      b=list(dict.values())
      for i in range(len(b)):
          ca=max(b)
          t=b.index(ca)
          d.append(t)
          sum+=w[t]
          b[t]=0
      if sum==c:
             break
      for i in d:
        total=total+p[i]
      print("Maximum profit is:",total)  
