# Döngüler ve Kontrol İfadeleri (break, continue)
Python'da döngüler, belirli bir işlemi tekrarlamak için kullanılır. for ve while döngüleri en yaygın kullanılan döngü türleridir. Bu derste, bu döngülerin nasıl kullanılacağını ve döngüler içinde kullanılan break ve continue ifadelerinin ne işe yaradığını öğreneceksiniz.

## for Döngüsü
for döngüsü, bir dizi veya iterable üzerindeki her öğe için belirtilen işlemi tekrarlar.

````
for sayi in range(1, 6):
    print(sayi)
````
##### çıktı
````
1
2
3
4
5
````

## while Döngüsü
while döngüsü, belirli bir koşul doğru olduğu sürece belirtilen işlemi tekrarlar.

````
sayi = 1
while sayi <= 5:
    print(sayi)
    sayi += 1
````
çıktı
````
1
2
3
4
5
````

### break İfadesi
break ifadesi, döngüyü aniden sonlandırır ve döngü bloğundan çıkar.

````
for sayi in range(1, 10):
    if sayi == 5:
        break
    print(sayi)
````
çıktı
````
1
2
3
4
````

### continue İfadesi
continue ifadesi, döngünün geri kalanını atlayarak döngünün başına döner.

````
for sayi in range(1, 6):
    if sayi == 3:
        continue
    print(sayi)
````

çıktı
````
1
2
4
5
````

## Özet
Bu derste, Python'da for ve while döngülerini nasıl kullanacağınızı, break ve continue ifadelerini nasıl kullanarak döngülerin akışını kontrol edebileceğinizi öğrendik. Döngüler, belirli işlemleri tekrarlamak ve programınızın dinamikliğini artırmak için çok güçlü araçlardır.

### Egzersizler
* 1'den 10'a kadar olan sayıları ekrana yazdıran bir for döngüsü yazın.
* Kullanıcıdan bir sayı girişi alın ve bu sayıya kadar olan sayıları ekrana yazdıran bir while döngüsü yazın.
* Bir liste oluşturun ve bu listenin elemanlarını tek tek ekrana yazdıran bir for döngüsü yazın.
