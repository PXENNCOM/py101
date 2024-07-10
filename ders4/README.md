# Değişkenler ve Veri Tipleri

Python programlama dilinde, değişkenler ve veri tipleri, kod yazarken sıkça karşılaşacağınız temel kavramlardır. Bu derste, değişkenlerin ne olduğunu, nasıl tanımlandığını ve Python'daki farklı veri tiplerini öğreneceksiniz.

## Değişkenler
### Değişken Nedir?

Değişkenler, programlama dilinde veri depolamak için kullanılan isimlendirilmiş alanlardır. Değişkenler, verileri saklamak ve bu verilere daha sonra erişmek için kullanılır.

### Değişken Tanımlama

Python'da değişken tanımlamak oldukça basittir. Bir değişkene değer atamak için = operatörünü kullanırız.

````
isim = "Ahmet"  # String tipinde bir değişken
yas = 25       # Integer tipinde bir değişken
boy = 1.75     # Float tipinde bir değişken
````
### Değişken İsimlendirme Kuralları

1. Değişken isimleri harfler, sayılar ve alt çizgi (_) içerebilir, ancak sayı ile başlayamaz.
2. Büyük ve küçük harfler farklıdır (isim ve Isim farklı değişkenlerdir).
3. Python'da ayrılmış kelimeler (örneğin, def, if, else) değişken ismi olarak kullanılamaz.

##### Geçersiz Değişken İsimleri:

````
1isim      # Sayı ile başlayamaz
isim@      # Özel karakter içeremez
def        # Python'da ayrılmış bir kelime

````

### Veri Tipleri

Python'da farklı veri tipleri vardır. Temel veri tipleri şunlardır:

### 1. Sayılar (Numbers)

#### a. Tamsayılar (Integers)
Tamsayılar, ondalıklı kısım içermeyen sayılardır.

````
sayi = 10
````
#### b. Ondalıklı Sayılar (Floats)
Ondalıklı sayılar, ondalıklı kısım içeren sayılardır.

````
ondalikli_sayi = 10.5
````
### 2. Metinler (Strings)
Metinler, karakter dizileridir ve genellikle tırnak işaretleri içinde yazılır.

````
isim = "Ahmet"
````
### 3. Mantıksal Değerler (Booleans)
Mantıksal değerler, doğru (True) veya yanlış (False) olabilir.

````
dogru_mu = True
yanlis_mi = False
````

### 4. Listeler (Lists)
Listeler, birden fazla öğeyi tek bir değişkende saklamak için kullanılır. Köşeli parantezler ([]) içinde yazılır.

````
meyveler = ["elma", "muz", "çilek"]
````

### 5. Demetler (Tuples)
Demetler, tıpkı listeler gibi birden fazla öğeyi saklamak için kullanılır ancak demetlerin içeriği değiştirilemez. Parantezler (()) içinde yazılır.

````
renkler = ("kırmızı", "yeşil", "mavi")
````

### 6. Sözlükler (Dictionaries)
Sözlükler, anahtar-değer çiftlerini saklamak için kullanılır. Süslü parantezler ({}) içinde yazılır.

````
ogrenci = {"isim": "Ahmet", "yas": 25, "not": 85}
````

### Özet

Bu derste, değişkenlerin ne olduğunu, nasıl tanımlandığını ve Python'daki temel veri tiplerini öğrendik. Python programlamaya başlarken bu temel kavramları anlamak, ileri düzey konuları öğrenmenize yardımcı olacaktır.


1. Aşağıdaki değişkenleri tanımlayın:

isim: Kendi isminizi içeren bir metin
yas: Kendi yaşınızı içeren bir tamsayı
boy: Kendi boyunuzu içeren bir ondalıklı sayı
ogrenci_mi: Öğrenci olup olmadığınızı belirten bir mantıksal değer (True veya False)

2. Aşağıdaki veri tiplerine uygun birer örnek yazın:

Bir liste
Bir demet
Bir sözlük

####Bu ders, Python'da değişkenler ve veri tipleri hakkında temel bilgileri öğrenmenizi sağladı. Bu temel bilgileri kavradıktan sonra, daha ileri konuları keşfetmeye başlayabilirsiniz.
