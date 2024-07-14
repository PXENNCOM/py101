# Dosya Açma ve Yazma

## Dosya Okuma ve Yazma
Python'da dosya işlemleri yaparken open fonksiyonunu kullanırız. Dosya işlemlerinin temel adımları şunlardır:

* Dosyayı açmak    
* Dosya üzerinde işlem yapmak (okuma, yazma)    
* Dosyayı kapatmak

### Dosya Açma
Bir dosyayı açmak için open fonksiyonunu kullanırız. Bu fonksiyon iki temel parametre alır:

* 'dosya_adi': İşlem yapılacak dosyanın adı.
* 'mod': Dosyanın nasıl açılacağını belirten bir dize (okuma, yazma, ekleme vb.).

### Dosya Modları
Dosya modları, dosyanın nasıl açılacağını belirler:

* 'r': Okuma modu. Dosya mevcut değilse hata verir.
* 'w': Yazma modu. Dosya mevcutsa üzerine yazar, mevcut değilse yeni bir dosya oluşturur.
* 'a': Ekleme modu. Dosya mevcutsa sonuna ekler, mevcut değilse yeni bir dosya oluşturur.

### Dosya Yazma
Dosya yazmak için w veya a modunda dosya açmamız gerekir. Örnek:

````
# 'w' modu ile dosya açma ve yazma
dosya = open("ornek.txt", "w")
dosya.write("Merhaba Dünya!\n")
dosya.write("Bu, dosya yazma örneğidir.\n")
dosya.close()
````
### Dosya Okuma
Dosya okumak için r modunda dosya açmamız gerekir. Örnek:

````
# 'r' modu ile dosya açma ve okuma
dosya = open("ornek.txt", "r")
icerik = dosya.read()
print(icerik)
dosya.close()
````

### Dosya Satır Satır Okuma
Dosya içeriğini satır satır okumak için readline veya readlines fonksiyonlarını kullanabiliriz.

````
# readline ile satır satır okuma
dosya = open("ornek.txt", "r")
satir = dosya.readline()
while satir:
    print(satir, end='')
    satir = dosya.readline()
dosya.close()
````
````
# readlines ile tüm satırları liste olarak okuma
dosya = open("ornek.txt", "r")
satirlar = dosya.readlines()
for satir in satirlar:
    print(satir, end='')
dosya.close()
````

### with İfadesi ile Dosya Açma
Dosya açma ve kapatma işlemlerini daha güvenli ve otomatik hale getirmek için 'with' ifadesini kullanabiliriz. 'with' ifadesi ile dosya otomatik olarak kapatılır.

````
# with ifadesi ile dosya açma ve yazma
with open("ornek.txt", "w") as dosya:
    dosya.write("Bu, with ifadesi ile yazılmıştır.\n")

# with ifadesi ile dosya açma ve okuma
with open("ornek.txt", "r") as dosya:
    icerik = dosya.read()
    print(icerik)
````

#### Özet
Bu dersimizde Python'da dosya açma ve yazma işlemlerini öğrendik. Dosya modları (r, w, a) ile dosya okuma ve yazma işlemlerini nasıl yapacağımızı gördük. Ayrıca, dosya işlemlerinde güvenlik ve kolaylık sağlayan 'with' ifadesini kullandık.



