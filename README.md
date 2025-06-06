# Code.project
import random
sz=int(input("enter lenght of password:"))
'''for i in range(1,sz):
    x=random.randint(33,127)
    print(end=chr(x))
print("\n")
print("Done!!!")'''
Alist=[]
for i in range(65,91):
    Alist=Alist+list(chr(i))
print(Alist)
alist=[]
for i in range(97,123):
    alist=alist+list(chr(i))
print(alist)
num=[]
for i in range(1,10):
    num=num+list(str(i))
print(num)
spchlist=[]
for i in range(33,47):
    spchlist=spchlist+list(chr(i))
print(spchlist)
'''
if(sz==16):
    newAlist=[]
    for i in range(1,len(Alist)):
        newAlist+=list(random.choice(Alist))
        if(i==4):
            break
    print(newAlist)
    
    newalist=[]
    for i in range(1,len(alist)):
        newalist+=list(random.choice(alist))
        if(i==8):
            break
    print(newalist)
    
    newnum=[]
    for i in range(1,len(num)):
        newnum+=list(random.choice(num))
        if(i==2):
            break
    print(newnum)
    
    newspchlist=[]
    for i in range(1,len(spchlist)):
        newspchlist+=list(random.choice(spchlist))
        if(i==2):
            break
    print(newspchlist)
    f16=newAlist+newspchlist+newalist+newnum
    print("Final password for 16 length password:",f16)
elif(sz==12):
    newAlist=[]
    for i in range(1,len(Alist)):
        newAlist+=list(random.choice(Alist))
        if(i==3):
            break
    print(newAlist)
    
    newalist=[]
    for i in range(1,len(alist)):
        newalist+=list(random.choice(alist))
        if(i==6):
            break
    print(newalist)
    
    newnum=[]
    for i in range(1,len(num)):
        newnum+=list(random.choice(num))
        if(i==2):
            break
    print(newnum)
    
    newspchlist=[]
    for i in range(1,len(spchlist)):
        newspchlist+=list(random.choice(spchlist))
        if(i==1):
            break
    print(newspchlist)
    f12=newAlist+newspchlist+newalist+newnum
    print("Final password for 16 length password:",f12)'''
def find_pass(int):
    newAlist=[]
    for i in range(1,len(Alist)):
        newAlist+=list(random.choice(Alist))
        if(i==sz/4):
            break
    print(newAlist)
    
    newalist=[]
    for i in range(1,len(alist)):
        newalist+=list(random.choice(alist))
        if(i==sz/2):
            break
    print(newalist)
    
    newnum=[]
    for i in range(1,len(num)):
        newnum+=list(random.choice(num))
        if(i==sz/8):
            break
    print(newnum)
    
    newspchlist=[]
    for i in range(1,len(spchlist)):
        newspchlist+=list(random.choice(spchlist))
        if(i==sz/8):
            break
    print(newspchlist)
    flist=newAlist+newspchlist+newalist+newnum
    print("Final password for 16 length password:",flist)
find_pass(sz)
