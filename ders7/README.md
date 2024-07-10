# Koşullu İfadeler (if, elif, else)
Python'da koşullu ifadeler, belirli bir koşulun doğru veya yanlış olmasına bağlı olarak farklı kod bloklarını çalıştırmanızı sağlar. Bu derste, if, elif ve else yapılarını kullanarak nasıl koşullu ifadeler oluşturabileceğinizi öğreneceksiniz.

### if Yapısı
if yapısı, belirli bir koşulun doğru olması durumunda bir kod bloğunu çalıştırır.

````
sayi = 10

if sayi > 5:
    print("Sayı 5'ten büyüktür.")  # Bu blok çalışır
````

### else Yapısı
else yapısı, if koşulu yanlış olduğunda bir kod bloğunu çalıştırır.

````
sayi = 3

if sayi > 5:
    print("Sayı 5'ten büyüktür.")
else:
    print("Sayı 5'ten küçük veya eşittir.")  # Bu blok çalışır

````

### elif Yapısı
elif yapısı, birden fazla koşulun kontrol edilmesini sağlar. elif, "else if" anlamına gelir ve if ve else yapılarının arasında kullanılır.

````
sayi = 5

if sayi > 5:
    print("Sayı 5'ten büyüktür.")
elif sayi == 5:
    print("Sayı 5'e eşittir.")  # Bu blok çalışır
else:
    print("Sayı 5'ten küçüktür.")
````

### Birden Fazla Koşul
Birden fazla koşulu kontrol etmek için and, or ve not gibi mantıksal operatörleri kullanabilirsiniz.

````
sayi = 7

if sayi > 5 and sayi < 10:
    print("Sayı 5 ile 10 arasında.")  # Bu blok çalışır
````


### İç İçe if Yapıları
Bir if yapısı içinde başka bir if yapısı kullanarak daha karmaşık koşullar oluşturabilirsiniz.

````
sayi = 8

if sayi > 5:
    if sayi < 10:
        print("Sayı 5 ile 10 arasında.")  # Bu blok çalışır
    else:
        print("Sayı 10 veya daha büyük.")
else:
    print("Sayı 5 veya daha küçük.")
````

### Özet
Bu derste, Python'da if, elif ve else yapılarını kullanarak koşullu ifadeler oluşturmayı öğrendik. Bu yapılar, programlarınızda karar verme mekanizmaları oluşturmanıza olanak tanır.

### Egzersizler

* Bir sayı alın ve bu sayının pozitif, negatif veya sıfır olduğunu belirleyin ve ekrana yazdırın.
* Bir öğrencinin notunu alın ve bu nota göre harf notu (A, B, C, D, F) belirleyin.
  
    * 90 ve üzeri: A
    * 80-89: B
    * 70-79: C
    * 60-69: D
    * 60'ın altı: F
 
Bu ders, Python'da koşullu ifadeleri anlamanıza ve kullanmanıza yardımcı olacaktır. Bu beceriler, programlama yolculuğunuzda önemli bir rol oynayacaktır.







 





