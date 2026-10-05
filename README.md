#Hiển thị các phần tử lớn nhất trong mảng
tui=[]
n=int(input("nhập số lượng phần tử list:"))
for i in range(n):
    a=int(input(f"nhập arr {i+1}:"))
    tui.append(a)
print("list chưa sort:",end="")
for item in tui:
    print(item,end=" ")
print()
if len(tui)==0:
    print("mảng rỗng !!!")
else:
    maxA=tui[0]
    for item in tui:
        if item > maxA:
            maxA=item
    print(f"các phần tử lớn nhất trong mảng",end=" ")
    for item in tui:
     if item==maxA:
        print(item,end=" ")
#Có bao nhiêu phần tử nhỏ nhất trong số các phần tử là số chính phương trong mảng
tui=[]
n=int(input("nhập số lượng phần tử list:"))
for i in range(n):
    a=int(input(f"nhập arr {i+1}:"))
    tui.append(a)
print("list chưa sort:",end="")
for item in tui:
    print(item,end=" ")
print()
mina=None
for item in tui:
 if item>=0:
    i=1
    while i*i<=item:
        if i*i==item:
           if mina==None or mina>item:
               mina=item
           break
        i=i+1
if mina!=None:
 dem=0
 for item in tui:
    if item==mina:
     dem =dem+1
 print("số phần tử nhỏ nhất trong các số phần tử chính phương là",dem)
else:
    print(" không có số chính phương")
#Sắp xếp mảng giảm dần các phần tử chẵn, tăng dần các phần tử lẻ. Lưu ý là vị trí các phần tử là chẵn hay lẻ giữ nguyên như ban đầu
tui=[]
n=int(input("nhập số lượng phần tử list:"))
for i in range(n):
    a=int(input(f"nhập tui {i+1}:"))
    tui.append(a)
print("list chưa sort:",end="")
for item in tui:
    print(item,end=" ")
print()
tuichan=[]
for item in tui: 
 if item%2 ==0:
    tuichan.append(item)
tuichan.sort(reverse=True)
j=0
for i in range (len(tui)):
    if tui[i]%2==0:
        tui[i]=tuichan[j]
        j=j+1

tuile=[]
for item in tui: 
 if item%2 !=0:
    tuile.append(item)
tuile.sort()
j=0
for i in range (len(tui)):
    if tui[i]%2!=0:
        tui[i]=tuile[j]
        j=j+1
print("list đã sort:",end="")
for item in tui:
    print(item,end=" ")
print()
