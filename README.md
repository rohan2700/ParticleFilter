Sensor Fusion - Particle Filter
---------------------------------
This project focuses on the implementation of a Particle Filter (PF) to estimate the positions and velocity vectors of multiple balls thrown simultaneously, based solely on observed erroneous positions over time. The goal is to demonstrate the effectiveness of the Particle Filter in handling uncertainty and noise in sensor data while tracking multiple indistinguishable targets.

## Methodology

-Particle Filter Implementation: The core of the project involves implementing the Particle Filter algorithm, which includes:
-Prediction Step: Predicting the future state of each particle based on the motion model.
-Update Step: Updating the weights of the particles based on the likelihood of the observed data.
-Resampling Step: Resampling particles to focus on those with higher weights, ensuring effective tracking.
-Simulation of Observations: The project simulates the observation process, incorporating noise and dropout periods to reflect real-world sensor limitations.
-Parameterization of Uncertainty: The uncertainty in the observations is parameterized, allowing for flexibility in the simulation and testing of different scenarios.
-Visualization: The results of the Particle Filter are visualized graphically, showing the estimated trajectories of the balls alongside the true trajectories and noisy observations.

## Libraries Used

- `numpy`
- `matplotlib`
- `random`

## Parameters

- `n_balls`: Number of balls to simulate
- `T`: Total simulation time
- `dt`: Time step
- `g`: Acceleration due to gravity
- `observation_noise_std` : Noise observation\
- `n_particles_per_ball` : Number of particles for each ball
- `dropout_length` : Dropout intervals

## How to Run

1. Make sure you have Python and Jupyter Notebook installed.
2. Install required libraries using pip install
3. The provided code is structured sequentially, with each section building upon the previous one. To run the simulation and generate the plots, execute the Python script.
4. The script will:
 - Generate true trajectories with ballistic information.
 - Generate noisy observations based on these trajectories.
 - Initialize and run the Particle Filter to estimate the ball paths.
 - Simulate sensor dropouts and variable observation rates.
 - Demonstrate variable time step simulation.
 - Display several plots visualizing the different stages and results of the tracking process.

## Note 

An additional file named "ParticleFilter_Experiments" has been included in this which shows our research and experimentations that helped us in our learning process to understand the final particle filter implementation. 

## Authors
Rohan Sanjay Patil (k70875)
Vidya Padmanabha (k70818)
