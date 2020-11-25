# Python
print ('merhaba')

print ('patataesasdaskdjaskşldkasşldkaşsd')

a = 'selamlar'
print (a)

print (ax2)

print (a*3)

c = 1
d = 2
print (c)
print (d)
print ('======')
c,d = d,c
print ('======')
print (c)
print (d)

input ('sayı giriniz')

girilenSayi = input('Sayı giriniz')
print ('girdiğiniz sayı şudur:',girilenSayi)

isminizNedir = input('Adınız nedir?')
print ('Adınızı öğrendim ->', isminizNedir)

zbap = ('ivj')
len(zbap)

saç = 2
print(saç)

a = ('herkese selamlar')
a[6]
a[4:7]
a[:4]
a[3]
a[2:8:2]
a[::2]

liste = [1,2,3,5,6]
liste.append(329847)
print(liste)

# ========GÜN-2=============

# OPERATÖRLER

10 / 3
5 * 2
5 / 1
8 // 2
10 % 3  --> #Kalan ifade ediyor

abs (-3) #mutlak değeri verir
round(4.6) #yuvarlıyor

liste = [3,4,6,2,7]
max(liste)
min(liste)
sum(liste)  #topluyor

                 #sondaki atlama terimi
for i in range(2,6,2):    
  print(i)     #range 2den 6ya liste

a = 3
a +=2 #= a = a +2
a *=4 
a /=3
a **=2
a *=2
a //=3

#işlemleri sırasıyla yapıyor
    
print (a)

a = 3
b = 4
a == b   
a != b
a < b
a >= b

a = 1
b = 2
c = 3
d = 4

a == b and c != d
a == b    or    c != d
not (a == b and c != d)    #fasa fiso

x = 3           
y = 5

print (id(x))
print (id(y)) 
                        #fasa fiso
x is y 
x is not y

liste = [54,61,45,34,2]
54 in liste 
123 not in liste

#Bitwise operatörleri!!
#2lik ve onluk sistem olayı var

bin(45) #---> 101101
bin (3) #---> 11
bin(5) #---> 101
bin(360) #---> 101101000

45>>3  #= 5      #bu işlem soldaki sayının 2lik sistemdeki gösteriminden sondaki üç haneyi çıkarıyor ardından
                  #çıkan sonucu normal sayı olarak yazıyor
    
45<<3  #=360     #bu işlem ise baştaki sayının 2lik gösterimine sağda belirtildiği kadar sıfır ekle 
45<<8             #ve çıkan sonucu normal sayı olarak yaz

        #bu üçü de sırasıyla        
45|3    #veya
45&3    #ve
45^3    #anlatması güç                        (ikilik gösterimler için geçerlidir)
~45    # bu da zıttını işaret ediyor     

# KOŞULLAR

if-elif else

if True:                                    #baş harf büyük
    print('patates')                        #yeniden sayfa başına dönersen if'in hükümü kalkar

print('sucuk')

#sırayla deniyor hangisi doğru çıkarsa o işlemi gerçekleştiriyor. eskilerden not ekliyorum: a!=b -> a eşit değil b demektir 

a = 45
b = 42

if a<b:
    a+=10
    print(a)                           #elifler işe yaramazsa son olarak else yazıp istediğin işlemi yaptırıyorsun
    
elif a==b:
    a+=20
    print(a)

elif a<=b:
    a+=33
    print(a)
    
else:
    a+=666
    print(a)

a = 3
b = 4

print('Çalışıyor') if a>b else print('Çalışmıyor')

ilkDeğer = input('İlk değeri giriniz.')
ikinciDeğer = input('İkinci değeri giriniz')

if ilkDeğer > ikinciDeğer:
    print('İlk girdiğiniz değer ikinci girdiğiniz değerden büyüktür.')
elif ilkDeğer < ikinciDeğer:
    print('İkinci girdiğiniz değerilk girdiğiniz değerden büyüktür.')
else:
    print('Girdiğiniz iki değer birbirine eşittir.')

# DÖNGÜLER

