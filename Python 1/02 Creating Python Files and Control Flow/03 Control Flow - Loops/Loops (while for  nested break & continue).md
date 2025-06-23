
**![](file:///C:/Users/NAVEED~1/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png)**

**1.**      **Use real life examples**

a.      A cat chases a pointer **_while_** it has energy
```python
energy = 3

while energy > 0:
    print("🐱 Zoom! The cat chases the laser!")
    energy -= 1

print("😴 The cat flops on the floor. Done.")
```

b.      **_For_** every student in class, say “Good Morning!”
```python
students = ["Aki", "Ken", "Yui", "Mao"]

for student in students:
    print(f"Good Morning, {student}! 🌞")
```

c.      **Nested loops:** Use a multiplication table (9 x 9 table  ) 
		i. Outer loop controls rows 
		ii. Inner loop controls columns**
	
```python
	for i in range(1,9): #outer loop : 9 rows
       for j in range(1,9): #inner loop: 9 columns
                      print(f”{i} x {j} = {i*j}”)
       print() # prints a blank line between rows
```
d.      **Break/Continue : skip/stop like games**

                                                                          **i.**      If it rains, we **break(stop)** the game

                                                                        **ii.**      If I’m tired, I’ll **skip** the gym — but still do the rest of my day.”

|   |   |
|---|---|
|activities = ["breakfast", "gym", "work", "dinner"]<br><br>for activity in activities:<br><br>if activity == "gym":<br><br>print("I'm tired... skipping the gym.")<br><br>continue<br><br>print(f"Doing: {activity}")|Doing: breakfast<br><br>I'm tired... skipping the gym.<br><br>Doing: work<br><br>Doing: dinner|