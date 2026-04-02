## 1. Projectile Motion (Projectile Fired from Ground)

**Given Parameters:**
* Initial Velocity ($v_0$): $100 \text{ m/s}$
* Angle ($\theta$): $37^\circ$ ($\sin 37^\circ \approx 0.6$, $\cos 37^\circ \approx 0.8$)
* Gravity ($g$): $10 \text{ m/s}^2$ (assumed for calculation)

### a) Differential Equations of Motion
In projectile motion without air resistance, the only force acting is gravity in the negative $y$ direction.
* **Horizontal (x-axis):** There is no acceleration.
  $$\frac{d^2x}{dt^2} = 0$$
* **Vertical (y-axis):** Acceleration is constant and equal to $-g$.
  $$\frac{d^2y}{dt^2} = -g$$

### b) Time of Flight ($t_{f}$)
The time of flight is the total time the projectile remains in the air until it returns to $y = 0$.
Using the kinematic equation $y = (v_0 \sin\theta)t - \frac{1}{2}gt^2$:
$$0 = (100 \cdot 0.6)t - \frac{1}{2}(10)t^2$$
$$60t = 5t^2 \implies t_{f} = \frac{60}{5} = \mathbf{12 \text{ s}}$$

### c) Maximum Height ($H_{max}$)
Maximum height occurs when the vertical velocity $v_y$ is zero.
$$H_{max} = \frac{(v_0 \sin\theta)^2}{2g}$$
$$H_{max} = \frac{(100 \cdot 0.6)^2}{2 \cdot 10} = \frac{3600}{20} = \mathbf{180 \text{ m}}$$

### d) Range ($R$)
The range is the total horizontal distance traveled during the time of flight.
$$R = (v_0 \cos\theta) \cdot t_{f}$$
$$R = (100 \cdot 0.8) \cdot 12 = 80 \cdot 12 = \mathbf{960 \text{ m}}$$
