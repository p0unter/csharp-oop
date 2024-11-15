# CLASS Kavramı

## Sınıf Kavramı Nedir? Neden Sınıf Yapısı Kullanılır?
OOP'de bir nesne oluşturabilmek için öncelikle o nesnenin modellenmesi ve tanımlanması gerekmektedir. Bir nesnenin tanımını oluşturmak için sınıf yapısı kullanılır. Sınıf içinde field, property, indexer ve metotlar tanımlanabilir.

## Sınıf ile Nesne Arasındaki İlişki Nedir?
Sınıflarda, nesnelerdeki ortak alan tanımları yapılır (Örn: Adı (Field), YasHesapla (Metot)).

## Sınıf Nasıl Oluşturulur ve Nerede Oluşturulur?

### Nasıl Oluşturulur?
Sınıf, `class Sınıfİsim { }` şeklinde tanımlanır.

### Nerede Oluşturulur?
Sınıf üç farklı yerde oluşturulabilir:

1. **Namespace içerisinde:** Sınıf, belirli bir isim alanında tanımlanır.
2. **Namespace dışında:** Sınıf, namespace dışında tanımlandığında erişim için uygun hale getirilmelidir.
3. **Namespace'den bağımsız, sınıf içinde (Nested):** İç içe sınıf olarak tanımlanabilir.

> **Önemli:** Bir isim alanı veya sınıf içinde aynı isimde birden fazla sınıf tanımlanamaz.

## Sınıf ile Nesne Modeli Tasarlama
Sınıf içinde tanımlanan tüm değişkenler bir field'dir (Örn: `int a;`).

## Sınıf Modelinden Referans Noktası Oluşturma
Stack'te tanımlanan referans noktası ile Heap'teki nesneye ulaşabiliriz. Bir sınıf tanımlandığında, o sınıf bir türdür. Bu türü kullanabilmek için sınıf adını kullanmamız yeterlidir (Örn: `OrnekModel degisken_ismi;`).

Eğer bir referans, herhangi bir nesneye işaret etmiyorsa, bu referans noktası `null` değere sahiptir. Referans türündeki değişkenler özünde nullable değişkenlerdir.
