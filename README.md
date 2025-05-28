✈️ Air Traffic Control (ATC) Simulation System
Welcome to the ATC Simulation System, a C++-based project designed to simulate the operations of an air traffic control system. This project manages aircraft scheduling, runway operations, flight phases, and violation monitoring, all while providing a visual representation using SFML. Created as of May 28, 2025, this system demonstrates multi-threading, inter-process communication, and real-time simulation.

🚀 Project Overview
The ATC Simulation System models the activities of an airport, including:

Flight Scheduling: Manages arrivals and departures with priority-based scheduling.
Runway Operations: Simulates runway usage for takeoffs and landings, ensuring proper allocation.
Aircraft Phases: Tracks various flight phases (e.g., taxiing, taking off, cruising).
Violation Monitoring: Detects and logs violations (e.g., speed, altitude) and issues fines.
Visualization: Provides a graphical interface using SFML to visualize aircraft movements on runways.

The system is composed of multiple C++ files, each handling specific components, and a shell script to run them in separate terminals.

🛠️ Features

Multi-Threaded Architecture: Utilizes POSIX threads for concurrent flight operations.
Inter-Process Communication: Uses named pipes (FIFOs) for communication between ATC and violation subsystems.
Graphical Interface: Displays aircraft movements on runways using SFML.
Violation System: Automatically detects rule violations and generates fines.
Runner Script: Automates compilation and execution of all components in separate terminals.


📂 Project Structure
The project consists of the following key files:

atc2.cpp: Core ATC simulation logic, including flight scheduling, runway management, and visualization.
file1.cpp: Handles aircraft phase simulations (placeholder name; replace with your actual file).
file2.cpp: Manages violation detection and fine generation (placeholder name; replace with your actual file).
file3.cpp: Oversees airline and aircraft data (placeholder name; replace with your actual file).
run_all.sh: Shell script to compile and run all .cpp files in separate terminals.

Directory Structure
ATC-Simulation/
│
├── atc.cpp             # Main ATC simulation with SFML visualization
├── stripepay.cpp       # stripe payment manager simulation
├── avn.cpp             # Violation detection and fines
├── airline-portal.cpp  # Airline and aircraft management
├── run_all.sh          # Runner script for compilation and execution (not implemented)
├── runway.png          # Runway image for SFML visualization
├── plane2.png          # Plane image for SFML visualization
├── ARIAL.TTF           # Font file for SFML text rendering
└── README.md           # Project documentation


⚙️ Prerequisites
Before running the project, ensure you have the following installed:

C++ Compiler: g++ (GNU Compiler Collection)
SFML Library: For graphical visualization
Install on Ubuntu: sudo apt-get install libsfml-dev
Install on macOS: brew install sfml


POSIX-Compatible System: Linux or macOS (Windows may require WSL or adjustments)
Terminal Emulator: gnome-terminal (Ubuntu) or xterm for the runner script
Install gnome-terminal: sudo apt-get install gnome-terminal
Install xterm: sudo apt-get install xterm

🏁 Getting Started
Follow these steps to set up and run the project:

Clone the Repository (if hosted on GitHub or similar):
git clone <repository-url>
cd ATC-Simulation


Ensure Required Files:

Place runway.png, plane2.png, and ARIAL.TTF in the project directory (required for SFML visualization).
Verify that all .cpp files and run_all.sh are present.


Make the Runner Script Executable:
chmod +x run_all.sh


Run the Project:

Execute the runner script to compile and run all components in separate terminals:./run_all.sh


This will:
Compile each .cpp file using g++.
Launch each executable in a new terminal window.
Keep terminals open until you press Enter.




Interact with the Simulation:

Observe the graphical window (via SFML) showing aircraft movements on runways.
Monitor terminal outputs for flight status, violations, and logs.




📸 Screenshots
Simulation Window
![My Image]("AirTrafficControlSystem\Saud_Ur_Rahman_23i-0540_Hadi_Wasim_23f-0681\Saud_Ur_Rahman_23i-0540_Hadi_Wasim_23f-0681\runway.png")
Terminal Outputs
![My Image]("AirTrafficControlSystem\Saud_Ur_Rahman_23i-0540_Hadi_Wasim_23f-0681\Saud_Ur_Rahman_23i-0540_Hadi_Wasim_23f-0681\Screenshot2025-05-28220800.png")


🧑‍💻 Usage

Graphical Interface: The SFML window displays three runways (RWY-A, RWY-B, RWY-C) with aircraft movements.
RWY-A: For arrivals.
RWY-B: For departures.
RWY-C: For cargo, emergencies, and overflow.


Terminals:
Each terminal shows logs for a specific component (e.g., flight scheduling, violations).
Press Enter in each terminal to close it after the simulation ends.


Violations:
Speed, altitude, and position violations are logged and fines are issued automatically.
Check the terminal running the violation component for details.




🛠️ Customization

Adjust Flight Phases: Modify simDepart() and simArrive() in atc2.cpp to change phase durations (e.g., increase sleep() values).
Change Visualization Speed: In sfmlRender(), adjust the plane movement speed by modifying the division factor (e.g., speed / 3000.0f).
Add More Aircraft: Update the generateAircrafts() method in atc2.cpp to include additional aircraft.
Modify Runway Logic: Edit the Runway class to change allocation rules.


📝 Notes

Performance: The simulation uses multi-threading, so ensure your system supports POSIX threads.
Dependencies: Missing SFML or font/image files will cause the program to fail. Ensure all prerequisites are met.
Terminal Emulator: If gnome-terminal is unavailable, edit run_all.sh to use xterm or another terminal emulator (e.g., open -a Terminal on macOS).


🤝 Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch (git checkout -b feature/your-feature).
Make your changes and commit (git commit -m "Add your feature").
Push to the branch (git push origin feature/your-feature).
Open a pull request.


📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

📅 Project Timeline

Created: May 28, 2025, at 10:00 PM PKT
Last Updated: May 28, 2025


📧 Contact
For questions or feedback, reach out to the project maintainers:

Email: hadiwasim644@gmail.com
GitHub: Hadi-Wasim


Happy simulating! 🛫
