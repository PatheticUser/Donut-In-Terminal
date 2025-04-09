# **Spinning Donut Animation**

This is a **terminal-based spinning donut animation** written in C++. The project produces a mesmerizing rotating donut effect using ASCII characters, trigonometry, and a simple loop-driven rendering algorithm.

---

## **Steps to Run**

1. Clone the repository or copy the code into a local file, e.g., `donut.cpp`.
2. Open your terminal and navigate to the directory containing `donut.cpp`.
3. Compile the code with:

   ```bash
   g++ donut.cpp -o donut -lm
   ```

4. Run the compiled program:

   ```bash
   ./donut
   ```

---

## **Custom ASCII Patterns**

The donut shape can be enhanced using various ASCII character sets. To apply a custom pattern, replace the following line in the source code:

```cpp
b[o] = ".,-~:;=!*#$@"[N > 0 ? N : 0];
```

with any of the following alternatives (uncomment the desired line):

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

Recompile the code after modifying it to see the updated animation.

---

## **How It Works**

This animation leverages mathematical and programming techniques to simulate 3D rotation on a 2D terminal screen:

### Core Components:

1. **3D to 2D Projection**  
   Trigonometric functions (sine and cosine) are used to calculate the 3D coordinates of the donut shape, which are then projected onto a 2D grid of ASCII characters.

2. **Screen Buffer Update**  
   A character buffer is continuously refreshed to redraw each frame with updated rotation values, creating the illusion of spinning.

3. **Animation Timing**  
   The rotation speed is controlled by a delay function. You can modify `usleep(30000);` to speed up or slow down the animation. For example:
   - Faster spin: `usleep(10000);`
   - Slower spin: `usleep(50000);`

---

## **Modifications & Personalization**

- Adjust the rotation speed via the `usleep()` function.
- Swap out ASCII patterns to give the donut a unique look.
- Change terminal dimensions or font to enhance the visual appeal.

---

## **Disclaimer**

This is not an original creation. The base code was written by an anonymous developer as a demo of terminal graphics using ASCII and trigonometry. Minor enhancements have been made to allow customization through ASCII pattern templates, making it a more interactive and visually appealing experience.

If this project helped you, please consider giving it a **star** on GitHub, it motivates me to improve and share more cool stuff!

> Click on the 🌟 button at the top right of the repo. It takes 2 seconds and helps a lot!
