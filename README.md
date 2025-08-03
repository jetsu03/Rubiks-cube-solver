# Rubik’s Cube Solver – Web Application
Python & C Web App | High-Performance Solver

### Project Overview
This project is a high-performance 3x3 Rubik's Cube solver that combines a powerful C-based backend with an intuitive web interface built using Python and Flask. The application allows users to input any scrambled cube configuration and receive an efficient, step-by-step solution. The solver visualizes the entire process on a 3D interactive cube, making it an excellent tool for both learning and analysis. This application was designed to provide a fast and accessible way to solve a Rubik's Cube, mimicking real-world logic through a sequence of valid moves displayed in a user-friendly format.

### Technologies Used

| Tool / Language | Purpose                               |
| :-------------- | :------------------------------------ |
| **C** | Core cube-solving logic (for speed)   |
| **Python** | Backend web server and logic          |
| **Flask** | Web framework                         |
| **HTML/CSS/JS** | Interactive 3D frontend and UI        |
| **Numpy** | Data manipulation in the Python backend |

### Folder Structure

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

### Installation & Usage

**Prerequisites**

  * Python 3
  * `pip` (Python package installer)
  * A C Compiler (like GCC) is required if you want to modify and recompile the C source code.

**Run the Web Application**

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

### Screenshot Gallery

This section showcases the application's interface. These examples help visualize how the solver works.

| Type                      | Screenshot                                       |
| :------------------------ | :----------------------------------------------- |
| **🎨 CLI Interface** | ![image alt](https://github.com/jetsu03/Rubiks-cube-solver/blob/main/CLI.jpg?raw=true)        |
| **📝 Scramble & Solution** | ![image alt](https://github.com/jetsu03/Rubiks-cube-solver/blob/main/Main_screen.jpg?raw=true) |

### Demo Video
A brief video demonstrating the web interface in action.
https://github.com/user-attachments/assets/8e2e3b3d-2ec5-44c3-a8bc-9c38bb9d9ab9
