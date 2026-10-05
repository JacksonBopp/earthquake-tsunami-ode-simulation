# Earthquake and Tsunami ODE Simulation

A Python notebook that models an earthquake, its aftershocks, and the resulting
tsunami with simple ordinary differential equations. You enter a magnitude,
depth, location, and duration, and it plots the results. It's a conceptual
model for visualization, not a prediction tool.

- **Ground motion:** a damped harmonic oscillator, based on elastic rebound theory
- **Aftershocks:** an Omori's-law decay rate
- **Tsunami:** wave height versus distance from the epicenter, driven by an estimate of seafloor displacement

Built with NumPy, SciPy (`odeint`), and Matplotlib.

<img width="1255" height="789" alt="Earthquake displacement, velocity, and aftershock rate over time" src="https://github.com/user-attachments/assets/d19ba34f-6181-4e83-8abc-f26f144d0d3e" />

<img width="1300" height="940" alt="Tsunami wave height versus distance at several time snapshots" src="https://github.com/user-attachments/assets/8ba833fd-c062-403b-a309-8f675ee05550" />

## Running it

[Open it in Google Colab](https://colab.research.google.com/github/JacksonBopp/earthquake-tsunami-ode-simulation/blob/main/Earthquake_ODE.ipynb),
or locally:

```bash
pip install numpy scipy matplotlib jupyter
jupyter notebook Earthquake_ODE.ipynb
```
