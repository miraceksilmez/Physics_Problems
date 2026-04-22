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
$$\frac{m}{k} \ln\left(\frac{mg + kv}{mg + kv_0}\right) = -t$$

Solving for $v(t)$:
$$v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}$$

### Position Equation $x(t)$
Integrating $v(t)$ with the initial condition $x(0) = 10$:
$$x(t) = 10 + \int_{0}^{t} v(t') dt'$$
$$x(t) = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)(1 - e^{-\frac{k}{m}t}) - \frac{mg}{k}t$$

---

## 2. Determining Maximum Height

At maximum height ($H_{max}$), the velocity is zero ($v(t_{up}) = 0$).

### Time to reach peak ($t_{up}$):
Setting $v(t) = 0$:
$$0 = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t_{up}} - \frac{mg}{k}$$
$$e^{-\frac{k}{m}t_{up}} = \frac{mg}{mg + kv_0}$$
$$t_{up} = \frac{m}{k} \ln\left(1 + \frac{kv_0}{mg}\right)$$

### Maximum Height Value:
Substitute $t_{up}$ into the $x(t)$ equation:
$$H_{max} = 10 + \frac{mv_0}{k} - \frac{m^2g}{k^2} \ln\left(1 + \frac{kv_0}{mg}\right)$$

---

## 3. Comparison with Vacuum Case (No Drag)

When $k = 0$, the equations simplify to standard kinematics:
* **Time to peak:** $t_{vacuum} = \frac{v_0}{g}$
* **Max Height:** $H_{vacuum} = 10 + \frac{v_0^2}{2g}$

**Key Differences:**
1.  **Asymmetry:** With drag, the time to go up is shorter than the time to come down.
2.  **Terminal Velocity:** In the drag case, the object approaches a constant speed $v_t = \frac{mg}{k}$ during fall, whereas in vacuum, speed increases indefinitely.
3.  **Peak:** $H_{max}$ with drag is always lower than $H_{vacuum}$.

---

## 4. Numerical Simulation (Python)

You can use the following Python script to visualize the motion:

```python
import numpy as np
import matplotlib.pyplot as plt

# Parameters
m, g, k = 1.0, 9.8, 0.2
v0, x0 = 20.0, 10.0
dt = 0.01
t = [0]
v = [v0]
x = [x0]

# Euler Method Simulation
while x[-1] > 0 or v[-1] > 0:
    dvdt = -g - (k/m)*v[-1]
    v_new = v[-1] + dvdt * dt
    x_new = x[-1] + v_new * dt
    
    t.append(t[-1] + dt)
    v.append(v_new)
    x.append(x_new)
    if x_new < 0: break

# Plotting
plt.plot(t, x)
plt.title("Vertical Motion with Air Drag")
plt.xlabel("Time (s)")
plt.ylabel("Height (m)")
plt.grid(True)
plt.show()
