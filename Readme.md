# 🍩 Spinning Donut Animation

**An ASCII-based spinning donut animation** made in C++! This project offers a mesmerizing effect that rotates endlessly in your terminal using creative ASCII art, trigonometry, and a simple looping algorithm.

### Steps to Run

1. Clone the repository or copy the code to a local file, say `donut.cpp`.
2. Open your terminal and navigate to the directory containing `donut.cpp`.
3. Compile the code with:

   ```bash
   g++ donut.cpp -o donut -lm
   ```

4. Run the compiled program:

   ```bash
   ./donut
   ```

## 🎨 Custom Patterns

This donut includes several ASCII patterns to enhance its effect. Uncomment one of the patterns below and recompile to see the changes:

```cpp
// b[o] = "JackEatDonut"[N > 0 ? N : 0];
// b[o] = "====o===="[N > 0 ? N : 0];
// b[o] = "O O O O O"[N > 0 ? N : 0];
// b[o] = "###===###"[N > 0 ? N : 0];
// b[o] = "@@@@@@@@"[N > 0 ? N : 0];
// b[o] = "(((  )))"[N > 0 ? N : 0];
// b[o] = "===000==="[N > 0 ? N : 0];
// b[o] = "~~~~~~~"[N > 0 ? N : 0];
// b[o] = "  0 0  "[N > 0 ? N : 0];
// b[o] = "  OOO  "[N > 0 ? N : 0];
```

Simply replace the line:

```cpp
b[o] = ".,-~:;=!*#$@"[N > 0 ? N : 0];
```

with any of the lines above, recompile, and run the animation again.

## 🛠️ How It Works

The program uses trigonometric functions to compute points in a 3D space, then projects them into 2D ASCII characters. Each frame is redrawn with slight rotation increments (A and B variables) to simulate a spinning effect.

### Main Logic Overview

1. **Trigonometric Projection**: Uses sin and cos functions to project points in a rotating donut shape.
2. **Buffer Refreshing**: Continuously updates the terminal screen with new frames, creating an animated effect.
3. **Sleep Cycle**: Adjust `usleep(30000);` to control the animation speed (lower for faster spin, higher for slower).

## 🔧 Modifications

You can change the animation speed by modifying the `usleep` parameter. For example, `usleep(10000);` will make it faster.

---

## 📜 Note

This project is not my original work. I have added some ASCII templates to give a cooler animation effect, making it a fun, customizable donut animation! 😊 Feel free to fork, modify, and use it however you like!

Enjoy the spin! 🍩✨

--- 
