# Object Oriented Programming (OOP)

## Nedir?
Nesne yönelimli programlama, günümüzde birçok modern dil tarafından desteklenen bir yaklaşımdır.

## Amacı
Yazılım geliştirme sürecini kısaltan ve sistematik hale getiren bir tekniktir.

## Yaklaşım Şekli
Gerçek hayatı simüle eden nesneleri baz alan bir programlama tekniğidir. Her şey bir nesne olarak modellenir:

- Sen
- Ben
- Personel
- Ürün

## Çalışma Şekli
Gerçek bir sistem, nesnel parçalara ayrılır ve bu parçalar (nesneler) arasında ilişkiler kurulur. Nesneler kendi aralarında haberleşebilir.

## Nesnenin Anatomisi
Merkezde obje vardır: Nesne tabanlı programlamada en küçük esas parça nesne/obje'dir.

- **Field**: Nesneler içinde veri tutulan alanlar.
- **Metotlar**: Nesneler içinde field'lardaki değerleri işleyen fonksiyonlar.

> **Not:** Tüm nesneler bir sınıf modellemesinin örneğidir.

## Nesne Kavramı
Nesne, nesnellik felsefesine dayanan bir kavramdır. Programlamada nesneler, günlük hayattaki nesnelerin muadilidir.

Gerçek hayattaki herhangi bir olguyu, programlama dünyasında nesne olarak tarif eder ve o şekilde modelleyebiliriz.

## Nesne Modellemesi
Nesnelerin oluşturulabilmesi için önce modellenmesi gereklidir. Nesne modeli **class** ile gerçekleştirilir.

## Nesneler Hangi Türdendir?
Nesneler referans türündedir.

### Referans Türlü Değerler Nedir?
- **STACK**: Değer türündeki değişkenler ve referanslar tutulur.
- **HEAP**: Sadece nesneler tutulur.

Nesne, bir veya birden fazla değer barındıran yapılardır.

- **Stack'te**: Kod yazarken değişkenlere isimleri üzerinden erişebiliriz.
- **Heap'teki nesnelere erişim**: Heap'teki nesnelere direkt erişemeyiz ancak Stack'teki referanslar aracılığıyla erişebiliriz. Stack'te Heap'teki nesneleri işaret eden referanslar tanımlarız, böylece dolaylı olarak erişim sağlamış oluruz.

## Sınıf (Class) Kavramı
Sınıf, OOP'nin temelidir. Sınıflar, nesnelerin şablonlarıdır.
