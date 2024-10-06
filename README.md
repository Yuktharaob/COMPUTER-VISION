Shadow Simulation with Multiple Point Light Sources
This repository contains a Python implementation that simulates the shadow intensity on a plane, cast by an occluder, under multiple point light sources. It uses NumPy for mathematical computations and Matplotlib for visualization.

Features
Shadow Intensity Calculation: The code computes the shadow intensity on a 2D plane due to a square occluder.
Multiple Light Sources: You can adjust the number of point light sources to observe how the shadow changes (sharp with fewer sources and softer with more).
Visualization: The results are plotted using matplotlib to compare the shadow intensity patterns for different numbers of point light sources.
Prerequisites
To run the code, you need Python installed with the following libraries:

numpy
matplotlib
You can install the necessary dependencies with:

bash
Copy code
pip install numpy matplotlib
How It Works
Occluder and Plane Setup:

The occluder is centered at a specified point, and its size is configurable.
A 2D plane, where the shadow will be projected, is set up at a specified resolution.
Multiple Point Light Sources:

The light sources are arranged in a grid around the occluder, and the user can configure the number of light sources.
For each light source, the code calculates the shadow cast by the occluder at each point on the plane.
Shadow Calculation:

For each pixel on the plane, the code checks if it falls within the shadow of the occluder based on the position of the light sources.
The intensity of the shadow at each point is calculated and normalized across all the light sources.
Plotting the Shadows:

The code generates plots showing the shadow intensities for different numbers of point light sources.
Code Structure
compute_shadow_intensity(occluder_center, occluder_size, plane_size, num_point_sources):
Computes the shadow intensity grid for a given configuration.
The shadow intensity is computed for various numbers of point sources, and the resulting shadows are displayed in a grid.
Usage
You can modify the parameters like occluder_size, plane_size, and the number of point sources (num_sources_list) to observe different shadow behaviors.

Run the code with:

bash
Copy code
python shadow_simulation.py
Example Output
The output will be a set of plots showing shadow intensities for varying numbers of light sources (e.g., 1, 4, 16, 64). Here is an example of what you might see:

Sharp shadows with fewer light sources.
Softer, more distributed shadows with an increasing number of light sources.
License
This project is licensed under the MIT License - see the LICENSE file for details.

This should be sufficient to document your project for GitHub. Let me know if you want to include any specific images or additional details!











