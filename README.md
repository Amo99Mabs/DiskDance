# 🩰 DiskDance

DiskDance is a Python-based simulation of the classic **Tower of Hanoi** puzzle, creatively solved using recursion. Watch as disks "dance" across rods in a logical sequence, demonstrating elegant algorithmic movement.

---

## ⚙️ Features

- Recursive solution to the Tower of Hanoi problem
- Real-time visualization of rod states after each move
- Configurable number of disks
- Clear and simple structure using Python lists

---

## 📜 How It Works

1. **Setup**:
   - `NUMBER_OF_DISKS` sets how many disks are used
   - Rods are represented by Python lists: `A` (source), `B` (auxiliary), and `C` (target)

2. **Recursive Function**:
   ```python
   def move(n, source, auxiliary, target):
       if n <= 0:
           return
       move(n - 1, source, target, auxiliary)
       target.append(source.pop())
       print(A, B, C, '\n')
       move(n - 1, auxiliary, source, target)
   ```

3. **Execution**:
   ```python
   NUMBER_OF_DISKS = 5
   A = list(range(NUMBER_OF_DISKS, 0, -1))
   B = []
   C = []
   move(NUMBER_OF_DISKS, A, B, C)
   ```

Each move prints the current state of the rods, giving you a step-by-step view of the puzzle being solved.

---

## 🧠 Learnings

- 📚 How recursion simplifies complex, layered logic
- 🎯 Function call stacks and base conditions
- 🧩 Efficient use of memory and data structures

---

## 🔮 Ideas for Future Enhancements

- Add a GUI using `tkinter` or `pygame` to animate disk movement
- Count and display total moves made
- Represent disks with icons or emojis for visual clarity 🥏
- Add command-line arguments for customizable runs

---

## 🙌 Credits

Crafted with logic and rhythm by [Amogelang](https://github.com/Amo99Mabs).  
A recursive journey wrapped in simplicity and elegance.

---

## 🐍 Requirements

- Python 3.x

No external libraries needed.

---

## 🚀 Getting Started

Clone the repo and run:

```bash
python diskdance.py
```

Want help designing a logo or adding a badge for the project? I’d love to collaborate more on this! 😄