## FOR DÖNGÜSÜ
liste = [54,45,342,643]
for i in liste:
    print(i)


metin = 'ptts'                   #sayılarda döngüler çalışmaz
for x in metin:
    print(x)

#break
liste = [54,'sakarya','güzel',88,23,2,3,4,5,6,]
for i in liste:
    if i==23:
        break
    print(i)


#continue
liste = [54,'sakarya','güzel',88,23,2,3,4,5,6,]
for i in liste:
    if i==23:
        continue
    print(i)


#pass
liste = [54,'sakarya','güzel',88,23,2,3,4,5,6,]
for i in liste:
    if i==23:
        pass
    print(i)



#for range ile çok kullanılacak
for i in range(1,4):
    print('patates')

## WHILE DÖNGÜSÜ

x = 56

if x>2:
    print('patates kafa')
    
while x>3:
    print('abo')
    x = x/2

i = 1
while i < 6:
    print('i=',i)
    if i == 4:
        break
    i += 1

        
    

i = 1
while i < 6:
    print("i: ",i)
    i+=1
    if i == 3:
        continue
    #i+=1

i = 1
while i < 6:
    print("i: ",i)
    if i == 3:
        pass
    i += 1

#else
i = 1
while i < 6:
    print("i: ",i)
    i += 1
    
else:
    print('olmadı')

#İÇ İÇE DÖNGÜLER

meyveler = ['elma','armut','muz']
sayılar = [54,61,34,45]
for x in meyveler:
    for y in sayılar:
        print(x,y)

# List Comprehension #buraları oku


liste = [3,5,2,6,1]
yeniListe = []

for i in liste:
    yeniListe.append(i)
    
print(yeniListe)

yeniListe = [i for i in liste]
print(yeniListe)


yeniListe = [i**2 for i in liste]
print(yeniListe)

liste1 = [1,2,3,4,5,6,7,8,9]
liste2 = list()

for i in liste1: 
    if i % 2 == 0 or i == 9:
        liste2.append(i)
        
print(liste2)


liste2 = [i**3 for i in liste1 if (i % 2 == 0 or i == 9)]
print(liste2)

# =================== GÜN 3 ======================

# Fonksiyonlar

#void fonksiyon          #return fonksiyon edemiyorsak void diyoruz
isim = input('isminiz nedir')
print(f'hoşgeldin kardeş {isim}')

isim = input('isminiz nedir')
print(f'hoşgeldin kardeş {isim}')

isim = input('isminiz nedir')
print(f'hoşgeldin kardeş {isim}')

isim = input('isminiz nedir')
print(f'hoşgeldin kardeş {isim}')


def hosgeldin(ad,soyad):
    print("Hoşgeldin ",ad,soyad)
    
isim = input("İsminizi öğrenebilir miyim? ")
soyisim = input("Soyadınızı öğrenebilir miyim? ")

hosgeldin(isim,soyisim)

def hosgeldin(ad,soyad):
    print("Hoşgeldin ",ad,soyad)
    
isim = input("İsminizi öğrenebilir miyim? ")
soyisim = input("Soyadınızı öğrenebilir miyim? ")

hosgeldin(isim,soyisim)


selam = hosgeldin
selam("Abdülkerim","Şahin")

### Argümanlar
#*args

def calisan(*bilgiler):
    print('çalışanlarımın bilgileri: ')
    for i in bilgiler:
        print(i)
calisan('adam','gibi','adamlarda','bugün')

#**kwargs

def calisan(**bilgiler):
    print('İkametgah: ',bilgiler['ikametgah'])
    print('İş Yeri: ',bilgiler['işyeri'])
    print('Soyadı: ',bilgiler['soyadi'])
    print('Adı:',bilgiler['adi'])
calisan(adi='Salakmatik',soyadi='patatesköfte',ikametgah='çöplük',işyeri='Tımarhane')

#return
def topla(x,y):
    toplam = x+y
    return toplam

sonuc = topla(3333,4)
print(sonuc)
type(x)

#pass <- gereksiz dendi
def fonksiyon():
    pass

#Lambda
#def topla(x,y):
#   return x+y

