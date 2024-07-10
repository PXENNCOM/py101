# Öğrenci Bilgi Sistemi Uygulaması

Bu uygulamanın ilk dersten itibaren yapılması size zorlayıcı gelebilir. Ancak, müfredatımızda konuları adım adım detaylı bir şekilde zaten işleyeceğiz. Bu uygulama, sadece farklı bir başlangıç yapmak ve kod yazma sürecine dair bir ön fikir vermek amacıyla tasarlanmıştır. Python 101 derslerinde ele alacağımız birçok konudan küçük örnekler içermekte ve her satırı detaylı olarak açıklamaktayız. Lütfen kodu inceleyin, düşünün ve anlamasanız bile yazmayı deneyin. Bu süreç, öğrenme yolculuğunuzda size yardımcı olacaktır.

öğrenci bilgilerini yönetmek için basit bir yapı sunar. Kullanıcıya öğrenci eklemek, öğrenci bilgilerini listelemek için bir arayüz sağlar. Bu sayede değişkenler, döngüler ve fonksiyonlar gibi temel Python kavramlarını pratiğe dökebilirsiniz.

### "#" ile başlayan satırlara yorum satırı denir. Uygulamaya hiç bir etki etmez. 

````

# Programın ana fonksiyonunu tanımlıyoruz
def main():
    # Ekrana hoş geldiniz mesajı yazdırıyoruz
    print("Hoş Geldiniz!")
    
    # Sonsuz bir döngü başlatıyoruz, kullanıcı çıkış yapana kadar devam edecek
    while True:
        # Kullanıcıya yapmak istediği işlemi soruyoruz
        print("\nLütfen yapmak istediğiniz işlemi seçin:")
        print("1. Öğrenci Ekle")
        print("2. Öğrenci Listele")
        print("3. Çıkış")

        # Kullanıcının seçimini alıyoruz
        choice = input("Seçiminizi yapın (1/2/3): ")

        # Kullanıcının seçimine göre işlemler yapıyoruz
        if choice == "1":
            # Kullanıcı 1'i seçtiyse, öğrenci ekleme fonksiyonunu çağırıyoruz
            add_student()
        elif choice == "2":
            # Kullanıcı 2'yi seçtiyse, öğrenci listeleme fonksiyonunu çağırıyoruz
            list_students()
        elif choice == "3":
            # Kullanıcı 3'ü seçtiyse, programdan çıkıyoruz
            print("Programdan çıkılıyor...")
            break
        else:
            # Kullanıcı geçersiz bir seçim yaptıysa, uyarı mesajı yazdırıyoruz
            print("Geçersiz seçim. Tekrar deneyin.")

# Öğrenci bilgilerini tutacak bir liste oluşturuyoruz
students = []

# Yeni öğrenci ekleme fonksiyonunu tanımlıyoruz
def add_student():
    print("\nÖğrenci ekleme işlemi:")
    # Kullanıcıdan öğrencinin adını alıyoruz
    name = input("Öğrencinin adını girin: ")
    # Kullanıcıdan öğrencinin notunu alıyoruz
    grade = float(input("Öğrencinin notunu girin: "))

    # Yeni öğrenciyi sözlük olarak oluşturup listeye ekliyoruz
    students.append({"name": name, "grade": grade})
    # Öğrencinin başarıyla eklendiğini bildiriyoruz
    print(f"{name} adlı öğrenci başarıyla eklendi!")

# Öğrenci listeleme fonksiyonunu tanımlıyoruz
def list_students():
    print("\nÖğrenci Listesi:")
    # Öğrenciler listesindeki her bir öğrenci için döngü başlatıyoruz
    for student in students:
        # Her bir öğrencinin adını ve notunu yazdırıyoruz
        print(f"{student['name']} - Notu: {student['grade']}")

# Bu dosya doğrudan çalıştırıldığında ana fonksiyonu çalıştırıyoruz
if __name__ == "__main__":
    main()
````

### Detaylı Açıklamalar

1. def main(): - Programın ana fonksiyonunu tanımlıyoruz.
2. print("Hoş Geldiniz!") - Kullanıcıya hoş geldiniz mesajı yazdırıyoruz.
3. while True: - Sonsuz bir döngü başlatıyoruz, böylece kullanıcı işlemleri seçip tekrar tekrar yapabilir.
4. print("\nLütfen yapmak istediğiniz işlemi seçin:") - Kullanıcıya yapmak istediği işlemi sormak için bir menü gösteriyoruz.
5. print("1. Öğrenci Ekle") - Kullanıcıya 1. seçeneği gösteriyoruz (Öğrenci Ekle).
6. print("2. Öğrenci Listele") - Kullanıcıya 2. seçeneği gösteriyoruz (Öğrenci Listele).
7. print("3. Çıkış") - Kullanıcıya 3. seçeneği gösteriyoruz (Çıkış).
8. choice = input("Seçiminizi yapın (1/2/3): ") - Kullanıcının seçimini alıyoruz.
9. if choice == "1": - Kullanıcı 1'i seçerse:
10. add_student() - add_student fonksiyonunu çağırıyoruz.
11. elif choice == "2": - Kullanıcı 2'yi seçerse:
12. list_students() - list_students fonksiyonunu çağırıyoruz.
13. elif choice == "3": - Kullanıcı 3'ü seçerse:
14. print("Programdan çıkılıyor...") - Çıkış mesajı yazdırıyoruz.
15. break - Döngüyü kırarak programdan çıkıyoruz.
16. else: - Geçersiz bir seçim yapılmışsa:
17. print("Geçersiz seçim. Tekrar deneyin.") - Uyarı mesajı yazdırıyoruz.
18. students = [] - Öğrenci bilgilerini tutacak bir liste oluşturuyoruz.
19. def add_student(): - Yeni öğrenci ekleme fonksiyonunu tanımlıyoruz.
20. print("\nÖğrenci ekleme işlemi:") - Öğrenci ekleme işlemi başladığını belirten mesajı yazdırıyoruz.
21. name = input("Öğrencinin adını girin: ") - Kullanıcıdan öğrencinin adını alıyoruz.
22. grade = float(input("Öğrencinin notunu girin: ")) - Kullanıcıdan öğrencinin notunu alıyoruz.
23. students.append({"name": name, "grade": grade}) - Yeni öğrenciyi sözlük olarak oluşturup listeye ekliyoruz.
24. print(f"{name} adlı öğrenci başarıyla eklendi!") - Öğrencinin başarıyla eklendiğini bildiriyoruz.
25. def list_students(): - Öğrenci listeleme fonksiyonunu tanımlıyoruz.
26. print("\nÖğrenci Listesi:") - Öğrenci listesinin başlığını yazdırıyoruz.
27. for student in students: - Öğrenciler listesindeki her bir öğrenci için döngü başlatıyoruz.
28. print(f"{student['name']} - Notu: {student['grade']}") - Her bir öğrencinin adını ve notunu yazdırıyoruz.
29. if __name__ == "__main__": - Bu dosya doğrudan çalıştırıldığında:
30. main() - main fonksiyonunu çalıştırıyoruz.

Bu açıklamalar, her bir satırın ne işe yaradığını anlamanıza yardımcı olacaktır. Programı bu şekilde detaylandırarak, Python'un temel kavramlarını ve yapılarını daha iyi anlayabilirsiniz.


