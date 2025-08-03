# 🧠 Rubik’s Cube Solver – Web Application

Python & C Web App | High-Performance Solver

### 🚀 Project Overview

This project is a high-performance 3x3 Rubik's Cube solver that combines a powerful C-based backend with an intuitive web interface built using Python and Flask. The application allows users to input any scrambled cube configuration and receive an efficient, step-by-step solution. The solver visualizes the entire process on a 3D interactive cube, making it an excellent tool for both learning and analysis.

This application was designed to provide a fast and accessible way to solve a Rubik's Cube, mimicking real-world logic through a sequence of valid moves displayed in a user-friendly format.

### 🎯 Key Features

🧩 **Dual Cube Input Modes**

  * **Scramble Algorithm Mode:**
      * Input a scramble using standard cube notation (e.g., `R U R' U'`).
      * Select from pre-defined patterns or apply your own scramble.
      * Watch the cube animate the scramble and the solution.
  * **Manual Color Input Mode:**
      * Manually assign colors to all 6 faces of the cube using an interactive color palette.
      * Click on the 3D cube's faces to input a real-world cube's state.
      * Apply the colors and proceed to the solution visualization.

🎞️ **Interactive Animation Controls**

  * **Playback:** Start, pause, step forward (`Next`), and step backward (`Prev`) through the solution animation.
  * **Speed Control:** Adjust the animation speed with a convenient slider.
  * **Move Display:** The sequence of moves for the current step is clearly displayed.

### 🛠️ Technologies Used

| Tool / Language | Purpose                               |
| :-------------- | :------------------------------------ |
| **C** | Core cube-solving logic (for speed)   |
| **Python** | Backend web server and logic          |
| **Flask** | Web framework                         |
| **HTML/CSS/JS** | Interactive 3D frontend and UI        |
| **Numpy** | Data manipulation in the Python backend |

### 📁 Folder Structure

```
rubiks-cube-solver/
├── bin/                    # Compiled binaries (solver executable and library)
│   ├── libcubesolver.dll
│   └── solver
│
├── data/                   # Algorithm data for OLL and PLL
│   ├── olls.csv
│   ├── plls.csv
│   └── patterns.csv
│
├── src/                    # C source code for the solver logic
│   ├── cross.c
│   ├── cube.c
│   ├── f2l.c
│   ├── lastlayer.c
│   ├── solver.c
│   ├── solver_library.c
│   └── utils.c
│
├── static/                 # Frontend assets (CSS, JS, images)
│   ├── cube.css
│   ├── cube.js
│   └── ...
│
├── templates/              # Flask HTML templates
│   └── cube.html
│
├── app.py                  # Main Flask application file
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

### 📥 Installation & Usage

🔧 **Prerequisites**

  * Python 3
  * `pip` (Python package installer)
  * A C Compiler (like GCC) is required if you want to modify and recompile the C source code.

🖥️ **Run the Web Application**

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/jetsu03/Rubiks-cube-solver.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd Rubiks-cube-solver
    ```
3.  **Install Python dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Run the Flask application:**
    ```bash
    python app.py
    ```
5.  Open your web browser and go to **[http://127.0.0.1:5000](https://www.google.com/search?q=http://127.0.0.1:5000)**.

### 📚 Notation Reference

Before using scramble input, familiarize yourself with the **standard Rubik’s Cube notation**:

| Notation | Meaning                     |
| :------- | :-------------------------- |
| **U** | Up face clockwise           |
| **U'** | Up face counter-clockwise   |
| **R**, **L** | Right / Left face           |
| **F**, **B** | Front / Back face           |
| **D** | Down face                   |
| **x, y, z** | Cube rotations |

### 📷 Screenshot Gallery

This section showcases the application's interface. These examples help visualize how the solver works.

| Type                      | Screenshot                                       |
| :------------------------ | :----------------------------------------------- |
| **🎨 Main Interface** | `![Main UI](path/to/your/screenshot.png)`        |
| **📝 Scramble & Solution** | `![Solution View](path/to/your/screenshot2.png)` |

### 🎨 Demo Video

A brief video demonstrating the web interface in action.

`[Link to your demo video or embed a GIF here]`
