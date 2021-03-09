# Tugas-Video-5
#program menghitung fpb atau kpk dari 2 bilangan
#input pilihan dari user fpb atau mencari kpk, 2 inputan bilangan 
print('program menghitung FPB dan KPK\n1.FPB\n2.KPK')
pilihan=int(input('masukan pilihan anda:'))
x=int(input('masukan bilangan:'))
y=int(input('masukan bilangan:'))
#proses
n=1
fakx=1
faky=1
if pilihan==1:
    if x<y:
        min=x
    elif y<x:
        min=y
    while n<=min:
        n+=1
        if x%n==0 and y%n==0:
            fpb=n
    print(fpb) #output

elif pilihan==2:
    while x!=y:
        fakx=x*n
        faky=y*n
        n+=1
        if fakx%y==0:
            print(fakx) #output
            break
        elif faky%x==0:
            print(faky) #output
            break
