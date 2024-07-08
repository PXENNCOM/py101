
# Python Temel Sözdizimi

Bu belge, Python programlama dilinin temel sözdizimini açıklamak için tasarlanmıştır.

## Değişkenler ve Veri Türleri

Python'da değişkenler tanımlandığında veri türü belirtilmez. Bazı temel veri tipleri şunlardır:

### Tamsayılar (integers)

```python
x = 5
y = -10
````
###  Noktalı Sayılar (floats)

````
pi = 3.14
rate = 1.5
````
### Karakter Dizileri (strings)

````
name = "Ahmet"
message = 'Merhaba, dünya!'
````
Python, dinamik tür atamaya sahiptir, bu nedenle bir değişkenin türü otomatik olarak belirlenir.

### Koşullu İfadeler

Koşullu ifadeler, belirli koşullara göre kararlar vermek için kullanılır:

 ````
a = 10
b = 5

if a > b:
    print("a, b'den büyüktür.")
elif a == b:
    print("a, b'ye eşittir.")
else:
    print("a, b'den küçüktür.")
````

### Döngüler
#### for Döngüsü
for döngüsü, bir liste veya başka bir veri yapısı üzerinde iterasyon yapmak için kullanılır:

````
numbers = [1, 2, 3, 4, 5]

for num in numbers:
    print(num)

````
#### while Döngüsü
while döngüsü, belirli bir koşul sağlandığı sürece tekrarlanır:

````
count = 0
while count < 5:
    print(count)
    count += 1

````

### Fonksiyonlar
Fonksiyonlar, belirli bir işlevi yerine getirmek için kullanılır:

````
def greet(name):
    print("Merhaba,", name)

greet("Ahmet")

````

### Listeler
Listeler, virgülle ayrılmış öğelerin köşeli parantez içinde tanımlanmasıyla oluşturulur:

````
colors = ["kırmızı", "yeşil", "mavi"]

````






