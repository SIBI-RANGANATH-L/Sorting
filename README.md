# Sorting
#Writing a sorting methods
n=int(input("number of elements:"))
l=[]
for i in range(n):
    num=int(input("enter the element:"))
    l.append(num)
n=len(l)
for i in range(1,n):
    for j in range(0,i):
        if l[j]>l[i]:
            l.insert(j,l[i])
            del l[i+1]
    print(l)
