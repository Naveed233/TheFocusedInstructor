
This chapter introduces how strings behave in Python and the concept of built-in functions for string handling and type conversion. Instructors should emphasize how Python treats strings differently from numbers and help students identify common type errors early.

---

- [[#1. String Operations]]
- [[#2. Built-in Functions For Strings]]
- [[#3. Built-in Functions for Type Conversion]]
   
## 1. String Operations

### ✅ Key Concepts

- `+` is used to **concatenate** (join) strings.
- `*` is used to **replicate** strings.
- Operations between mismatched types (like string + int) cause errors.
    

### ⚠️ Common Issues

- Trying to add a string to an integer without converting it first.
- Using `"text" * "2"` or `"name" * 2.5` causes errors.
- Students assuming Python treats numbers and strings the same way.

### 🧑‍🏫 Instructor Tips

- Demonstrate correct use:

```python
first_name = "John"
last_name = "Smith"
full_name = first_name + " " + last_name
print(full_name)  # John Smith

print("Hi" * 3)    # HiHiHi
```

- Try invalid operations on purpose and read the error:

```python
print("Age: " + 25)        # TypeError
print("Hi" * "3")          # TypeError
print("Hello" * 2.5)       # TypeError
```

### 📣 Japanese Phrases (String Ops)

| Japanese              | English                       | Romaji                                          |
| --------------------- | ----------------------------- | ----------------------------------------------- |
| 文字列を結合するには `+` を使います。 | Use `+` to join strings.      | mojiretsu o ketsugō suru ni wa `+` o tsukaimasu |
| `*` を使うと文字列を繰り返せます。   | Use `*` to repeat strings.    | `*` o tsukau to mojiretsu o kurikaesemasu       |
| 型が違うとエラーになります。        | Different types cause errors. | kata ga chigau to erā ni narimasu               |

---

## 2. Built-in Functions For Strings

### ✅ Key Concepts

- `print()` displays values in the terminal.
- `input()` collects user input (always as a string).
- `len()` returns the number of characters in a string.
    
### ⚠️ Common Issues

- Forgetting that `input()` returns a string.
- Trying to perform math on `input()` values without conversion.
- Expecting `len()` to count words instead of characters.

### 🧑‍🏫 Instructor Tips

- Make a simple app:    

```python
name = input("What is your name? ")
print("Hello, " + name + "!")
```

- Show how `len()` counts characters:

```python
message = "Python"
print(len(message))  # 6
```

- Pass function output into other functions:

```python
print(len(input("Type a word: ")))
```

### 📣 Japanese Phrases (String Functions)

|Japanese|English|Romaji|
|---|---|---|
|`print()` は画面に表示します。|`print()` shows text.|`print()` wa gamen ni hyōji shimasu|
|`input()` はキーボードから受け取ります。|`input()` takes user input.|`input()` wa kibōdo kara uketorimasu|
|`len()` は文字数を返します。|`len()` returns length.|`len()` wa mojisū o kaeshimasu|

---

## 3. Built-in Functions for Type Conversion

### ✅ Key Concepts

- `str()` converts data to string
- `int()` converts strings (or floats) to integer
- `float()` converts to a floating-point number
- `type()` shows the data type

### ⚠️ Common Issues

- Forgetting to use `str()` in concatenation
- Assuming `int("hello")` will work
- Misunderstanding what `type()` shows

### 🧑‍🏫 Instructor Tips

- Show working type conversions:

```python
age = 25
print("I am " + str(age) + " years old.")
```

- Show type checking:
    

```python
print(type("hello"))     # <class 'str'>
print(type(3.14))        # <class 'float'>
print(type(int("123")))  # <class 'int'>
```

- Show failed conversions:

```python
int("hello")  # ValueError
```

### 📣 Japanese Phrases (Type Conversion)

| Japanese               | English                      | Romaji                                  |
| ---------------------- | ---------------------------- | --------------------------------------- |
| `str()` は文字列に変換します。    | `str()` converts to string.  | `str()` wa mojiretsu ni henkan shimasu  |
| `int()` は整数に変換します。     | `int()` converts to integer. | `int()` wa seisū ni henkan shimasu      |
| `float()` は小数に変換します。   | `float()` converts to float. | `float()` wa shōsū ni henkan shimasu    |
| `type()` はデータの種類を返します。 | `type()` returns data type.  | `type()` wa dēta no shurui o kaeshimasu |

---

## ✅ Summary for Instructors

- Students will likely enjoy this chapter — make it interactive!
- Let them try invalid string + int operations and understand errors.
- Use `input()` and `print()` to build mini programs and reinforce learning.
- Type conversion is key — use lots of small examples.
- Encourage exploring: "What happens if I try this?"

---