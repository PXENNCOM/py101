# Sınıf Tanımlama ve Nesne Oluşturma
Nesne Yönelimli Programlama (OOP), yazılım geliştirme sürecinde kullanılan güçlü bir paradigmadır. Bu paradigmada, veri ve bu veriye uygulanacak işlemler bir arada tutulur. Bu yapı, sınıflar ve nesneler kullanılarak oluşturulur.

## Sınıf Tanımlama
Sınıf, bir nesnenin özelliklerini ve davranışlarını tanımlayan bir şablondur. Sınıf tanımlamak için 'class' anahtar kelimesi kullanılır.
````
class Araba:
    marka = ""
    model = ""
    yil = 0

    def bilgileri_goster(self):
        print(f"Marka: {self.marka}, Model: {self.model}, Yıl: {self.yil}")
````

Bu örnekte, Araba adında bir sınıf tanımladık. Bu sınıfın 'marka', 'model' ve 'yil' adında üç özelliği (değişkeni) ve 'bilgileri_goster' adında bir metodu var.

### Nesne Oluşturma
Bir sınıftan nesne oluşturmak için sınıfın adını ve ardından parantezleri kullanırız.

````
# Araba sınıfından bir nesne oluşturma
araba1 = Araba()
araba1.marka = "Toyota"
araba1.model = "Corolla"
araba1.yil = 2020

araba1.bilgileri_goster()
````
Bu örnekte, Araba sınıfından araba1 adında bir nesne oluşturduk ve bu nesnenin özelliklerine değer atadık. Son olarak, bilgileri_goster metodunu çağırarak nesnenin bilgilerini ekrana yazdırdık.

### Yapıcı (Constructor) ve Metodlar

### Yapıcı (Constructor)
Yapıcı, bir sınıftan nesne oluşturulduğunda otomatik olarak çağrılan özel bir metottur. Python'da yapıcı metot '__init__' olarak adlandırılır.

````
class Araba:
    def __init__(self, marka, model, yil):
        self.marka = marka
        self.model = model
        self.yil = yil

    def bilgileri_goster(self):
        print(f"Marka: {self.marka}, Model: {self.model}, Yıl: {self.yil}")
````
Bu örnekte, Araba sınıfına bir yapıcı ekledik. Bu yapıcı, marka, model ve yil parametrelerini alır ve bunları sınıfın özelliklerine atar.

### Metodlar
Metodlar, bir sınıfın davranışlarını tanımlayan fonksiyonlardır. Sınıfın içindeki tüm metodlar, ilk parametre olarak self alır. Bu parametre, metodun hangi nesne üzerinde çalıştığını belirtir.

````
class Araba:
    def __init__(self, marka, model, yil):
        self.marka = marka
        self.model = model
        self.yil = yil

    def bilgileri_goster(self):
        print(f"Marka: {self.marka}, Model: {self.model}, Yıl: {self.yil}")

    def yas_hesapla(self, mevcut_yil):
        return mevcut_yil - self.yil

# Araba sınıfından bir nesne oluşturma
araba1 = Araba("Toyota", "Corolla", 2020)

araba1.bilgileri_goster()
print(f"Araba yaşı: {araba1.yas_hesapla(2024)}")
````

Bu örnekte, 'Araba' sınıfına 'yas_hesapla' adında bir metod ekledik. Bu metod, arabanın yaşını hesaplar ve geri döner.


#### Özet
Bu derste Nesne Yönelimli Programlama (OOP) kavramlarını, sınıf tanımlamayı, nesne oluşturmayı, yapıcı (constructor) metodunu ve sınıf metodlarını öğrendik. OOP, daha organize ve yönetilebilir kod yazmamıza yardımcı olur.






