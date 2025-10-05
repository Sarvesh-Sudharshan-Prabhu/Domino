# 🁢 Domino (Java)

A simple Java program that models a **Domino tile**, supporting number comparison, equality checking, and reveal state management.

---

## 📂 Project Structure
```
Domino-main/
└── DominoCSA.java
```

---

## 🧩 Overview
The `Domino` class represents a standard domino tile with two sides — `top` and `bottom`.  
It allows users to create, compare, and reveal dominoes, making it useful for simulations or educational programming exercises.

---

## 🧠 Core Class: `Domino`

### Constructor
```java
public Domino(int x, int y)
```
Creates a new domino tile.  
- The smaller of `x` and `y` becomes the **top** value.  
- The larger becomes the **bottom** value.

### Methods
| Method | Description |
|--------|--------------|
| `int getTop()` | Returns the top value of the domino. |
| `int getBottom()` | Returns the bottom value of the domino. |
| `boolean isRevealed()` | Checks whether the domino has been revealed. |
| `void setRevealed(boolean revealed)` | Sets the reveal state of the domino. |
| `boolean equals(Domino other)` | Returns `true` if both dominos have the same top and bottom values. |

---

## 🧪 Example Usage
```java
public class Main {
    public static void main(String[] args) {
        Domino d1 = new Domino(3, 6);
        Domino d2 = new Domino(6, 3);

        System.out.println("Domino 1: " + d1.getTop() + "|" + d1.getBottom());
        System.out.println("Domino 2: " + d2.getTop() + "|" + d2.getBottom());

        System.out.println("Are they equal? " + d1.equals(d2));

        d1.setRevealed(true);
        System.out.println("Is Domino 1 revealed? " + d1.isRevealed());
    }
}
```

### Sample Output
```
Domino 1: 3|6
Domino 2: 3|6
Are they equal? true
Is Domino 1 revealed? true
```

---

## ⚙️ How to Run

1. Ensure **Java (JDK 8+)** is installed.  
2. Save `DominoCSA.java` and (optionally) `Main.java` in the same folder.  
3. Compile and run using:
   ```bash
   javac DominoCSA.java Main.java
   java Main
   ```

---