topla = lambda x,y : x + y
topla(3,4)

carp = lambda x,y,e,s,f,t,w : x - e * y / w + t + f **s      #çorba ;)
carp(3,77,33,42,545,634,643)

# MODÜLLER 

import math
math.sqrt(16)

def patates(x):
    return x**(0.5)
patates(4)
    

import math as matematik
matematik.sqrt(3434)

from math import sqrt,factorial
factorial(5)

## hatalar

try:
    print('a')
except NameError:
    print('NameError ile karşılaştım')
except ValueError:
    print('ValueError ile karşılaştım')
except:
    print('i have no idea')

try:
    print('a')
except NameError:
    print('NameError ile karşılaştım')
except ValueError:
    print('ValueError ile karşılaştım')
except:
    print('i have no idea')
else:
    print('her şey yolunda')

try:
    print(a)
except NameError:
    print('NameError ile karşılaştım')
except ValueError:
    print('ValueError ile karşılaştım')
except:
    print('i have no idea')
else:
    print('her şey yolunda')
finally:
    print('patates köfte')

# =======================-GÜN-4-==============================

##  NESNE TABANLI PROGRAMLAMA

#### Sınıf(Class) ve Nesne (Object)

class kitap():
    pass

kitap1=kitap()
kitap2=kitap()

kitap1.ad='Salakhane'
kitap1.yazar='Tuna Okulu'
kitap2.ad='Kerizler'
kitap2.yazar='Bunyamin Şahan'

print(kitap1.ad)
print(kitap1.yazar)
print(kitap2.ad)
print(kitap2.yazar)

### init ve self

class kitap():
    def __init__(self,ad,yazar):
        self.ad = ad
        self.yazar = yazar
kitap1 = kitap('Salakhane','Tuna Okulu')
print(kitap1.ad)

### Metodlar Class'lara ait fonksiyonlar

class kitap():
    def __init__(self,ad,yazar,sayfa):
        self.ad = ad
        self.yazar = yazar
        self.sayfa = sayfa
    
    def bilgileriGöster(self):
        return print('Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {}'.format(self.ad,self.yazar,self.sayfa))
    
    def degerArttir(self,deger):
        self.sayfa += deger #!
     
    
    
kitap1=kitap('Salakhane','Tuna Okulu',123)
kitap1.bilgileriGöster()
kitap1.degerArttir(113) #!               ###BAKILSINN

### Class variables & instance variables

class kitap():
    kutuphaneninAdi='Universite Kütüphanesi'
    def __init__(self,ad,yazar,sayfa):
        self.ad = ad
        self.yazar = yazar
        self.sayfa = sayfa
    
    def bilgileriGöster(self):
        return print('Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {}'.format(self.ad,self.yazar,self.sayfa))
    
kitap1=kitap('Salakhane','Tuna Okulu',123)
kitap2=kitap('Kerizler','Bunyamin Şahan',31)


kitap.kutuphaneninAdi
kitap1.kutuphaneninAdi

kitap1.ad
kitap2.ad

kitap.kutuphaneninAdi='İTÜ Kütüphanesi'
kitap.kutuphaneninAdi

class kitap():
    kutuphaneninAdi='Universite Kütüphanesi'
    kitapSayisi = 0
    kitapID = 1000
    def __init__(self,ad,yazar,sayfa):
        self.ad = ad
        self.yazar = yazar
        self.sayfa = sayfa
        kitap.kitapSayisi += 1
        self.kitapID += 10
        kitap.kitapID = self.kitapID
    def bilgileriGöster(self):
        return print('Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {}'.format(self.ad,self.yazar,self.sayfa))
    
kitap1=kitap('Salakhane','Tuna Okulu',123)
kitap2=kitap('Kerizler','Bunyamin Şahan',31)
kitap3=kitap('Armutlar','Fatih Çelik',445)




kitap.kitapSayisi
kitap2.kitapSayisi
kitap1.kitapID

### Metodlar vs

