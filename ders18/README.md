# Kendi Modüllerimizi Yazma

## Modül Oluşturma
### Modül Nedir?
Modül, belirli bir işlevi yerine getiren bir dizi fonksiyon, sınıf ve değişken içeren bir Python dosyasıdır. Modüller, kodunuzu daha düzenli ve yönetilebilir hale getirir ve kodun tekrar kullanımını kolaylaştırır.

### Modül Oluşturma
Bir modül oluşturmak için yapmanız gereken tek şey, bir Python dosyası (.py uzantılı) oluşturmak ve içine fonksiyonlar, sınıflar ve değişkenler tanımlamaktır.

### Örnek:
mymodule.py adlı bir dosya oluşturun ve içine şu kodu yazın:

````
# mymodule.py

def selam_ver(isim):
    return f"Merhaba, {isim}!"

pi = 3.14159

class Hesaplayici:
    def kare(self, sayi):
        return sayi * sayi
````
Bu modül, bir 'selam_ver' fonksiyonu, bir 'pi' değişkeni ve bir Hesaplayici sınıfı içerir.

### Modülü Kullanma
Oluşturduğunuz modülü kullanmak için 'import' ifadesini kullanabilirsiniz. Örnek:

````
# main.py

import mymodule

print(mymodule.selam_ver("Dünya"))
print(f"Pi sayısı: {mymodule.pi}")

hesap = mymodule.Hesaplayici()
print(hesap.kare(4))
````
Bu kod, 'mymodule' modülünü ithal eder ve modül içindeki fonksiyonu, değişkeni ve sınıfı kullanır.


### Paket Yapısı
#### Paket Nedir?
Paket, birbiriyle ilişkili modülleri bir arada tutan bir dizindir. Paketler, modüllerinizi organize etmek ve daha büyük projeleri yönetmek için kullanışlıdır.

#### Paket Oluşturma
Bir paket oluşturmak için bir dizin oluşturun ve bu dizinin içine modül dosyalarınızı koyun. Ayrıca, dizin içinde bir '__init__.py' dosyası oluşturmalısınız. Bu dosya, Python'a bu dizinin bir paket olduğunu bildirir.

Örnek dizin yapısı:

````
mypackage/
    __init__.py
    mod1.py
    mod2.py
````

'__init__.py' dosyası boş olabilir veya paketin başlatılmasını sağlayan kodları içerebilir.

#### Paket Kullanma
Paket içindeki modülleri kullanmak için 'from' ve 'import' ifadelerini kullanabilirsiniz.    

Örnek:    
'mod1.py:'    
````
# mod1.py

def fonksiyon1():
    return "Modül 1'den fonksiyon 1"
````

'mod2.py':    
````
# mod2.py

def fonksiyon2():
    return "Modül 2'den fonksiyon 2"
````

'__init__.py':    
````

# __init__.py

from .mod1 import fonksiyon1
from .mod2 import fonksiyon2
````
Bu dizin yapısında, 'mypackage' adlı bir paket oluşturduk ve içine 'mod1.py' ve 'mod2.py' adlı iki modül koyduk. '__init__.py' dosyasında, bu modüllerdeki fonksiyonları ithal ettik.    

Şimdi, bu paketi kullanabiliriz:    

````
# main.py

import mypackage

print(mypackage.fonksiyon1())
print(mypackage.fonksiyon2())
````

Bu kod, mypackage paketini ithal eder ve paketin içindeki fonksiyonları kullanır.

#### Alt Paketler
Paketler ayrıca alt paketler içerebilir. Alt paketler, büyük projeleri daha da küçük parçalara ayırmanıza yardımcı olur.

Örnek alt paket yapısı:

````
mypackage/
    __init__.py
    altpaket/
        __init__.py
        mod3.py
````

'altpaket/mod3.py':
````
# mod3.py

def fonksiyon3():
    return "Alt paketten fonksiyon 3"

````


'altpaket/__init__.py':
````
# __init__.py

from .mod3 import fonksiyon3
````
Bu yapıda, 'mypackage' paketi içinde altpaket adlı bir alt paket oluşturduk.    

Kullanımı:    
````
# main.py

import mypackage.altpaket

print(mypackage.altpaket.fonksiyon3())
````
Bu kod, 'mypackage' içindeki altpaket paketini ithal eder ve alt paketin içindeki fonksiyonu kullanır.

### Özet
Bu derste, Python'da modül oluşturmayı ve kullanmayı, paket yapısını ve '__init__.py' dosyasının önemini öğrendik. Modüller ve paketler, kodunuzu daha düzenli ve yönetilebilir hale getirir, ayrıca kodun tekrar kullanımını kolaylaştırır. Kendi modüllerinizi ve paketlerinizi oluşturarak projelerinizi daha iyi organize edebilirsiniz.


















