# Dosya İşlemleri ve Hata Yönetimi
## Dosya İşlemlerinde Hata Yakalama
Dosya işlemleri sırasında çeşitli hatalarla karşılaşabilirsiniz. Örneğin:

* Dosya mevcut değilse, okuma işlemi hata verebilir.
* Dosyaya yazma izniniz yoksa, yazma işlemi hata verebilir.

Bu tür hataları yönetmek ve programınızın çökmesini engellemek için try-except bloklarını kullanabiliriz.

### Try-Except Blokları
Python'da hata yakalama ve yönetme işlemi try-except blokları ile yapılır. Temel yapı şu şekildedir:

````
try:
    # Hata alması muhtemel kodlar buraya yazılır
    ...
except ExceptionType as e:
    # Hata durumunda yapılacak işlemler buraya yazılır
    ...
````
### Dosya Okuma ve Hata Yönetimi
Dosya okuma sırasında karşılaşılabilecek hataları yönetmek için try-except bloklarını kullanabiliriz. Örnek:

````
try:
    dosya = open("mevcut_olmayan_dosya.txt", "r")
    icerik = dosya.read()
    print(icerik)
    dosya.close()
except FileNotFoundError as e:
    print("Hata: Dosya bulunamadı.")
    print(e)
except Exception as e:
    print("Beklenmeyen bir hata oluştu.")
    print(e)
````

### Dosya Yazma ve Hata Yönetimi
Dosya yazma sırasında karşılaşılabilecek hataları yönetmek için try-except bloklarını kullanabiliriz. Örnek:

````
try:
    dosya = open("korumali_dosya.txt", "w")
    dosya.write("Bu dosyaya yazma iznim yok.\n")
    dosya.close()
except PermissionError as e:
    print("Hata: Dosyaya yazma izniniz yok.")
    print(e)
except Exception as e:
    print("Beklenmeyen bir hata oluştu.")
    print(e)
````

### with İfadesi ve Hata Yönetimi
with ifadesi kullanırken de hata yönetimi yapabiliriz. Örnek:

````
try:
    with open("mevcut_olmayan_dosya.txt", "r") as dosya:
        icerik = dosya.read()
        print(icerik)
except FileNotFoundError as e:
    print("Hata: Dosya bulunamadı.")
    print(e)
except Exception as e:
    print("Beklenmeyen bir hata oluştu.")
    print(e)
````

### Hata Türleri
Dosya işlemlerinde sıkça karşılaşılabilecek hata türleri şunlardır:

* FileNotFoundError: Dosya bulunamadığında ortaya çıkar.
* PermissionError: Dosyaya erişim izni olmadığında ortaya çıkar.
* IOError: Giriş/Çıkış işlemleri sırasında genel hatalar için kullanılır.

### Özet
Bu derste dosya işlemlerinde hata yakalama ve yönetme işlemlerini öğrendik. 'try-except' blokları ile dosya okuma ve yazma sırasında karşılaşılabilecek hataları nasıl yöneteceğimizi gördük. Ayrıca, 'with' ifadesi ile hata yönetimini inceledik.