class kitap():
    kutuphaneninAdi='Universite Kütüphanesi'
    kitapSayisi = 0
    kitapID = 1000
   
    def __init__(self,ad,yazar,sayfa = 'Bilgi Girilmedi'):
        self.ad = ad
        self.yazar = yazar
        self.sayfa = sayfa
        kitap.kitapSayisi += 1
        self.kitapID += 10
        kitap.kitapID = self.kitapID
    #instance metod
    def bilgileriGöster(self):
        return print('Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {}'.format(self.ad,self.yazar,self.sayfa))
    #class metod
    @classmethod
    def kitapSayısınıSöyle(cls):
        return kitap.kitapSayisi
    #classmetod
    @classmethod
    def stringİleOluştur (cls,metin):
        ad,yazar = metin.split(' ')
        return cls(ad,yazar,)
    #static method
    @staticmethod
    def kutuphaneAdiniSöyle():
        return kitap.kutuphaneninAdi
        
    
kitap1=kitap('Salakhane','Tuna Okulu',21)
kitap2=kitap('Kerizler','Bunyamin Şahan',31)
kitap3=kitap('Armutlar','Fatih Çelik',445)
kitap4=kitap.stringİleOluştur('Saplayıcılar M.EnesOnuş')




#kitap1.kitapSayisi

#kitap.kitapSayısınıSöyle()
#kitap4.bilgileriGöster()


kitap.kutuphaneAdiniSöyle()

## Kalıtım

class kitap():
    kutuphaneninAdi='Universite Kütüphanesi'
    kitapSayisi = 0
    kitapID = 1000
   
    def __init__(self,ad,yazar,sayfa = 'Bilgi Girilmedi'):
        self.ad = ad
        self.yazar = yazar
        self.sayfa = sayfa
        kitap.kitapSayisi += 1
        self.kitapID += 10
        kitap.kitapID = self.kitapID
    #instance metod
    def bilgileriGöster(self):
        return print('Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {} \n'.format(self.ad,self.yazar,self.sayfa))
    #class metod
    @classmethod
    def kitapSayısınıSöyle(cls):
        return kitap.kitapSayisi
    #classmetod
    @classmethod
    def stringİleOluştur (cls,metin):
        ad,yazar = metin.split(' ')
        return cls(ad,yazar,)
    #static method
    @staticmethod
    def kutuphaneAdiniSöyle():
        return kitap.kutuphaneninAdi

    
    

class bayraktarKitaplar(kitap):
    pass
class anayurtKitaplar(kitap):
    pass

bayraktarKitap1 = bayraktarKitaplar('Salakhane','Tuna Okulu', 21)
bayraktarKitap1.bilgileriGöster()

anayurtKitaplar1 = anayurtKitaplar('Armutlar', 'Fatih Çelik', 45)
anayurtKitaplar1.bilgileriGöster()

class anayurtKitaplar(kitap):
    def __init__(self,ad,yazar,sayfa,cevirmen):
        self.ad = ad
        self.yazar = yazar
        self.sayfa = sayfa
        self.cevirmen = cevirmen
    def bilgileriGöster(self):
        return print('Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {} \nKitabın Çevirmeni: {}\n '.format(self.ad,self.yazar,self.sayfa,self.cevirmen))
    
    def cevirmenDeğiştir(self,yeniÇevirmen):
        self.cevirmen = yeniÇevirmen
        
        
anayurtKitaplar1 = anayurtKitaplar('Armutlar', 'Fatih Çelik', 45, 'M.Ali Çiçek')
anayurtKitaplar1.bilgileriGöster()
print('-İşler Değişti Aslan')
print(' ')
anayurtKitaplar1.cevirmenDeğiştir('Furkan Aydemir')
anayurtKitaplar1.bilgileriGöster()

### super().init

class anayurtKitaplar(kitap):
    def __init__(self,ad,yazar,sayfa,cevirmen):
        super().__init__(ad,yazar,sayfa)
        self.cevirmen = cevirmen
    def bilgileriGöster(self):
        return print('Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {} \nKitabın Çevirmeni: {}\n '.format(self.ad,self.yazar,self.sayfa,self.cevirmen))
    
    def cevirmenDeğiştir(self,yeniÇevirmen):
        self.cevirmen = yeniÇevirmen

