# Class Members (Sınıf Üyeleri)

### Field (Alan)

Field, bir nesne içerisinde veri depolamak veya tutmak için kullanılan alanlardır. Sınıf içerisindeki değişkenlerdir ve herhangi bir türden olabilir. Field'lar, türlerine özgü varsayılan değerler alır (örneğin, `int a;` varsayılan olarak `0` değerini alır). Varsayılan değerler yalnızca field'larda atanabilir; metotlar veya diğer yapılar için varsayılan değer verilmez.

### Property (Özellik)

Property, bir nesne içerisinde özellik sağlamaktadır. Aslında bir metot olan property, fiziksel olarak parametre almamakta ve içinde `get` ve `set` olmak üzere iki blok barındırmaktadır. Bu bloklar, derleme sonucunda `get` ve `set` isimli metotlar olarak ortaya çıkar.

#### Property Blokları
- **get**: Property'nin değeri çağrıldığında tetiklenir.
- **set**: Property'e bir değer gönderildiğinde tetiklenir.

Property'ler, field'lara doğrudan erişimi kontrol etmek amacıyla kullanılır. Böylece, nesne üzerindeki veri okuma ve atama işlemleri daha güvenli bir şekilde gerçekleştirilir. Bu işleme kapsülleme (encapsulation) denir.

### Kapsülleme (Encapsulation)

Kapsülleme, bir nesne içerisindeki verilerin (field'lardaki verilerin) dışarıya kontrollü bir şekilde erişilmesini sağlamaktadır.

### Property İmzaları

Property yapısı oluşturmanın birkaç farklı yolu vardır:
1. **Full Property**
2. **Prop**
3. **Auto Property Initializers**
4. **Ref Readonly Returns**
5. **Computed Properties**
6. **Expression-Bodied Property**
7. **Init-Only Properties ve Init Accessor**

#### 1. Full Property

En sade property yapısıdır. `get` ve `set` blokları tanımlanmalıdır.

```csharp
class MyClass 
{
    private int yasi;

    public int Yasi 
    {
        get { return yasi; }
        set { yasi = value; }
    }
}
```

#### 2. Prop Property

Bir property'nin, field'daki veriye müdahale etmeden erişimini sağlar.

```csharp
class MyClass 
{
    public int Yasi { get; set; }
}
```

#### 3. Auto Property Initializers (C# 6.0)

ReadOnly olan property'lere hızlıca değer atamaya olanak tanır.

```csharp
public int Yasi { get; set; } = 20;
```

#### 4. Ref Readonly Returns

Bir sınıf içerisindeki field'ı referansıyla döndürmemizi sağlar.

```csharp
public ref readonly string Adi => ref adi;
```

#### 5. Computed Properties

Aritmetik işlemler yapan property'lerdir.

```csharp
public int Topla 
{
    get { return s1 + s2; }
}
```

#### 6. Expression-Bodied Property

Lambda ifadeleri kullanarak tanımlamayı sağlar.

```csharp
public string Cinsiyet => "Kadın";
```

#### 7. Init-Only Properties (C# 9.0)

Nesnenin sadece yaratılış anında property'lerine değer atamasını sağlar.

## Metot

Nesne üzerinde, field'lar veya dışarıdan parametreler ile gelen değerler üzerinde işlemler yapmamızı sağlar. Hiçbir property, metotlarda yapılabildiği gibi `void` (geriye dönüş değeri olmayan) olamaz.

## Indexer (İndeksleyici)

Nesneye indeksleme özelliği kazandıran, property ile benzer yapıdadır.

```csharp
public int this[int a] 
{
    get { return a; }
    set { yas = value; }
}
```

## Sonuç

C# dilinde OOP prensiplerini anlamak, yazılım geliştirme süreçlerimizi daha etkili hale getirecektir. Yukarıda belirtilen özellikler ve yapılar, nesne yönelimli programlamanın temel taşlarını oluşturur ve yazılımın sürdürülebilirliğini artırır.
