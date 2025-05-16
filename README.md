ZA25 Quantum Communication Simulation
This repository contains the implementation of a quantum communication simulation inspired by the ZA25 protocol, developed by the Centre of Excellence for Technology Quantum and AI (CETQAC). The project achieves a 100 km repeater-enhanced simulation with a fidelity of 0.9950, real-time 10-bit transmission of the message "10" with a fidelity of 0.946, and 100% shot accuracy. Built using Qiskit and IBM Quantum's Noisy Intermediate-Scale Quantum (NISQ) devices, this simulation demonstrates advancements in Quantum Secure Direct Communication (QSDC).
Features

Simulates a 100 km quantum repeater network with a mitigated fidelity of 0.9950.
Executes real-time 10-bit quantum message transmission with a fidelity of 0.946.
Achieves 100% shot accuracy using M3 error mitigation techniques.
Runs on IBM Quantum's ibm_sherbrooke device or compatible backends.
Includes data analysis and visualization tools for fidelity and accuracy metrics.

Prerequisites

Python 3.8 or higher
Qiskit 0.44 or later (pip install qiskit)
An IBM Quantum account (Sign up)
Optional: NumPy and Matplotlib for data analysis and visualization
Git for version control

Installation

Clone the repository:git clone https://github.com/your-username/za25-simulation.git
cd za25-simulation


Set up a virtual environment and install dependencies:python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt


Configure IBM Quantum credentials:
Obtain your API token from IBM Quantum.
Save it in ~/.qiskit/qiskitrc or set it programmatically in simulation.py.



Usage
To run the 100 km repeater-enhanced simulation:
python simulation.py --distance 100 --repeater --fidelity-target 0.9950

To execute the real-time 10-bit transmission:
python transmission.py --message "10" --device ibm_sherbrooke

Results, including fidelity and shot accuracy metrics, are saved in the results/ directory as CSV files and visualizations.
File Structure

simulation.py: Main script for the 100 km repeater-enhanced simulation.
transmission.py: Script for real-time 10-bit quantum message transmission.
utils/: Helper functions for error mitigation and data processing.
error_mitigation.py: M3 error mitigation implementation.
data_processing.py: Tools for analyzing simulation outputs.


results/: Output files (e.g., output.csv, plots/fidelity_plot.png).
requirements.txt: List of Python dependencies.
config.yaml: Simulation parameters (e.g., distance, device).
demo.ipynb: Jupyter notebook demonstrating the simulation workflow.
tests/: Unit tests for validating simulation scripts.

Results

Repeater Simulation: 100 km distance, Fidelity = 0.9950, Shot Accuracy = 100%.
Real-Time Transmission: 10-bit message "10", Fidelity = 0.946, Shot Accuracy = 100%.
Detailed metrics and visualizations are available in results/output.csv and results/plots/.

Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a feature branch (git checkout -b feature/your-improvement).
Commit your changes (git commit -m "Add new feature").
Push to the branch (git push origin feature/your-improvement).
Open a pull request on GitHub.

Please follow the Contributing Guidelines for more details.
License
This project is licensed under the MIT License - see the LICENSE file for details.
Acknowledgments

Built with Qiskit and IBM Quantum's NISQ devices.
Inspired by the ZA25 protocol (ResearchSquare Preprint).
Thanks to CETQAC for pioneering advancements in QSDC.
Gratitude to the open-source quantum computing community.

Contact
For questions or feedback, please open an issue on GitHub or contact info@thecetqap.com 
