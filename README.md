#Approach-1
n=int(input())
a=list(map(int,input().split()))
r1=0
r2=0
for i in range(n):
  if a[i]%2==0 and a[i]>r1:
    r1=a[i]
for j in range(n):
  if a[j]%2!=0 and a[j]>r2:
    r2=a[j]
print(r1+r2)

#Approach-2
n=int(input())
a=list(map(int,input().split()))
r1=0
r2=0
for i in range(n):
  if a[i]%2==0 and a[i]>r1:
    r1=a[i]
  elif a[i]>0:
    r2=a[i]
print(r1+r2)

#Approach-3
n=int(input())
a=list(map(int,input().split()))
r1=0
r2=0
for i in a:
  if i%2==0 and i>r1:
    r1=i
  elif i>0:
    r2=i
print(r1+r2)

#Approach-4
n=int(input())
a=list(map(int,input().split()))
e=[]
o=[]
for i in range(n):
  if a[i]%2!=0:
    e.append(a[i])
  elif a[i]>0:
    o.append(a[i])
print(max(e)+max(o))

#Approach-5
n=int(input())
a=list(map(int,input().split()))
e=[]
o=[]
for i in a:
  if i%2!=0:
    e.append(i)
  elif i>0:
    o.append(i)
print(max(e)+max(o))

#Approach-6
n=int(input())
a=list(map(int,input().split()))
e=[0]
o=[0]
for i in a:
  if i%2!=0:
    e.append(i)
  elif i>0:
    o.append(i)
print(max(e)+max(o))