anayurtKitaplar1 = anayurtKitaplar('Armutlar', 'Fatih Çelik', 45, 'M.Ali Çiçek')
anayurtKitaplar1.bilgileriGöster()
print('-İşler Değişti Aslan')
print(' ')
anayurtKitaplar1.cevirmenDeğiştir('Furkan Aydemir')
anayurtKitaplar1.bilgileriGöster()

## Dunder (Magic Special) Methods

liste = [54,45,62,61]
#type(liste)
#dir(liste)

### str

#bu kodda bilgileri göster kodunu silip str ekledik böylese direkt print diyince çalışacak. bu arada 
#returnun önündeki printi de sildik

class kitap():
    kutuphaneninAdi='Universite Kütüphanesi'
    kitapSayisi = 0
    kitapID = 1000
   
    def __init__(self,ad,yazar,sayfa = 'Bilgi Girilmedi'):
        self.ad = ad
        self.yazar = yazar
        self.sayfa = sayfa
        kitap.kitapSayisi += 1
        self.kitapID += 10
        kitap.kitapID = self.kitapID
    #instance metod
    def __str__(self):
        return 'Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {} \n'.format(self.ad,self.yazar,self.sayfa)
    #class metod
    @classmethod
    def kitapSayısınıSöyle(cls):
        return kitap.kitapSayisi
    #classmetod
    @classmethod
    def stringİleOluştur (cls,metin):
        ad,yazar = metin.split(' ')
        return cls(ad,yazar,)
    #static method
    @staticmethod
    def kutuphaneAdiniSöyle():
        return kitap.kutuphaneninAdi

    
kitap1=kitap('Salakhane','Tuna Okulu',21)
kitap2=kitap('Kerizler','Bunyamin Şahan',31)
kitap3=kitap('Armutlar','Fatih Çelik',445)
kitap4=kitap.stringİleOluştur('Saplayıcılar M.EnesOnuş')
 

print(kitap1)

### len

lise = [2,3,4]
len(lise)

class kitap():
    kutuphaneninAdi='Universite Kütüphanesi'
    kitapSayisi = 0
    kitapID = 1000
   
    def __init__(self,ad,yazar,sayfa = 'Bilgi Girilmedi'):
        self.ad = ad
        self.yazar = yazar
        self.sayfa = sayfa
        kitap.kitapSayisi += 1
        self.kitapID += 10
        kitap.kitapID = self.kitapID
    #instance metod
    def __str__(self):
        return 'Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {} \n'.format(self.ad,self.yazar,self.sayfa)
    #class metod
    @classmethod
    def kitapSayısınıSöyle(cls):
        return kitap.kitapSayisi
    #classmetod
    @classmethod
    def stringİleOluştur (cls,metin):
        ad,yazar = metin.split(' ')
        return cls(ad,yazar,)
    #static method
    @staticmethod
    def kutuphaneAdiniSöyle():
        return kitap.kutuphaneninAdi
    def __len__(self):
        return self.sayfa
        
kitap1=kitap('Salakhane','Tuna Okulu',21)
kitap2=kitap('Kerizler','Bunyamin Şahan',31)
kitap3=kitap('Armutlar','Fatih Çelik',445)
kitap4=kitap.stringİleOluştur('Saplayıcılar M.EnesOnuş')
 

len(kitap1)

### add

class kitap():
    kutuphaneninAdi='Universite Kütüphanesi'
    kitapSayisi = 0
    kitapID = 1000
   
    def __init__(self,ad,yazar,sayfa = 'Bilgi Girilmedi'):
        self.ad = ad
        self.yazar = yazar
        self.sayfa = sayfa
        kitap.kitapSayisi += 1
        self.kitapID += 10
        kitap.kitapID = self.kitapID
    #instance metod
    def __str__(self):
        return 'Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {} \n'.format(self.ad,self.yazar,self.sayfa)
    #class metod
    @classmethod
    def kitapSayısınıSöyle(cls):
        return kitap.kitapSayisi
    #classmetod
    @classmethod
    def stringİleOluştur (cls,metin):
        ad,yazar = metin.split(' ')
        return cls(ad,yazar,)
    #static method
    @staticmethod
    def kutuphaneAdiniSöyle():
        return kitap.kutuphaneninAdi
    def __len__(self):
        return self.sayfa
    def __add__(self,other):
        return self.ad + other.ad
        
        
