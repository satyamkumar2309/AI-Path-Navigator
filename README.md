# AI-Path-Navigator

AI Path Navigator (A Pathfinding)*

An intelligent, graph-based navigation system designed for Societies . This project uses the A* Search Algorithm to find optimal walking paths, accounting for real-world factors like stairs, terrain quality, and accessibility.

Overview

Navigating large, developing campuses can be a challenge. Standard mapping tools often lack the granular detail of internal walking paths or fails to distinguish between a flat walkway and a  staircase. AI Path Navigator transforms a physical campus layout into a digital State-Space Search Graph. By applying a cost-sensitive search, it provides users with the most efficient Path based on their specific needs (e.g., avoiding stairs for heavy luggage or seeking them out for athletic training).

AI Concepts Applied

Graph Theory: Society Campus landmarks are represented as Nodes, and walkways as Weighted Edges. Informed Search (A*): Utilizes the evaluation function f(n) = g(n) + h(n). Admissible Heuristic: Employs Euclidean Distance to ensure the path found is always mathematically optimal. Cost Functions: Dynamically adjusts edge weights based on "Surface Factors" (e.g., a 1.5x multiplier for stairs).

Tech Stack

Language: Python 3.xGraph Library: NetworkX (Robust graph manipulation and pathfinding)

Visualization: Matplotlib (Spatial plotting and UI)

Math: Python math module for heuristic calculations.

 Society Campus Map Nodes The system currently maps 16 key locations including:

Administrative: Main Entrance, Office Block, Society Office, Meeting Area.

Residents: Food Court, Market Area, Community Hall, Fitness Center.

Residential: Tower A, B, C, and D.

Recreational: PlayGround, Club House, Health Center.

Results

The algorithm generates a visual map where:

Gray Circles: Represent Society Campus landmarks.

Black Lines: Represent standard flat paths.

Grey/Red Overlay: Highlights the calculated optimal route.

Distance Calculation: Provides the total weighted distance in meters in the window title.

**How to Run the Project**

Follow these steps to set up the environment and execute the navigator on your local machine.

Prerequisites
Ensure you have Python 3.7 or higher installed. You can check your version by running: python --version

Clone the Repository
Download the project files to your local system: git clone https://github.com/satyamkumar2309/AI-Path-Navigator cd AI-Path-navigator

Install Required Libraries
This project relies on NetworkX for graph logic and Matplotlib for the GUI. Install them via pip: pip install networkx matplotlib

Execute the Script
Run the main Python file to launch the visual navigator: https://github.com/devesh18-design/Smart-Campus-Navigator/blob/main/Smart%20university%20navigator.py

Interacting with the OutputThe Map Window: A window titled "AI Path Navigator by Satyam Kumar" will appear.

The Visualization:

Grey Nodes: Your calculated path.

Red Edges: The specific route chosen by the A* algorithm.

Lightgreen Nodes: Other available campus landmarks.

Console Output: The terminal will print the step-by-step route
