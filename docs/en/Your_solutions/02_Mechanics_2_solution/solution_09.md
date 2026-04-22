# Physics Solution: Vertical Throw with Air Drag

This document analyzes the motion of an object thrown vertically upwards subject to a linear drag force ($F_d = -kv$).

---

## 1. Equation of Motion

The total force acting on the object is the sum of gravity and air resistance. According to Newton's Second Law:

$$m \frac{dv}{dt} = -mg - kv$$

### Analytical Solution
To solve for velocity $v(t)$, we rearrange and separate variables:

$$\frac{m \cdot dv}{mg + kv} = -dt$$

Integrating both sides from $v_0$ to $v(t)$ and $0$ to $t$:

$$\frac{m}{k} \ln\left(\frac{mg + kv(t)}{mg + kv_0}\right) = -t$$

Solving for $v(t)$:

$$v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}$$

### Position Equation $x(t)$
Integrating the velocity equation with the initial condition $x(0) = 10$:

$$x(t) = 10 + \int_{0}^{t} v(t') dt'$$

$$x(t) = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)(1 - e^{-\frac{k}{m}t}) - \frac{mg}{k}t$$

---

## 2. Determining Maximum Height

At maximum height ($H_{max}$), the velocity is zero ($v(t_{up}) = 0$).

### A. Time to reach peak ($t_{up}$)
Setting the velocity equation to zero:

$$0 = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t_{up}} - \frac{mg}{k}$$

$$t_{up} = \frac{m}{k} \ln\left(1 + \frac{kv_0}{mg}\right)$$

### B. Maximum Height Value
Substituting $t_{up}$ back into the position equation:

$$H_{max} = 10 + \frac{mv_0}{k} - \frac{m^2g}{k^2} \ln\left(1 + \frac{kv_0}{mg}\right)$$

---

## 3. Comparison: Drag vs. Vacuum Case

| Feature | Vacuum ($k=0$) | Air Drag ($k > 0$) |
| :--- | :--- | :--- |
| **Max Height** | Higher ($H = 10 + \frac{v_0^2}{2g}$) | Lower (Energy lost to drag) |
| **Time to Peak** | $t = \frac{v_0}{g}$ | $t < \frac{v_0}{g}$ |
| **Velocity Decay** | Linear | Exponential |
| **Terminal Speed** | None (increases indefinitely) | Approaches $v_t = \frac{mg}{k}$ |

---

## 4. Numerical Simulation (Python)

The following script performs a numerical integration using the Euler method to simulate the flight:

```python
import numpy as np
import matplotlib.pyplot as plt

# Parameters
m, g, k = 1.0, 9.8, 0.2
v0, x0 = 20.0, 10.0
dt = 0.01

# Initializing lists
t, v, x = [0], [v0], [x0]

# Simulation loop
while x[-1] > 0:
    a = -g - (k/m) * v[-1]
    v_new = v[-1] + a * dt
    x_new = x[-1] + v_new * dt
    
    t.append(t[-1] + dt)
    v.append(v_new)
    x.append(x_new)

# Output results
print(f"Max Height: {max(x):.2f} m")

# Plotting
plt.figure(figsize=(8, 5))
plt.plot(t, x, label='Height (x)')
plt.axhline(0, color='black', lw=1)
plt.title("Vertical Motion with Linear Air Drag")
plt.xlabel("Time (s)")
plt.ylabel("Height (m)")
plt.legend()
plt.grid(True)
plt.show()
