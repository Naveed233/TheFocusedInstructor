
This chapter introduces expressions, variables, comments, and Python’s most basic data types. Most students won’t struggle much with syntax, but instructors should focus on reinforcing **mental models** (like "a variable is a label for a box") and making abstract types feel real.

---
[[#🧮 1. Python Expressions]]
[[#📦 2. Introduction to Variables]]
[[#💬 3. Comments]]
[[#🧰 4. Introduction to Data Types]]
[[#🔢 5. Numeric Data Types]]
[[#✅ Summary for Instructors]]

## 🧮 1. Python Expressions

### ✅ Key Concepts
- An **expression** is any valid combination of values and operators that returns a result.
- Python uses **mathematical operators**: `+`, `-`, `*`, `/`, `//`, `%`, `**`
- **Order of operations** matters (PEMDAS-style logic)
- Parentheses `()` can override the default order.

### ⚠️ Common Issues
- Students may misread order of operations (`2 + 3 * 4`)
- Forget that `/` returns a float, `//` returns an integer
- Use invalid combinations like `"hello" * "3"`

### 🧑‍🏫 Instructor Tips
- Write a few expressions on the board. Ask students: “What will this return?”
- Run expressions in REPL and change parentheses to show effect.
- Give “guess the output” challenges.

```python
5 * 6 / 3 + 2      # 12.0
2**4 * 2           # 32
15 // 4 + 2        # 5
"hello" + " world" # hello world
```

---

### 📣 Japanese Phrases (Expressions)
| Japanese | English | Romaji |
|----------|---------|--------|
| 式は値を返します。 | Expressions return values. | shiki wa atai o kaeshimasu |
| 順序に気をつけてください。 | Be careful with order of operations. | junjo ni ki o tsukete kudasai |
| 括弧は優先されます。 | Parentheses take priority. | kakko wa yūsen saremasu |

---

## 📦 2. Introduction to Variables

### ✅ Key Concepts
- A **variable** stores a value with a name.
- Think of a variable like a **labeled box** storing something in memory.
- Variables can be reassigned or even hold different data types later.
- Syntax: `name = value`

### ⚠️ Common Issues
- Students use invalid names (start with numbers, use spaces)
- Confuse `=` (assignment) with `==` (comparison)
- Don’t understand that assignment changes the value stored
- Forget quotes when assigning strings

### 🧑‍🏫 Instructor Tips
- Use the **box analogy**:
  > "You don’t need to open the box, just read the label!"
- Show how variables are reassigned:
  ```python
  user_name = "John"
  user_name = "Sarah"
  ```
- Demonstrate assignment using values and other variables.

```python
a = 5
b = 10
total = a + b  # 15
```

---

### 📣 Japanese Phrases (Variables)
| Japanese | English | Romaji |
|----------|---------|--------|
| 変数はデータを保存します。 | Variables store data. | hensū wa dēta o hozon shimasu |
| 変数名は数字で始められません。 | Variable names cannot start with numbers. | hensūmei wa sūji de hajimeraremasen |
| `=` は代入です。 | `=` means assignment. | `=` wa dainyū desu |

---

## 💬 3. Comments

### ✅ Key Concepts
- Comments explain the code or disable parts of it.
- Start a comment with `#` for single-line.
- Use `""" """` or `''' '''` for multi-line comments.

### ⚠️ Common Issues
- Students forget `#` or try to “comment” in regular text
- Try to comment with slashes like `//` (common in other languages)
- Don’t know that triple quotes are not **technically** comments (they're just unused string blocks)

### 🧑‍🏫 Instructor Tips
- Show:
  ```python
  # This adds two numbers
  x = 5
  y = 10
  z = x + y  # result is 15
  ```
- Teach: “Comment for humans, not for the computer.”

---

### 📣 Japanese Phrases (Comments)
| Japanese | English | Romaji |
|----------|---------|--------|
| コメントは実行されません。 | Comments are not executed. | komento wa jikkō saremasen |
| `#` を使ってコメントします。 | Use `#` to write a comment. | `#` o tsukatte komento shimasu |

---

## 🧰 4. Introduction to Data Types

### ✅ Key Concepts
- **Data types** define the kind of value stored: text, number, etc.
- Python has many types, but the main ones are:
  - **String**: `"Hello"`
  - **Integer**: `25`
  - **Float**: `25.5`

### ⚠️ Common Issues
- Forgetting quotes for strings
- Confusing `"3.14"` (string) with `3.14` (float)
- Not knowing what a "type" really is

### 🧑‍🏫 Instructor Tips
- Show real-world examples:
  - `"john.doe@email.com"` = string
  - `123456` = int
  - `3.14` = float
- Play a “What type is this?” game with students

---

### 📣 Japanese Phrases (Data Types)
| Japanese | English | Romaji |
|----------|---------|--------|
| データには種類があります。 | Data has types. | dēta ni wa shurui ga arimasu |
| 文字列はクオートで囲みます。 | Strings are enclosed in quotes. | mojiretsu wa kuōto de kakomimasu |

---

## 🔢 5. Numeric Data Types

### ✅ Key Concepts
- **Integers** are whole numbers: `1`, `0`, `-5`
- **Floats** are decimals: `3.14`, `-1.7`
- Numbers are used differently depending on context (e.g. salary vs ID)

### ⚠️ Common Issues
- Mistaking strings for numbers (e.g. `"100"` vs `100`)
- Forgetting decimal point for floats
- Mixing types in operations (`"10" + 5` causes error)

### 🧑‍🏫 Instructor Tips
- Show how Python handles:
  ```python
  x = 10
  y = 2.5
  print(x + y)  # 12.5
  ```
- Use Celsius → Fahrenheit as a practice exercise:
  ```python
  celsius = 25.0
  fahrenheit = celsius * 1.8 + 32
  ```

---

### 📣 Japanese Phrases (Numbers)
| Japanese | English | Romaji |
|----------|---------|--------|
| 整数は小数点がありません。 | Integers have no decimal. | seisū wa shōsūten ga arimasen |
| `3.14` は小数（float）です。 | `3.14` is a float. | `3.14` wa shōsū desu |

---

## ✅ Summary for Instructors

- Build strong mental models:
  - Variables = labeled boxes
  - Data types = kinds of contents
- Focus more on **why** than just syntax.
- Use REPL to demonstrate results in real time.
- Let students make small mistakes and figure it out.
- Use real-world analogies to bring abstract ideas to life.

