# Kalıtım ve Polimorfizm
### Kalıtım Yapıları
Kalıtım (inheritance), nesne yönelimli programlamada bir sınıfın başka bir sınıftan özellik ve davranışları devralmasını sağlayan bir mekanizmadır. Kalıtım, kod tekrarını azaltır ve daha esnek ve yeniden kullanılabilir kod yazmamıza olanak tanır.

### Temel Sınıf (Base Class) ve Türemiş Sınıf (Derived Class)
Bir sınıf, başka bir sınıftan kalıtım aldığında, kalıtım alınan sınıf "temel sınıf" (base class) olarak adlandırılır. Kalıtım alan sınıf ise "türemiş sınıf" (derived class) olarak adlandırılır.

````
# Temel Sınıf
class Hayvan:
    def __init__(self, isim):
        self.isim = isim

    def ses_cikar(self):
        pass

# Türemiş Sınıf
class Kopek(Hayvan):
    def ses_cikar(self):
        return "Hav Hav!"

# Türemiş Sınıf
class Kedi(Hayvan):
    def ses_cikar(self):
        return "Miyav Miyav!"
````
Bu örnekte, 'Hayvan' adında bir temel sınıf tanımladık. 'Kopek' ve 'Kedi' sınıfları, Hayvan sınıfından kalıtım alır ve 'ses_cikar' metodunu kendilerine özgü şekilde yeniden tanımlar.

### Kalıtımın Kullanımı
Bir sınıftan kalıtım almak için türemiş sınıfın tanımında temel sınıfı parantez içinde belirtiriz.

````
# Nesneler oluşturma
kopek = Kopek("Karabaş")
kedi = Kedi("Minnak")

print(f"{kopek.isim}: {kopek.ses_cikar()}")
print(f"{kedi.isim}: {kedi.ses_cikar()}")
````
Bu örnekte, 'Kopek' ve 'Kedi' sınıflarından nesneler oluşturduk ve bu nesnelerin ses_cikar metodunu çağırdık.

### Polimorfizm ve Metod Overriding
#### Polimorfizm
Polimorfizm, nesne yönelimli programlamada aynı işlemi farklı nesneler üzerinde gerçekleştirme yeteneğidir. Bu, genellikle türemiş sınıfların temel sınıftan kalıtım aldığı ve metodlarını kendilerine özgü şekilde yeniden tanımladığı durumlarda kullanılır.

````
# Polimorfizm örneği
hayvanlar = [Kopek("Karabaş"), Kedi("Minnak")]

for hayvan in hayvanlar:
    print(f"{hayvan.isim}: {hayvan.ses_cikar()}")
````
Bu örnekte, 'hayvanlar' listesi hem 'Kopek' hem de 'Kedi' nesnelerini içerir. Döngü içinde her hayvanın 'ses_cikar' metodu çağrıldığında, her sınıfın kendi metodunun çalıştığını görürüz.

### Metod Overriding
Metod overriding, türemiş bir sınıfın temel sınıftan kalıtım aldığı bir metodu kendine özgü şekilde yeniden tanımlamasıdır.

````
# Temel Sınıf
class Hayvan:
    def __init__(self, isim):
        self.isim = isim

    def ses_cikar(self):
        return "Bilinmeyen Ses"

# Türemiş Sınıf
class Kopek(Hayvan):
    def ses_cikar(self):
        return "Hav Hav!"

# Türemiş Sınıf
class Kedi(Hayvan):
    def ses_cikar(self):
        return "Miyav Miyav!"
````
Bu örnekte, 'Kopek' ve 'Kedi' sınıfları, Hayvan sınıfının 'ses_cikar' metodunu kendilerine özgü şekilde yeniden tanımlar.


#### Özet
Bu derste, kalıtım ve polimorfizm kavramlarını öğrendik. Kalıtım, bir sınıfın başka bir sınıftan özellik ve davranışları devralmasını sağlar. Polimorfizm, aynı işlemi farklı nesneler üzerinde gerçekleştirme yeteneğidir. Ayrıca, metod overriding ile türemiş sınıfların temel sınıftan kalıtım aldığı metodları kendilerine özgü şekilde yeniden tanımladığını gördük.





