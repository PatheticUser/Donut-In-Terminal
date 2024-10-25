Floating Donut 🍩

Ever thought donuts and C++ could make a mesmerizing combo? This C++ program brings an animated, rotating donut right into your terminal, with a unique ASCII twist. Inspired by the genius behind the original donut animation, this project merges trigonometry and ASCII art for a hypnotic effect. 🚀


---

🔍 How It Works

The animation uses sine and cosine functions to calculate points on a 3D torus, projecting them onto a 2D plane. This method creates depth and shading, making the donut appear as if it's rotating in real-time.

🔢 Math Breakdown

Sine & Cosine: These functions drive the rotation, calculating angles for each point on the donut.

Depth Mapping: Shading is achieved by evaluating each point’s angle relative to a light source.

ASCII Art: Different symbols (.,-~:;=!*#$@) depict depth by altering brightness/shade. Plus, you can choose from extra designs for a custom donut vibe! 🖌️



---

🍩 ASCII Donut Toppings 🍩

Uncomment any line in the code to customize the donut “frosting”:

Classic: .,-~:;=!*#$@

Goofy: "AshEatDonut"

Chill Waves: "~~~~~~~"

Cool Rings: "###===###"

Binary Donut: "O O O O O"

Cosmic Donut: "(((  )))"

Monochrome: "  OOO  "



---

🚀 How to Run

1. Compile the Code

g++ donut.cpp -o donut -lm


2. Run the Executable

./donut



Ensure your terminal supports ANSI escape codes for the best experience!


---

🧑‍🎤 Credits

A nod to the original creator of this legendary donut animation! It’s a joy to bring it to life again in C++.

