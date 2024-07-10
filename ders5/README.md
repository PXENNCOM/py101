
# Basit Matematiksel İşlemler
Python, temel matematiksel işlemleri yapabilmek için çeşitli operatörler sağlar. Bu derste, Python'da nasıl matematiksel işlemler yapacağınızı öğreneceksiniz. Toplama, çıkarma, çarpma, bölme gibi işlemler ve bazı ileri düzey matematiksel fonksiyonlar hakkında bilgi sahibi olacaksınız.

### Temel Matematiksel Operatörler
#### 1. Toplama (+)
Toplama operatörü, iki veya daha fazla sayıyı toplar.

````
a = 5
b = 3
sonuc = a + b
print("Toplama: ", sonuc)  # Çıktı: 8
````

#### 2. Çıkarma (-)
Çıkarma operatörü, bir sayıyı diğerinden çıkarır.
````
a = 5
b = 3
sonuc = a - b
print("Çıkarma: ", sonuc)  # Çıktı: 2
````
#### 3. Çarpma (*)
Çarpma operatörü, iki sayıyı çarpar.
````
a = 5
b = 3
sonuc = a * b
print("Çarpma: ", sonuc)  # Çıktı: 15
````

#### 4. Bölme (/)
Bölme operatörü, bir sayıyı diğerine böler. Sonuç her zaman ondalıklı (float) bir sayı olur.

````
a = 5
b = 3
sonuc = a / b
print("Bölme: ", sonuc)  # Çıktı: 1.6666666666666667
````

#### 5. Tam Sayı Bölme (//)
Tam sayı bölme operatörü, bir sayıyı diğerine böler ve sonucu aşağı yuvarlanmış bir tam sayı olarak döner.

````
a = 5
b = 3
sonuc = a // b
print("Tam Sayı Bölme: ", sonuc)  # Çıktı: 1
````

#### 6. Modülüs (%)
Modülüs operatörü, bir sayıyı diğerine böler ve kalanını döner.

````
a = 5
b = 3
sonuc = a % b
print("Modülüs: ", sonuc)  # Çıktı: 2
````

#### 7. Üs Alma (**)
Üs alma operatörü, bir sayının diğerine üssünü alır.

````
a = 5
b = 3
sonuc = a ** b
print("Üs Alma: ", sonuc)  # Çıktı: 125
````


## Matematiksel Fonksiyonlar
Python, daha ileri düzey matematiksel işlemler için math modülünü sağlar. Bu modülde birçok hazır fonksiyon bulunmaktadır.

### 'math' Modülü
math modülünü kullanmak için öncelikle import etmeniz gerekir:

````
import math
````

#### 1. Kare Kök (math.sqrt)
Bir sayının karekökünü alır.

````
import math

a = 16
sonuc = math.sqrt(a)
print("Karekök: ", sonuc)  # Çıktı: 4.0
````

#### 2. Mutlak Değer (math.fabs)
Bir sayının mutlak değerini alır.

````
import math

a = -5
sonuc = math.fabs(a)
print("Mutlak Değer: ", sonuc)  # Çıktı: 5.0
````

#### 3. Faktöriyel (math.factorial)
Bir sayının faktöriyelini alır.

````
import math

a = 5
sonuc = math.factorial(a)
print("Faktöriyel: ", sonuc)  # Çıktı: 120
````

### Özet
Bu derste, Python'da temel matematiksel işlemleri ve bazı ileri düzey matematiksel fonksiyonları öğrendik. Bu temel bilgileri kavrayarak, daha karmaşık matematiksel hesaplamalar yapabilirsiniz.



#### Egzersizler

1. Aşağıdaki işlemleri Python'da gerçekleştirin ve sonuçlarını ekrana yazdırın:

1: 15 + 7    
2: 20 - 4    
3: 6 * 9    
4: 25 / 5    
5: 17 // 3    
6: 19 % 4    
7: 2 ** 8  

 1.math modülünü kullanarak aşağıdaki işlemleri gerçekleştirin:

1: 64 sayısının karekökünü bulun.    
2: -10 sayısının mutlak değerini bulun.    
3: 7 sayısının faktöriyelini hesaplayın.   


#### Bu ders, Python'da temel ve ileri düzey matematiksel işlemleri anlamanıza yardımcı olacaktır. Bu beceriler, programlama yolculuğunuzda size büyük kolaylık sağlayacaktır.
