# Radiation Penetration Simulation (OpenGL)

A Computer Graphics project developed using C++ and OpenGL (GLUT). This application simulates the penetration behavior of radioactive elements (Alpha, Beta, and Gamma rays) against various shielding materials (Paper, Aluminum, and Lead).

![Simulation Demo](screenshots/demo2.png)

## 📖 Project Overview

This tool offers a real-time, hands-on simulation to understand how different types of radiation interact with matter. It visualizes the sinusoidal motion of radiation particles and demonstrates their ability (or inability) to penetrate specific barriers.

📄 **[Read the Full Project Report](docs/projectReport.pdf)**

---

## 🚀 Features

- **Real-Time Simulation:** Visualize Alpha, Beta, and Gamma rays moving in sinusoidal patterns.
- **Interactive Shielding:** Users can dynamically place or remove shielding materials (Paper, Aluminum, Lead).
- **Educational Overlay:** On-screen instructions and labels for rays and molecules.

---

## 🛠️ Tech Stack & Requirements

**Software:**

- **Language:** C++
- **Graphics Library:** OpenGL (GLUT - OpenGL Utility Toolkit)

**Hardware:**

- **Processor:** Ryzen 5 5500U (or equivalent)
- **RAM:** 8GB recommended

---

## ⚙️ Installation & Setup

To run this project locally, you will need a C++ compiler (MinGW) and the GLUT library.

### Prerequisites

1.  **MinGW w64** (or any standard GCC compiler).
2.  **FreeGLUT** (MinGW version).

### Steps to Run (VS Code / Command Line)

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/MofakkarHM/Radiation-Penetration-Simulation.git](https://github.com/MofakkarHM/Radiation-Penetration-Simulation.git)
    cd Radiation-Penetration-Simulation
    ```
2.  **Setup GLUT:** Ensure `freeglut.dll` (or `glut32.dll`) is in the `src/` directory next to the executable.
3.  **Compile the code:**
    ```bash
    g++ src/main.cpp -o main -I"path/to/include" -L"path/to/lib" -lfreeglut -lopengl32 -lglu32
    ```
4.  **Run the application:**
    ```bash
    ./main.exe
    ```

---

## 🎮 Controls (How to Operate)

The simulation is controlled via the keyboard to activate or deactivate specific shielding walls.

| Action         | Shield Material | Key                  |
| :------------- | :-------------- | :------------------- |
| **Activate**   | **Paper**       | `Left Arrow` (`<-`)  |
| **Activate**   | **Aluminum**    | `Down Arrow`         |
| **Activate**   | **Lead**        | `Right Arrow` (`->`) |
| **Deactivate** | **Paper**       | `End`                |
| **Deactivate** | **Aluminum**    | `Page Up`            |
| **Deactivate** | **Lead**        | `Page Down`          |
| **Exit**       | N/A             | `n`                  |

---

## 🧪 Simulation Logic

### Radiation Types

1.  **Alpha Ray:** Low penetration power. Stopped by Paper.
2.  **Beta Ray:** Medium penetration power. Passes Paper, stopped by Aluminum.
3.  **Gamma Ray:** High penetration power. Passes Paper and Aluminum, stopped by Lead.

---

## 👨‍💻 Author

**Mir Md. Mofakkar Hossain (Mahim)**

- **GitHub:** [MofakkarHM](https://github.com/MofakkarHM)
- **LinkedIn:** [Mir Md Mofakkar Hossain](https://www.linkedin.com/in/mofakkarhossain/)

---

## 📚 References

1.  [OpenGL Official Site](https://www.opengl.org/)
2.  [Radiation Penetration Science](https://sciencedemonstrations.fas.harvard.edu/presentations/%CE%B1-%CE%B2-%CE%B3-penetration-and-shielding)
