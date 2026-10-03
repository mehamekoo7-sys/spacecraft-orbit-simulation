# spacecraft-orbit-simulation
A simplified Python simulation showing how initial spacecraft velocity changes orbital trajectories.
# Spacecraft Orbit Simulation

A simplified two-body orbital simulation built in Python.

## Project question

How does the initial velocity of a spacecraft affect its trajectory?

## What the simulation shows

The simulation compares four initial velocities:

- 0.7 times the scaled circular velocity
- 1.0 times the scaled circular velocity
- 1.4 times the scaled circular velocity
- 1.5 times the scaled circular velocity

## Main result

A lower initial velocity produces an elliptical orbit. At the circular velocity, the spacecraft follows an approximately circular path. Close to escape velocity, the orbit becomes highly elongated. Above escape velocity, the spacecraft follows an escape trajectory.

## Physics

The simulation uses a simplified gravitational acceleration model:

a = -mu*r/r^3

The escape velocity is:

v_escape = sqrt(2*mu/r)

For this simulation, mu = 1 and the initial radius is 1, so the escape velocity is approximately 1.414 scaled velocity units.

## Limitations

This is an educational two-body model. It does not include:

- Atmospheric drag
- Thrust
- Other planets
- Planetary rotation
- Real spacecraft dimensions
- Real mission units

## Tools used

- Python
- NumPy
- Matplotlib
- Google Colab

## Preview

![Orbit comparison](orbit-comparison.png)

