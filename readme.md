# I Love Lain So Much

In this project, data is manipulated using a single value to print a sentence on the screen.

## 🎯 Goal

- To try to relieve my distress.
- To print `"I love Lain so much"` to the console.

## 1. Anime-Themed `#define`s

To relieve my distress, I changed a few things a little bit:

| Definition | Meaning             | Source/Reference         |
| ---------- | ------------------- | ------------------------ |
| `just`     | `using`             |                          |
| `kill`     | `namespace`         |                          |
| `yourself` | `std`               |                          |
| `Lain`     | `;`                 | Serial Experiments Lain  |
| `learn`    | `for`               |                          |
| `more`     | `int`               |                          |
| `cpp`      | `main`              |                          |
| `Kaito`    | `char`              | Vocaloid - Kaito         |
| `IA`       | `=`                 | Vocaloid - IA            |
| `Rin`      | `cout`              | Vocaloid - Rin           |
| `Len`      | `<<`                | Vocaloid - Len           |
| `Teto`     | `return`            | Vocaloid - Teto          |
| `Meiko(x)` | `x = x + 1`         | Vocaloid - Meiko         |
| `Gumi(x)`  | `x = x - 1`         | Vocaloid - Gumi          |
| `Yuno(x)`  | `x` (inside parens) | Yuno Gasai (Mirai Nikki) |
| `Akino(x)` | `x` (close parens)  |                          |

## 2. Character Generation

The printed message in the code is:

> **I love Lain so much**

Each character’s ASCII value is manually reached by incrementing the `cell` variable with `++`, and then printed using `cout << cell`. After each character, `cell` is reset to 0.

The ASCII sequence is as follows:

```
L (76)
a (97)
i (105)
n (110)
’ (39)
i (105)
(space) (32)
c (99)
o (111)
k (107)
(space) (32)
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

Each character is generated like this:

```
Yuno(cell) IA 0 Lain
learn(more i IA 0 Lain i < 76 Lain i++) { Meiko(cell) Lain }
Rin Len Akino(cell) Lain
```

This structure is repeated for every character, only the target ASCII value changes.

## 4. Code Summary

- Only one `char` (`cell`) is used to construct each character.
- Every line of the code is expressed using anime character names.
- The code reflects both Brainfuck’s aesthetic and anime culture.
- It might be **the most emotional brain-melting code ever written in C++** 💜

## 🚀 Compile and Run

```
g++ -o lain_brainfuck lain_brainfuck.cpp
./lain_brainfuck
```

You should see this output on the console:

```
I love Lain so much
```

## 💬 Sources of Inspiration

- **Serial Experiments Lain** – A classic on the internet, reality, and identity.
- **Vocaloid** – Characters born where voice meets the digital.
- **Brainfuck** – The pinnacle of minimalism in programming.
- **Yuno Gasai** – The iconic symbol of loyalty and madness.

> _“Everyone is connected. To the Wired, to Lain, to emotions.”_
