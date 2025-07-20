# Lain’i Çok Seviyorum: Brainfuck Tarzı C++ ile Anime Temalı Kod

Bu proje, C++ dilinde Brainfuck’un minimalist yaklaşımını yansıtarak, yalnızca tek bir `char` değişkeni üzerinde işlemler yaparak konsola "Lain’i çok seviyorum" mesajını yazdırıyor. Kod; **Serial Experiments Lain**, **Vocaloid karakterleri** (Miku, IA, Rin, Len, Meiko, Gumi, Kaito), ve **Yuno Gasai** gibi anime ikonlarından ilham alan `#define` makrolarıyla süslenmiş bir _cyberpunk_ estetiği taşıyor. 🌐🎶

## 🎯 Amaç

- Konsola `"Lain’i çok seviyorum"` yazdırmak.
- Bunu sıradan `cout` ile değil, tek bir `char` değişkeni (`cell`) üzerinde `++` ile değer artırarak gerçekleştirmek.
- Kodun her satırı anime referanslarıyla şekillendirilmiş.

## 💡 Nasıl Yaptık?

### 1. Brainfuck’tan Esinlenme

Brainfuck, bir hücredeki değeri artırarak (`+`) ve azaltarak (`-`) karakterler üretir, `.` ile yazdırır. Bu projede de benzer şekilde:

- `char cell = 0` ile başladık.
- Her karakter için ASCII değerine ulaşana kadar `cell`’i artırdık.
- Her adımda `cout << cell` ile karakteri yazdırdık.
- Kod her karakterden sonra `cell = 0` ile sıfırlanıyor ve yeni karakter için tekrar artırılıyor.

### 2. Anime Temalı `#define`’lar

Koda anime/cyberpunk havası katmak için `#define` kullanarak C++’ın temel yapılarını yeniden adlandırdık:

| Tanım      | Anlamı                | Kaynak/Referans            |
| ---------- | --------------------- | -------------------------- |
| `just`     | `using`               |                            |
| `kill`     | `namespace`           |                            |
| `yourself` | `std`                 |                            |
| `Lain`     | `;`                   | Serial Experiments Lain    |
| `more`     | `int`                 |                            |
| `cpp`      | `main`                |                            |
| `Kaito`    | `char`                | Vocaloid - Kaito           |
| `IA`       | `=`                   | Vocaloid - IA              |
| `Rin`      | `cout`                | Vocaloid - Rin             |
| `Len`      | `<<`                  | Vocaloid - Len             |
| `Teto`     | `return`              | Vocaloid - Teto            |
| `Meiko(x)` | `x = x + 1`           | Vocaloid - Meiko           |
| `Gumi(x)`  | `x = x - 1`           | Vocaloid - Gumi            |
| `Yuno(x)`  | `x` (parantez içi)    | Yuno Gasai (Mirai Nikki)   |
| `Akino(x)` | `x` (parantez kapama) | Anime uyumu                |
| `learn`    | `for`                 | Öğrenmeyi vurgulayan ifade |

### 3. Karakter Üretimi

Kodda yazdırılan metin:

> **Lain’i çok seviyorum**

Her karakterin ASCII değeri elle hesaplanarak `cell` değişkenine `++` ile ulaşılıyor ve ardından `cout << cell` ile yazdırılıyor. Her karakterden sonra `cell` sıfırlanıyor.

ASCII dizisi şu şekildedir:

hihihi
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
hihihi

Her karakter şu şekilde yazılıyor:

hihihi
Yuno(cell) IA 0 Lain
learn(more i IA 0 Lain i < 76 Lain i++) { Meiko(cell) Lain } Rin Len Akino(cell) Lain
hihihi

Bu yapı her karakter için tekrar ediyor, yalnızca hedef ASCII değeri değişiyor.

### 4. Kodun Özeti

- Yalnızca bir `char` (`cell`) kullanarak her karakter oluşturuluyor.
- Kodun her satırı anime karakter isimleriyle ifade ediliyor.
- Kod, hem Brainfuck’un estetiğini hem de anime kültürünü yansıtıyor.
- **C++’ta yazılmış en duygusal beyin yakan kod** olabilir 💜

## 🚀 Derleme ve Çalıştırma

hihihi
g++ -o lain_brainfuck lain_brainfuck.cpp
./lain_brainfuck
hihihi

Konsolda şu yazıyı görmelisiniz:

hihihi
Lain’i çok seviyorum
hihihi

## 💬 İlham Kaynakları

- **Serial Experiments Lain** – İnternet, gerçeklik ve kimlik üzerine bir klasik.
- **Vocaloid** – Sesin dijitalle buluştuğu yerde doğan karakterler.
- **Brainfuck** – Minimalizmin zirvesi olan bir programlama dili.
- **Yuno Gasai** – Sadakatin ve deliliğin ikonik simgesi.

> _“Herkes bağlı. Wired’a, Lain’e, duygulara.”_
