# String Manipülasyonları
Stringler, Python'da metin verilerini temsil eden veri tipleridir. String manipülasyonları, stringler üzerinde çeşitli işlemler yapmanıza olanak tanır. Bu derste, Python'da string manipülasyonları için kullanılan bazı temel yöntemleri öğreneceksiniz.

#### String Tanımlama
Python'da stringler, tek tırnak (') veya çift tırnak (") kullanılarak tanımlanabilir.

````
tek_tirnakli_string = 'Merhaba, Dünya!'
cift_tirnakli_string = "Merhaba, Dünya!"
````
#### String Birleştirme (Concatenation)
İki veya daha fazla stringi birleştirmek için + operatörünü kullanabilirsiniz.

````
isim = "Ahmet"
soyisim = "Yılmaz"
tam_isim = isim + " " + soyisim
print(tam_isim)  # Çıktı: Ahmet Yılmaz
````

#### String Tekrarlama (Repetition)
Bir stringi belirli bir sayı kadar tekrarlamak için * operatörünü kullanabilirsiniz.

````
merhaba = "Merhaba! "
tekrar = merhaba * 3
print(tekrar)  # Çıktı: Merhaba! Merhaba! Merhaba! 
````

#### String Uzunluğu (Length)
Bir stringin uzunluğunu bulmak için len() fonksiyonunu kullanabilirsiniz.

````
mesaj = "Merhaba, Dünya!"
uzunluk = len(mesaj)
print(uzunluk)  # Çıktı: 15
````

#### String İçinde Karakterlere Erişim
Stringlerde belirli bir karaktere indeksleme kullanarak erişebilirsiniz. İndeksler sıfırdan başlar.

````
mesaj = "Merhaba"
ilk_karakter = mesaj[0]
son_karakter = mesaj[-1]
print(ilk_karakter)  # Çıktı: M
print(son_karakter)  # Çıktı: a
````


#### String Dilimleme (Slicing)
Stringin belirli bir bölümünü almak için dilimleme kullanabilirsiniz. Dilimleme, [başlangıç:bitiş] şeklinde yapılır.

````
mesaj = "Merhaba, Dünya!"
ilk_kelime = mesaj[:7]
ikinci_kelime = mesaj[9:]
print(ilk_kelime)  # Çıktı: Merhaba
print(ikinci_kelime)  # Çıktı: Dünya!
````

### String Metodları
Python'da stringler üzerinde çalışmak için birçok yerleşik metod vardır. İşte bazı yaygın olarak kullanılan string metodları:

#### 'upper()'
Bir stringi büyük harfe dönüştürür.

````
mesaj = "Merhaba, Dünya!"
buyuk_harf = mesaj.upper()
print(buyuk_harf)  # Çıktı: MERHABA, DÜNYA!
````

#### 'lower()'
Bir stringi küçük harfe dönüştürür.

````
mesaj = "Merhaba, Dünya!"
kucuk_harf = mesaj.lower()
print(kucuk_harf)  # Çıktı: merhaba, dünya!
````

#### 'strip()'
Bir stringin başındaki ve sonundaki boşlukları kaldırır.

````
mesaj = "   Merhaba, Dünya!   "
temiz_mesaj = mesaj.strip()
print(temiz_mesaj)  # Çıktı: Merhaba, Dünya!
````

#### 'replace()'
Bir string içindeki belirli bir alt stringi başka bir alt string ile değiştirir.

````
mesaj = "Merhaba, Dünya!"
yeni_mesaj = mesaj.replace("Dünya", "Python")
print(yeni_mesaj)  # Çıktı: Merhaba, Python!
````

#### 'split()'
Bir stringi belirli bir ayırıcıya göre böler ve bir liste döner.

````
mesaj = "Merhaba, Dünya!"
kelimeler = mesaj.split(", ")
print(kelimeler)  # Çıktı: ['Merhaba', 'Dünya!']
````

#### 'join()'
Bir listeyi belirli bir ayırıcı kullanarak bir stringe dönüştürür.

````
kelimeler = ['Merhaba', 'Dünya!']
birlesik_mesaj = ", ".join(kelimeler)
print(birlesik_mesaj)  # Çıktı: Merhaba, Dünya!
````

### Özet
Bu derste, Python'da stringlerle nasıl çalışılacağını ve string manipülasyonları için kullanılan temel yöntemleri öğrendik. Bu yöntemler, metin verileriyle çalışırken size büyük kolaylık sağlayacaktır.

### Egzersizler
* isim ve soyisim adında iki string değişken oluşturun ve bu değişkenleri birleştirerek tam adınızı ekrana yazdırın.    
* Bir string oluşturun ve bu stringin uzunluğunu ekrana yazdırın.    
* Bir string oluşturun ve bu stringin ilk ve son karakterini ekrana yazdırın.    
* Bir string oluşturun ve bu stringin belirli bir bölümünü dilimleyerek ekrana yazdırın.    
* Bir string oluşturun ve bu stringi büyük harfe, küçük harfe dönüştürerek ekrana yazdırın.    
* Bir string oluşturun ve bu stringin içindeki belirli bir alt stringi başka bir alt string ile değiştirerek ekrana yazdırın.    
* Bir string oluşturun ve bu stringi belirli bir ayırıcıya göre bölerek bir listeye dönüştürün ve bu listeyi ekrana yazdırın.    
* Bir liste oluşturun ve bu listeyi belirli bir ayırıcı kullanarak bir stringe dönüştürün ve bu stringi ekrana yazdırın.
  
Bu ders, Python'da string manipülasyonlarını anlamanıza ve kullanmanıza yardımcı olacaktır. Bu beceriler, metin verileriyle çalışırken size büyük kolaylık sağlayacaktır.    























