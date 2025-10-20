print('The length of DNA of flu A in 2024')

x1=[]
scores1=[]

for i in df['length']:
      scores1.append(i)
      for i in scores1:
          if i not in x1:
              x1.append(i)

x1=sorted(x1)

x=[]
r = [i for i in x1 if 800 < i < 1200]
if r:
    average = sum(r) / len(r)
    x.append(average)
r1=[i for i in x1 if 1200<i<1600]
if r1:
    average1=sum(r1)/len(r1)
    x.append(average1)

r2=[i for i in x1 if 1600<i<2000]
if r2:
    averge2=sum(r2)/len(r2)
    x.append(averge2)
r3=[i for i in x1 if i>2000]
if r3:
