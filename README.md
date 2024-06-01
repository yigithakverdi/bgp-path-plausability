# BGP Path Plausibility

## Overview
Welcome to the BGP Path Plausibility project! This repository focuses on enhancing path plausibility algorithms to improve the security of the Border Gateway Protocol (BGP). The project aims to address existing limitations and propose innovative solutions to mitigate BGP prefix hijacking, route leaks, and forged-origin prefix hijacks.

## Objectives
- **Enhance Path Plausibility Algorithms:** Improve the efficiency and accuracy of ASPA and AS-Cones algorithms.
- **Develop Hybrid Algorithms:** Create hybrid algorithms combining the strengths of ASPA and AS-Cones.
- **Simulation and Analysis:** Test new algorithms in a detailed simulation environment and compare them with existing ones.
- **Deployment Strategies:** Develop optimized deployment strategies to maximize the benefits of the new algorithms.
- **Security Evaluation:** Assess the security improvements offered by the new algorithms against various attack vectors.

## File Structure
The repository is organized as follows:
```
bgp-path-plausability/
│
├── docs/
│ ├── literature_review.md # Comprehensive review of existing BGP security literature
│ ├── algorithm_design.md # Detailed description of algorithm enhancements and hybrid algorithms
│ ├── deployment_guide.md # Guide for deploying the enhanced algorithms
│ └── security_assessment.md # In-depth evaluation of security performance
│
├── src/
│ ├── asp_enhanced.py # Implementation of the enhanced ASPA algorithm
│ ├── as_cones_enhanced.py # Implementation of the enhanced AS-Cones algorithm
│ ├── hybrid_algorithm.py # Implementation of the hybrid algorithm
│ └── utils.py # Utility functions for algorithm implementation
│
├── simulations/
│ ├── setup_environment.py # Script to set up the simulation environment
│ ├── run_simulations.py # Script to execute the simulations
│ ├── data/
│ │ ├── as_topology.json # AS topology model for simulations
│ │ └── bgp_updates.json # Real-world BGP update messages for testing
│ └── results/
│ ├── results_analysis.py # Analysis of simulation results
│ └── output/ # Directory to store simulation output data
│
├── tests/
│ ├── test_asp_enhanced.py # Unit tests for the enhanced ASPA algorithm
│ ├── test_as_cones_enhanced.py# Unit tests for the enhanced AS-Cones algorithm
│ ├── test_hybrid_algorithm.py # Unit tests for the hybrid algorithm
│ └── test_utils.py # Unit tests for utility functions
│
├── LICENSE # License information
├── README.md # Project overview and information
└── requirements.txt # List of dependencies
```


## Getting Started

### Prerequisites
- Python 3.8+
- Required Python packages listed in `requirements.txt`

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yigithakverdi/bgp-path-plausability.git
    cd bgp-path-plausability
    ```
2. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

### Running Simulations
1. Set up the simulation environment:
    ```bash
    python simulations/setup_environment.py
    ```
2. Run the simulations:
    ```bash
    python simulations/run_simulations.py
    ```

### Testing
Run unit tests to ensure everything is working correctly:
```bash
pytest tests/

