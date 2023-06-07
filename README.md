# Pavani_AnagramProgram
def anagram(l):
 l1=[]
 for i in l:
  l2=[]
  for j in l:
   if(sorted(list(i))==sorted(list(j)) and j!='0'):
    index=l.index(j)
    l[index]='0'
    l2.append(j)
  if(len(l2)>1):
   l1.append(l2)
 return l1

l=[i for i in input().split(",")]
print(anagram(l))