kitap1=kitap('Salakhane','Tuna Okulu',21)
kitap2=kitap('Kerizler','Bunyamin Şahan',31)
kitap3=kitap('Armutlar','Fatih Çelik',445)
kitap4=kitap.stringİleOluştur('Saplayıcılar M.EnesOnuş')
 

print(kitap1+kitap2)



### mul

class kitap():
    kutuphaneninAdi='Universite Kütüphanesi'
    kitapSayisi = 0
    kitapID = 1000
   
    def __init__(self,ad,yazar,sayfa = 'Bilgi Girilmedi'):
        self.ad = ad
        self.yazar = yazar
        self.sayfa = sayfa
        kitap.kitapSayisi += 1
        self.kitapID += 10
        kitap.kitapID = self.kitapID
    #instance metod
    def __str__(self):
        return 'Kitabın Adı: {} \nKitabın Yazarı: {} \nKitabın Sayfa Sayısı: {} \n'.format(self.ad,self.yazar,self.sayfa)
    #class metod
    @classmethod
    def kitapSayısınıSöyle(cls):
        return kitap.kitapSayisi
    #classmetod
    @classmethod
    def stringİleOluştur (cls,metin):
        ad,yazar = metin.split(' ')
        return cls(ad,yazar,)
    #static method
    @staticmethod
    def kutuphaneAdiniSöyle():
        return kitap.kutuphaneninAdi
    def __len__(self):
        return self.sayfa
    def __add__(self,other):
        return self.ad + other.ad
    def __mul__(self,other):
        return self.yazar+ '-' +other.yazar
        
kitap1=kitap('Salakhane','Tuna Okulu',21)
kitap2=kitap('Kerizler','Bunyamin Şahan',31)
kitap3=kitap('Armutlar','Fatih Çelik',445)
kitap4=kitap.stringİleOluştur('Saplayıcılar M.EnesOnuş')
 

print(kitap1*kitap3)

# =============GÜN5==============

## Iterator

__iter__
__next__

lise=[3,5,7,2,8]

iterator=iter(lise)

next(iterator)
next(iterator)
next(iterator)
next(iterator)
next(iterator)
next(iterator)

### For While ve Iterator ilişkisi

liste=[12,123,6546,34,87]
for i in liste:
    print(i)

print('=====')

iterator1=iter(liste)

while True:
    try:
        i = next(iterator1)
        print(i)
    except StopIteration:
        break
    

### Kendi class'ımızda kullanabilmek

class raftakiKitaplar():
    def __init__(self,kitaplar,raflar):
        self.kitaplar = kitaplar
        self.raflar = raflar
        self.index=-1
        
    def __iter__(self):
        return self
    def __next__(self):
        self.index += 1
        if(self.index < len(self.kitaplar)):
            return self.kitaplar [self.index]
        else:
            self.index = -1
            raise StopIteration

kitaplar1=raftakiKitaplar(['Salakhane','Armutlar','Kerizler'],'F16')

for i in kitaplar1:
    print(i)

## Generator

#for i in range(2,14,4):
#    print(i)

#print(range(2,5))

def üsAl():
    cevap=[]
    for i in range(1,13):
        cevap.append(i**4)
    return cevap
print(üsAl())


def üsAl():
    for i in range(1,13):
        yield i**4

generator=üsAl()
iterator=iter(generator)
print (next(generator))
print (next(generator))
print (next(generator))
print (next(generator))

## Decorator

### İç içe fonksiyon

def fonksiyon1()


def fonksiyon(islem):
    def topla(*args):
        sonuc = 0
        for i in args:
            sonuc += i
        return sonuc
    def carp(*args):
        sonuc = 1
        for i in args:
            sonuc *= i
        return sonuc
    
    if islem == "toplama":
        return topla
    else:
        return carp

