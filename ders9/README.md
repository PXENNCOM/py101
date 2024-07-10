# Fonksiyonlar ve Kullanımları
Python'da fonksiyonlar, belirli bir işlevi yerine getiren ve kodunuzu modüler hale getiren bloklardır. Bu derste, fonksiyonları nasıl tanımlayacağınızı, çağıracağınızı, parametreleri ve dönüş değerlerini nasıl kullanacağınızı öğreneceksiniz.

### Fonksiyon Tanımlama ve Çağırma
Fonksiyonlar def anahtar kelimesiyle tanımlanır ve return anahtar kelimesiyle bir değer döndürebilirler.

````
def selamla(isim):
    return "Merhaba, " + isim + "!"

print(selamla("Ahmet"))
````

Çıktı:
````
Merhaba, Ahmet!
````

### Parametreler
Fonksiyonlara parametreler geçirerek, fonksiyon içinde bu parametreleri kullanabilirsiniz.

````
def toplama(a, b):
    return a + b

print(toplama(3, 5))  # Çıktı: 8
````

### Dönüş Değeri
Fonksiyonlar return ifadesiyle bir veya birden fazla değer döndürebilir.

````
def kare_al(sayi):
    return sayi ** 2

sonuc = kare_al(4)
print(sonuc)  # Çıktı: 16
````
# Varsayılan Parametreler
Fonksiyonlara varsayılan parametreler atayarak, fonksiyon çağrılarında bu parametrelerin zorunlu olmadığını belirleyebilirsiniz.

````def selamla(isim="Dünya"):
    return "Merhaba, " + isim + "!"

print(selamla())  # Çıktı: Merhaba, Dünya!
print(selamla("Ahmet"))  # Çıktı: Merhaba, Ahmet!
````

## Özet
Bu derste, Python'da fonksiyonların nasıl tanımlandığını, çağrıldığını, parametrelerin nasıl kullanıldığını ve dönüş değerlerinin nasıl alındığını öğrendik. Fonksiyonlar, kodunuzu modüler hale getirmenizi ve tekrar kullanılabilir parçalar oluşturmanızı sağlar.

### Egzersizler

* Bir fonksiyon oluşturun ve bu fonksiyonla bir liste içindeki en büyük sayıyı bulun.
* İki sayı alan ve bu sayıların aritmetik ortalamasını döndüren bir fonksiyon yazın.
* Bir string alan ve bu string'in ters çevrilmiş halini döndüren bir fonksiyon yazın.

  Bu ders, Python'da fonksiyonları anlamanıza ve kullanmanıza yardımcı olacaktır. Bu beceriler, daha karmaşık programlar yazmanıza ve kodunuzu daha organize hale getirmenize olanak tanır.


















