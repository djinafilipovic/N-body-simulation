# N-body-simulation
This project implements an N-body simulation that models the collision of two identical spiral galaxies, each containing 400 particles. The simulation computes the state of the system at regular intervals over a period of 5 billion years (5 Gyr). The initial conditions of the galaxies, including the positions, velocities, and masses of the particles, are set up to simulate their motion and interaction over time. The simulation is executed for varying relative velocities (50 km/s, 100 km/s, 200 km/s, and 500 km/s) and different distances (100 kpc and 200 kpc) between the galaxies.

By observing the evolution of the total energy of the system (E) over time, the stability of the newly formed structure is evaluated. The results indicate that in all cases, the structure created is unstable. Adjusting the relative velocity and distance between the galaxies reveals that lower velocities and greater distances lead to longer-lasting stability.

Features
Gravitational Interaction: The simulation uses Newton's law of gravitation to calculate the force between particles.
Euler Integration: Euler's method is used to solve the equations of motion and update the position and velocity of each particle.
Energy Monitoring: The system's total energy (kinetic and potential) is tracked over time to determine the stability of the galaxy collision.
Customizable Parameters: Users can adjust the initial conditions, including particle mass, position, velocity, and the distance and relative velocity between the galaxies.
Graphical Output: The simulation generates graphical outputs for the system's behavior over time, including energy trends and galaxy structures

Methodology
The project simulates the collision of two galaxies by solving the N-body problem, which involves calculating the motion of particles under mutual gravitational attraction. The simulation ignores relativistic effects, using Newtonian gravity instead. The core equations that govern the motion of each particle are derived from Newton's law of gravitation.

Initial Conditions and Parameters
Number of Particles: 400 (representing stars in a galaxy, where each particle represents 250,000 stars).
Distance Between Galaxies: 100 kpc and 200 kpc.
Relative Velocities: 50 km/s, 100 km/s, 200 km/s, and 500 km/s.
Simulation Duration: 5 Gyr.
Integration Step Size: 10 Myr (with a total of 500 updates during the simulation).
Stability Analysis
The stability of the resulting galaxy structures after the collision is determined by monitoring the total energy of the system, calculated as the sum of potential and kinetic energies. The system is considered stable if the absolute value of the potential energy is greater than the kinetic energy.

The results indicate that while the system remains gravitationally bound, it shows signs of instability, particularly at higher relative velocities or shorter distances between the galaxies. This behavior is expected due to the inherent chaotic nature of galaxy collisions.

Results and Discussion
Earth-Sun Simulation: A simplified 2-body problem was simulated, where Earth orbits the Sun over one year. The results were used as a test to ensure the simulation code works as expected.
Isolated Galaxy: The stability of an isolated galaxy was tested by observing the total energy over 5 Gyr. The results showed the galaxy remained stable, with total energy staying negative throughout the simulation.
Galaxy Collision: The main focus of this project is simulating the collision of two galaxies. Different initial conditions (relative velocity and distance) were tested, revealing the instability of the resulting structure in all cases.
Conclusion
This N-body simulation provides valuable insights into the dynamics of galaxy collisions. The results highlight the sensitivity of the system to initial conditions, such as relative velocity and distance, and demonstrate the unstable nature of the structures formed during these events. Further improvements could involve the use of more advanced integrators for higher accuracy and the inclusion of relativistic effects for more realistic simulations.
