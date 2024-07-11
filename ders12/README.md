# Python'da Sözlükler ve Kümeler
## Sözlükler (Dictionaries)
Sözlükler, Python'da anahtar-değer çiftleriyle ilişkilendirilmiş veri yapılarıdır. Her anahtar benzersiz olmalıdır ve bir değere karşılık gelir.

### Sözlük Oluşturma
Sözlükler süslü parantez {} içinde ve anahtarlar ile değerler arasında : kullanılarak tanımlanır.

##### Örneğin:

````
sozluk = {'anahtar1': 'deger1', 'anahtar2': 'deger2', 'anahtar3': 'deger3'}
````
Sözlüklerin Özellikleri:    

* Değiştirilebilir (Mutable): Sözlüklerdeki değerler eklenebilir, çıkarılabilir veya değiştirilebilir.
* İndekslenmiş: Değerlere erişmek için anahtarlar kullanılır.
* Sırasızdır: Sözlüklerdeki anahtar-değer çiftleri tanımlandıkları sırayla tutulmazlar.

### Temel Sözlük İşlemleri:
* Değer Ekleme veya Güncelleme:

````
sozluk['yeni_anahar'] = 'yeni_deger'
````

* Değer Silme:

````
del sozluk['anahtar1']
````

* Anahtarlar ve Değerler:
````
print(sozluk.keys())   # Tüm anahtarları listeler
print(sozluk.values()) # Tüm değerleri listeler
````

## Kümeler (Sets)
Kümeler, Python'da benzersiz ve sırasız elemanların bir araya geldiği veri yapılarıdır. Bir küme içinde aynı elemandan yalnızca bir tane bulunabilir.

### Küme Oluşturma
Kümeler süslü parantez {} veya set() fonksiyonu kullanılarak oluşturulabilir.

#### Örneğin:

````
kume = {1, 2, 3, 4, 5}
````
### Kümelerin Özellikleri:

* Değiştirilebilir (Mutable): Kümelerdeki elemanlar eklenebilir veya çıkarılabilir.
* Benzersiz Elemanlar: Bir küme içinde her elemandan yalnızca bir tane bulunabilir.
* Sırasızdır: Kümelerdeki elemanlar tanımlandıkları sırayla tutulmazlar.

### Temel Küme İşlemleri:

* Eleman Ekleme:

````
kume.add(6)
````


