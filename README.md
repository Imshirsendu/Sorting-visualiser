# ⚡ Algorithm Visualizer -By shirsendu

> A powerful, interactive, and beautifully designed web application to visualize, compare, and learn computer science algorithms.

**Algorithm Visualizer - Pro** is a single-page web application (SPA) built entirely with vanilla HTML, CSS, and JavaScript. It provides a deep, interactive learning experience for data structures and algorithms, featuring everything from standard sorting animations to a custom domain-specific language (DSL) for visualizing your own code.

---

## ✨ Key Features

- 📊 **Interactive Visualization:** Watch algorithms sort data in real-time with customizable speed controls, play/pause functionality, and live metrics (comparisons, swaps).
- ⚖️ **Compare Mode:** Run two different sorting algorithms side-by-side on the exact same dataset to visually compare their speeds and efficiency.
- 🔍 **Deep Dive (PRO):** A step-by-step interactive mode that breaks down the algorithm's micro-steps. Features active code line highlighting, pointer tracking, and plain-English insights for every single operation.
- 🗺️ **Pathfinding Arena (NEW):** Grid-based pathfinding visualizer. Draw walls, set start/end points, and generate mazes. Watch BFS, DFS, Dijkstra, and A* explore the grid.
- 🛠️ **Custom DSL (PRO):** Write your own sorting algorithms using a built-in Domain Specific Language. Use commands like `compare(i, j)` and `swap(i, j)` and watch the visualizer animate your custom logic instantly!
- 📚 **Code Library:** A built-in reference library containing clean, syntax-highlighted code snippets for all algorithms. You can even run tests on the snippets directly in the browser.
- 🌗 **Modern UI/UX:** A stunning Glassmorphism design system with responsive layouts and a seamless Light/Dark mode toggle.

---

## 🧮 Supported Algorithms

### Sorting
1. **Bubble Sort** (O(n²))
2. **Selection Sort** (O(n²))
3. **Insertion Sort** (O(n²))
4. **Merge Sort** (O(n log n)) - *Includes Auxiliary Memory / Heap visualizer*
5. **Quick Sort** (O(n log n))
6. **Heap Sort** (O(n log n))
7. **Shell Sort** (O(n log n))
8. **Radix Sort** (O(nk))
9. **Counting Sort** (O(n+k))
10. **Cocktail Shaker Sort** (O(n²))

### Pathfinding
1. **Breadth-First Search (BFS)** - *Unweighted, guarantees shortest path*
2. **Depth-First Search (DFS)** - *Unweighted, does not guarantee shortest path*
3. **Dijkstra's Algorithm** - *Weighted, guarantees shortest path*
4. **A* Search (A-Star)** - *Weighted with Manhattan heuristic, guarantees shortest path*

---

## 🚀 Getting Started

This project is built to be as simple and accessible as possible. There are **no build steps, no dependencies, and no package managers** required.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/yourusername/algorithm-visualizer-pro.git](https://github.com/yourusername/algorithm-visualizer-pro.git)

## 💻 Tech Stack

* **HTML5:** Semantic structure.
* **CSS3:** Advanced styling using CSS Variables, Flexbox, CSS Grid, and Glassmorphism techniques (`backdrop-filter`).
* **Vanilla JavaScript (ES6+):** Complete application logic, DOM manipulation, asynchronous animations (`async/await`, `Promises`), and dynamic DSL parsing/execution.
* **HTML Canvas:** Used for rendering the live theoretical vs actual complexity charts.

---

## 🧠 Custom DSL Quick Start

Want to visualize your own algorithm? Navigate to the **Custom DSL** tab and use the built-in variables and functions:

* `n` - Length of the array.
* `compare(i, j)` - Compares elements at index `i` and `j`. Returns `> 0` if `arr[i] > arr[j]`. Triggers highlight animation.
* `swap(i, j)` - Swaps elements at index `i` and `j`. Triggers swap animation.
* `get(i)` - Reads the value at index `i`.
* `set(i, value)` - Overwrites the value at index `i`. Triggers overwrite animation.

**Example (Custom Selection Sort):**

```javascript
for (let i = 0; i < n - 1; i++) {
  let minIdx = i;
  for (let j = i + 1; j < n; j++) {
    if (compare(j, minIdx) < 0) {
      minIdx = j;
    }
  }
  if (minIdx !== i) swap(i, minIdx);
} 
```
## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
If you want to add a new algorithm or improve the UI:

1. Fork the project.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

---

## 📄 License

This project is open-source and available under the MIT License.

---
*Built with ❤️ and passion by Shirsendu*
