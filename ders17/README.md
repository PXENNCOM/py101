# Python Modülleri ve Import Kullanımı

### Modüller Nedir?
Python'da bir modül, genellikle belirli bir işlevi yerine getiren bir dizi fonksiyon, sınıf ve değişken içeren bir dosyadır. Modüller, kodunuzu daha düzenli ve yönetilebilir hale getirir, ayrıca kodun tekrar kullanımını kolaylaştırır.

Bir modül, .py uzantılı bir Python dosyasıdır. Örneğin, mymodule.py adlı bir dosyanız olabilir ve bu dosyada çeşitli fonksiyonlar ve değişkenler tanımlayabilirsiniz.

### Modül Oluşturma
Örnek olarak basit bir modül oluşturalım. mymodule.py adlı bir dosya oluşturun ve içine şu kodu yazın:

````
# mymodule.py

def selam_ver(isim):
    return f"Merhaba, {isim}!"

pi = 3.14159
````
Bu modül, bir 'selam_ver' fonksiyonu ve bir pi değişkeni içerir.

### Modül İthal Etme (Import)
Bir modülü kullanmak için 'import' ifadesini kullanırız. Örneğin, 'mymodule.py' modülünü ithal edip içindeki fonksiyonu ve değişkeni kullanabiliriz.

````
# main.py

import mymodule

print(mymodule.selam_ver("Dünya"))
print(f"Pi sayısı: {mymodule.pi}")
````

Bu kod, 'mymodule' modülünü ithal eder ve modül içindeki 'selam_ver 'fonksiyonunu ve 'pi' değişkenini kullanır.

### Modülden Belirli Öğeleri İthal Etme
Bazen bir modülden sadece belirli fonksiyonları veya değişkenleri ithal etmek isteyebilirsiniz. Bu durumda 'from' ifadesini kullanabilirsiniz.

````
# main.py

from mymodule import selam_ver, pi

print(selam_ver("Dünya"))
print(f"Pi sayısı: {pi}")
````
Bu kod, mymodule modülünden 'selam_ver' fonksiyonunu ve 'pi' değişkenini doğrudan ithal eder. Artık 'mymodule.selam_ver' veya 'mymodule.pi' yazmanıza gerek yoktur.

### Modüllere Takma Ad Vermek
Bir modüle takma ad vererek daha kısa veya anlamlı hale getirebilirsiniz. Bu, özellikle uzun modül adları için kullanışlıdır.

````
# main.py

import mymodule as mm

print(mm.selam_ver("Dünya"))
print(f"Pi sayısı: {mm.pi}")
````
Bu kodda, 'mymodule' modülüne 'mm' takma adı verildi ve bu ad kullanılarak modül içindeki öğelere erişildi.

### Standart Kütüphaneler
Python, çok sayıda kullanışlı modül içeren geniş bir standart kütüphaneye sahiptir. Bu modüller, sık kullanılan işlevleri kolayca gerçekleştirmek için tasarlanmıştır. İşte bazı yaygın kullanılan standart kütüphane modülleri:

### 'math' Modülü
math modülü, matematiksel işlevler ve sabitler sağlar.

````
import math

print(math.sqrt(16))  # Karekök hesaplama
print(math.factorial(5))  # Faktöriyel hesaplama
print(math.pi)  # Pi sayısı
````

### 'datetime' Modülü
datetime modülü, tarih ve saatle ilgili işlevler sağlar.

````
import datetime

simdi = datetime.datetime.now()
print(simdi)  # Şu anki tarih ve saat

dogum_gunu = datetime.datetime(1990, 5, 17)
print(dogum_gunu)  # Belirli bir tarih

````

### random Modülü
random modülü, rastgele sayı üretmek için kullanılır.

````
import random

print(random.randint(1, 10))  # 1 ile 10 arasında rastgele bir tam sayı
print(random.choice(['elma', 'muz', 'çilek']))  # Rastgele bir seçim
````

### 'os' Modülü
os modülü, işletim sistemi ile etkileşim kurmayı sağlar. Dosya ve dizin işlemleri gibi çeşitli işlevler sunar.

````
import os

print(os.getcwd())  # Mevcut çalışma dizinini al
os.mkdir('yeni_dizin')  # Yeni bir dizin oluştur
````

### 'sys' Modülü
sys modülü, Python yorumlayıcısı ile ilgili çeşitli işlevler sağlar.

````
import sys

print(sys.version)  # Python sürümünü al
print(sys.path)  # Modül arama yolunu al
````

#### Özet

Bu derste, Python'da modüller ve ithal etme (import) kavramlarını öğrendik. Modüllerin ne olduğunu, nasıl oluşturulacağını ve ithal edileceğini gördük. Ayrıca, Python'un standart kütüphanelerinden bazılarını inceledik. Standart kütüphaneler, Python'da sıkça ihtiyaç duyulan birçok işlevi kolayca gerçekleştirmemizi sağlar.

















