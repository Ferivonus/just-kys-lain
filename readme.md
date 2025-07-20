# Lain’i Çok seviyorum

Bu projede tek bir değer üzerinden veri manipülasyonu yapılarak ekrana kelime yazdırılmıştır.

## 🎯 Amaç

- Sıkıntımın geçmesine uğraşmak.
- Konsola `"Lain’i çok seviyorum"` yazdırmak.

## 1. Anime Temalı `#define`’lar

Sıkıntım geçmesi için bazı şeyleri birazcık değiştirdim ama:

| Tanım      | Anlamı                | Kaynak/Referans          |
| ---------- | --------------------- | ------------------------ |
| `just`     | `using`               |                          |
| `kill`     | `namespace`           |                          |
| `yourself` | `std`                 |                          |
| `Lain`     | `;`                   | Serial Experiments Lain  |
| `learn`    | `for`                 |                          |
| `more`     | `int`                 |                          |
| `cpp`      | `main`                |                          |
| `Kaito`    | `char`                | Vocaloid - Kaito         |
| `IA`       | `=`                   | Vocaloid - IA            |
| `Rin`      | `cout`                | Vocaloid - Rin           |
| `Len`      | `<<`                  | Vocaloid - Len           |
| `Teto`     | `return`              | Vocaloid - Teto          |
| `Meiko(x)` | `x = x + 1`           | Vocaloid - Meiko         |
| `Gumi(x)`  | `x = x - 1`           | Vocaloid - Gumi          |
| `Yuno(x)`  | `x` (parantez içi)    | Yuno Gasai (Mirai Nikki) |
| `Akino(x)` | `x` (parantez kapama) |                          |

### 2. Karakter Üretimi

Kodda yazdırılan metin:

> **Lain’i çok seviyorum**

Her karakterin ASCII değeri elle hesaplanarak `cell` değişkenine `++` ile ulaşılıyor ve ardından `cout << cell` ile yazdırılıyor. Her karakterden sonra `cell` sıfırlanıyor.

ASCII dizisi şu şekildedir:

```
L (76)
a (97)
i (105)
n (110)
’ (39)
i (105)
(32)
c (99)
o (111)
k (107)
(32)
s (115)
e (101)
v (118)
i (105)
y (121)
o (111)
r (114)
u (117)
m (109)
```

Her karakter şu şekilde yazılıyor:

```
Yuno(cell) IA 0 Lain
learn(more i IA 0 Lain i < 76 Lain i++) { Meiko(cell) Lain } Rin Len Akino(cell) Lain
```

Bu yapı her karakter için tekrar ediyor, yalnızca hedef ASCII değeri değişiyor.

### 4. Kodun Özeti

- Yalnızca bir `char` (`cell`) kullanarak her karakter oluşturuluyor.
- Kodun her satırı anime karakter isimleriyle ifade ediliyor.
- Kod, hem Brainfuck’un estetiğini hem de anime kültürünü yansıtıyor.
- **C++’ta yazılmış en duygusal beyin yakan kod** olabilir 💜

## 🚀 Derleme ve Çalıştırma

```
g++ -o lain_brainfuck lain_brainfuck.cpp
./lain_brainfuck
```

Konsolda şu yazıyı görmelisiniz:

```
Lain’i çok seviyorum
```

## 💬 İlham Kaynakları

- **Serial Experiments Lain** – İnternet, gerçeklik ve kimlik üzerine bir klasik.
- **Vocaloid** – Sesin dijitalle buluştuğu yerde doğan karakterler.
- **Brainfuck** – Minimalizmin zirvesi olan bir programlama dili.
- **Yuno Gasai** – Sadakatin ve deliliğin ikonik simgesi.

> _“Herkes bağlı. Wired’a, Lain’e, duygulara.”_
