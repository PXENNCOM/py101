# Lambda Fonksiyonları ve Scope
Lambda fonksiyonları, kısa ve anonim fonksiyonlar olarak tanımlanır ve genellikle tek seferlik kullanımlar için idealdir. Scope (kapsam), bir değişkenin erişilebilir olduğu alanı belirtir. Bu derste, lambda fonksiyonlarını ve değişken kapsamını öğreneceksiniz.

### Lambda Fonksiyonları
Lambda fonksiyonları lambda anahtar kelimesiyle tanımlanır ve genellikle tek bir ifade içinde yazılır.

````
kare = lambda x: x ** 2
print(kare(5))  # Çıktı: 25
````

## Yerel ve Global Değişkenler

### Yerel Değişkenler
Yerel değişkenler, bir fonksiyon içinde tanımlanan ve sadece o fonksiyon içinde erişilebilen değişkenlerdir.

````
def fonksiyon():
    yerel_degisken = "Bu bir yerel değişkendir."
    print(yerel_degisken)

fonksiyon()
print(yerel_degisken)  # Hata verir: NameError: name 'yerel_degisken' is not defined
````

### Global Değişkenler
Global değişkenler, programın her yerinden erişilebilen ve tanımlanan değişkenlerdir.

````
global_degisken = "Bu bir global değişkendir."

def fonksiyon():
    print(global_degisken)

fonksiyon()
print(global_degisken)
````

### Scope Kavramı
Scope, bir değişkenin erişilebilir olduğu alanı ifade eder. Python'da genellikle yerel ve global olmak üzere iki temel kapsam vardır.

````
global_degisken = "Bu bir global değişkendir."

def fonksiyon():
    yerel_degisken = "Bu bir yerel değişkendir."
    print(global_degisken)  # Global değişkene erişim
    print(yerel_degisken)   # Yerel değişkene erişim

fonksiyon()
print(global_degisken)      # Global değişkene erişim
print(yerel_degisken)       # Hata verir: NameError: name 'yerel_degisken' is not defined
````

## Özet
Bu derste, lambda fonksiyonlarını nasıl tanımlayacağınızı ve kullanacağınızı, ayrıca Python'da değişken kapsamını (scope) nasıl yöneteceğinizi öğrendik. Lambda fonksiyonları, kısa ve tek seferlik kullanımlar için uygundur, değişken kapsamı ise bir programın yapısını organize etmenize ve değişken erişimini kontrol etmenize olanak tanır.

### Egzersizler

* Bir lambda fonksiyonu kullanarak bir sayının karesini hesaplayın.
* Bir fonksiyon içinde bir yerel değişken tanımlayın ve bu fonksiyonun dışında bu değişkene erişmeye çalışın. Sonucu gözlemleyin.
* Bir global değişken tanımlayın ve bu değişkene bir fonksiyon içinde erişin. Daha sonra aynı global değişkene bir başka fonksiyondan erişin ve sonucu gözlemleyin.

Lambda fonksiyonları ve değişken kapsamı hakkında daha fazla bilgi edinmek için bu dersten yararlanabilirsiniz. Bu konular, Python programlama becerilerinizi geliştirmenize yardımcı olacaktır.







