This section introduces the Python REPL and how students can use it for quick experimentation. Instructors can support students by modeling mistakes, clarifying keyboard behavior, and making REPL feel like a safe place to “try stuff and break it.”

---
## 🗂️ Mini Table of Contents

- [[#🧩 REPL Basics]]
- [[#💡 When is the REPL Useful?]]
- [[#⚙️ Advice for Using the REPL]]

## 🧩 REPL Basics

> 💡 The REPL is like a live sandbox for testing one line of Python at a time.

### ✅ Key Concepts
- The REPL starts with `python` in the terminal.
- Shows `>>>` prompt when active.
- Commands like `quit()`, `help()`, and `dir()` must include parentheses.
- Up/down arrow keys cycle through command history.
- `Ctrl + C` = stop execution (not copy!).

### ⚠️ Common Issues
- Typing `quit` instead of `quit()` does nothing.
- Students forget `()`, especially for `help` and `dir`.
- Confuse `Ctrl + C` with copying, when it’s actually for interrupting.
- Don’t realize indentation matters even in REPL.
- Don’t know how to paste or clear output.

### 🧑‍🏫 Instructor Tips

#### 🖥️ Live Demo Steps:
1. Open terminal → type:
   ```bash
   python
   ```
2. Show the prompt:
   ```python
   >>>
   ```
3. Type the following:
   ```python
   help
   help()
   dir()
   quit()
   ```

4. Type:
   ```python
   while True:
       print("looping")
   ```
   Then press `Ctrl + C` to interrupt.

5. Demo copy/paste properly:
   - ✅ Windows/Linux: `Ctrl + Shift + C`, `Ctrl + Shift + V`
   - ✅ Mac: `Cmd + C`, `Cmd + V`
   - ❌ `Ctrl + C` alone = KeyboardInterrupt

---

### 📣 Japanese Phrases (REPL Basics)
| Japanese                     | English                                 | Romaji                            |
| ---------------------------- | --------------------------------------- | --------------------------------- |
| Pythonを1行ずつ試せます。             | You can test Python one line at a time. | Python o ichigyō zutsu tamesemasu |
| `()`を忘れないでください。              | Don’t forget the parentheses.           | `()` o wasurenaide kudasai        |
| `Ctrl + C` はコピーではありません。      | Ctrl+C is not for copy.                 | Ctrl + C wa kopī dewa arimasen    |
| コピーは `Ctrl + Shift + C` です。  | Copy is Ctrl + Shift + C.               | kopī wa Ctrl + Shift + C desu     |
| ペーストは `Ctrl + Shift + V` です。 | Paste is Ctrl + Shift + V.              | pēsto wa Ctrl + Shift + V desu    |

---

## 💡 When is the REPL Useful?

> Use REPL like a scratchpad: fast testing, immediate feedback.

### ✅ Best Use Cases
- Trying out one-liners
- Testing different encodings or syntax
- Debugging parts of a larger script
- Exploring modules or variables

### ⚠️ Common Issues
- Students may not realize it's **temporary** (data lost on close)
- Trying to use REPL like a full editor
- Confusion about current working directory

### 🧑‍🏫 Instructor Activity
Demo this scenario:
```python
with open('mystery_file.txt', 'r', encoding='shift_jis') as f:
    print(f.readlines())
```
Then:
- Press ↑ to restore line
- Change encoding and rerun

---

### 📣 Japanese Phrases (REPL Utility)
| Japanese | English | Romaji |
|----------|---------|--------|
| スクリプトを書く前にテストできます。 | You can test before writing a script. | sukiriputo o kaku mae ni tesuto dekimasu |
| 今いるフォルダにファイルを書きます。 | Files will be written in the current folder. | ima iru foruda ni fairu o kakimasu |

---

## ⚙️ Advice for Using the REPL

> REPL is fast and helpful — but it’s also volatile and not persistent.

### ⚠️ Common Pitfalls
- Forgetting that variables disappear after quitting
- Trying to copy/paste with the wrong shortcuts
- Indentation errors when writing loops or functions
- Losing progress if not saved to `.py` file

### 🧑‍🏫 Instructor Suggestions
- Tell students: “If it works in REPL, move it into your script.”
- Print copy/paste cheat sheet on board or slides.
- Practice intentional indentation errors:
  ```python
  for i in range(3):
  print(i)   # Error
  ```

---

### 📣 Japanese Phrases (REPL Advice)
| Japanese | English | Romaji |
|----------|---------|--------|
| 間違えても大丈夫です。 | It’s okay to make mistakes. | machigaete mo daijōbu desu |
| 結果がすぐに見えます。 | You see results immediately. | kekka ga sugu ni miemasu |
| REPLは保存されません。 | REPL is not saved. | REPL wa hozon saremasen |
| インデントに気をつけてください。 | Be careful with indentation. | indento ni ki o tsukete kudasai |

---

## ✅ Summary for Instructors

- REPL is **interactive and fast**, but **not permanent**
- Students will forget parentheses and indentation — let them!
- Model mistakes and help them recover → builds confidence
- Keep copy/paste + exit shortcuts visible in class
- Emphasize REPL = test lab, not final project

```python
# Remember:
#   quit()        = exit REPL
#   help()        = get help
#   dir()         = list variables/functions
#   Ctrl + C      = interrupt execution
```