ornek = fonksiyon("tssoplama")
ornek(2,3,4,1,4)

ornek = fonksiyon("toplama")
ornek(2,3,4,1,4)

#Decoratorlar Nasıl oluşturulur

def decorator(fonk):
    def wrapper():
        print('fonksiyon çalışmadan önce')
        fonk()
        print('fonksiyon çalıştıktan sonra')
    return wrapper

def fonksiyon():
    print('fonksiyon çalışıyor')
    
fonksiyon1=decorator(fonksiyon)
fonksiyon1()

def decorator(fonk):
    def wrapper():
        print('fonksiyon çalışmadan önce')
        fonk()
        print('fonksiyon çalıştıktan sonra')
    return wrapper
@decorator


def fonksiyon():
    print('fonksiyon çalışıyor')
    
fonksiyon()

import time

def zamanHesapla(fonk):
    def wrapper(*args,**kwargs):
        baslangic = time.time()
        fonk(*args,**kwargs)
        bitis = time.time()
        print(f'İşlem {bitis-baslangic} saniye sürdü')
    return wrapper
    
@zamanHesapla
def kareleriAl(liste):
    for i in liste:
        print(i**2)
        
@zamanHesapla
def küpünüAl(liste):
    for i in liste:
        print(i**3)
        
@zamanHesapla
def topla(a,b):
    print(a+b)

    
    
kareleriAl(range(4,6))

## Class Örneği

import time

class araba():
    galeriAdı = "Tekinler Galeri"
    aracSayısı = 0
    aracID = 2152
    def __init__(self,marka="Girilmedi",model="Girilmedi",yıl="Girilmedi",renk="Girilmedi"):
        self.marka = marka
        self.model = model
        self.yıl = yıl
        self.renk = renk
        araba.aracSayısı += 1
        araba.aracID += 5
        self.aracID = araba.aracID
        self.index = -1
        
    def zamanHesapla(fonk):
        def wrapper(*args,**kwargs):
            baslangic = time.time()
            fonk(*args,*kwargs)
            bitis = time.time()
            print("Bu işlem toplam {} saniye sürdü".format(bitis-baslangic))
        return wrapper
     
    @zamanHesapla    
    def renkDegistir(self,yeniRenk):
        self.renk = yeniRenk
        
    def __str__(self):
        return f"Arabanın markası: {self.marka}\nArabanın modeli: {self.model}\nArabanın yılı: {self.yıl}\nArabanın rengi: {self.renk}"
    
    def __len__(self):
        return self.yıl
    
    @zamanHesapla 
    def __add__(self,other):
        return self.yıl + other.yıl
    
    def __iter__(self):
        return self
    
    def __next__(self):
        self.index += 1
        if self.index < len(self.marka):
            return self.marka[self.index]
        else:
            self.index = -1
            raise StopIteration
            
    def ornekGenerator(self):
        for i in range(1,self.yıl):
            yield 2*i
            
    @classmethod
    def aracSayısınıSoyle(cls):
        return cls.aracSayısı
    
    @staticmethod
    def galeriAdınıSoyle():
        return araba.galeriAdı

arac1 = araba("Renault","Megane",2015,"Beyaz")
arac2 = araba("Fiat","Linea",2017,"Kırmızı")

#print(arac1)
#len(arac1)
araba.galeriAdı
araba.aracSayısı
arac1.aracID
arac2.aracID
arac1.renkDegistir("Siyah")
#print(arac1)

arac1 + arac2


for i in arac1:
    print(i)
print("-------")
    
iterator = iter(arac2)    
while True:
    try:
        i = next(iterator)
        print(i)
    except StopIteration:
        break

araba.aracSayısınıSoyle()
araba.galeriAdınıSoyle()

generator = arac1.ornekGenerator()
iterator = iter(generator)
next(iterator)
next(iterator)
next(iterator)
next(iterator)
next(iterator)

# ==============GÜN6===============


