# Rotational Dynamics and Moment of Inertia: Class-work Solutions

MEC101 (Mechanics) class work.

## Contents
- [1. Motor coming to rest](#1-motor-coming-to-rest)
- [2. Fan accelerating](#2-fan-accelerating)
- [3. Pulley with bucket](#3-pulley-with-bucket)
- [4. Moment of inertia of wheel](#4-moment-of-inertia-of-wheel)
- [5. Angle rotated in successive seconds](#5-angle-rotated-in-successive-seconds)
- [6. Torque to stop the wheel](#6-torque-to-stop-the-wheel)
- [7. Angular velocity after 5 s](#7-angular-velocity-after-5-s)
- [8. Acceleration of the two blocks (Atwood machine with massive pulley)](#8-acceleration-of-the-two-blocks-atwood-machine-with-massive-pulley)
- [9. Rod with two masses about AB](#9-rod-with-two-masses-about-ab)
- [10. Three particles of equilateral triangle about AX](#10-three-particles-of-equilateral-triangle-about-ax)
- [11. Four particles of a square about the centre](#11-four-particles-of-a-square-about-the-centre)
- [Continuous mass distributions](#continuous-mass-distributions)

---

## 1. Motor coming to rest
Initial angular speed:
$$
\omega_0 = 100\,\text{rev/min} = \frac{100 \times 2\pi}{60} = \frac{10\pi}{3}\,\text{rad/s}
$$
Time $t = 15\,\text{s}$, final $\omega = 0$.

Angular acceleration:
$$
\alpha = \frac{0 - \omega_0}{t} = -\frac{10\pi}{45} = -\frac{2\pi}{9}\,\text{rad/s}^2
$$

Angular displacement:
$$
\theta = \omega_0 t + \frac12\alpha t^2 = \left(\frac{10\pi}{3}\right)(15) + \frac12\left(-\frac{2\pi}{9}\right)(225) = 50\pi - 25\pi = 25\pi\,\text{rad}
$$

Number of revolutions:
$$
N = \frac{\theta}{2\pi} = 12.5
$$

## 2. Fan accelerating
Maximum angular speed:
$$
\omega_{\max} = 400\,\text{rpm} = \frac{400 \times 2\pi}{60} = \frac{40\pi}{3}\,\text{rad/s}
$$
Time to reach it from rest: $t = 5\,\text{s}$.

$$
\alpha = \frac{\omega_{\max}}{5} = \frac{8\pi}{3}\,\text{rad/s}^2
$$

Half maximum speed: $\omega = \frac{20\pi}{3}\,\text{rad/s}$.

Time taken:
$$
t' = \frac{\omega}{\alpha} = 2.5\,\text{s}
$$

## 3. Pulley with bucket
Radius $r = 10\,\text{cm} = 0.1\,\text{m}$, linear speed $v = 0.2\,\text{m/s}$, linear acceleration $a = 4.0\,\text{m/s}^2$.

Since the rope does not slip:
$$
\omega = \frac{v}{r} = \frac{0.2}{0.1} = 2\,\text{rad/s}
$$
$$
\alpha = \frac{a}{r} = \frac{4}{0.1} = 40\,\text{rad/s}^2
$$

## 4. Moment of inertia of wheel
Torque $\tau = Fr = 5.0 \times 0.10 = 0.50\,\text{N·m}$.

Given $\alpha = 2.0\,\text{rad/s}^2$:
$$
I = \frac{\tau}{\alpha} = \frac{0.50}{2.0} = 0.25\,\text{kg·m}^2
$$

## 5. Angle rotated in successive seconds
From rest, $\theta_1 = 2.5\,\text{rad}$ in first second:
$$
\theta = \frac12\alpha t^2 \implies 2.5 = \frac12\alpha \implies \alpha = 5\,\text{rad/s}^2
$$

Angle rotated in the next (second) second:
$$
\theta_2 = \frac12\alpha(2)^2 - \frac12\alpha(1)^2 = 10 - 2.5 = 7.5\,\text{rad}
$$

## 6. Torque to stop the wheel
$$
\omega_0 = 50\,\text{rpm} = \frac{5\pi}{3}\,\text{rad/s}, \quad t = 60\,\text{s}, \quad \omega = 0
$$
$$
\alpha = \frac{0 - \omega_0}{t} = -\frac{\pi}{36}\,\text{rad/s}^2
$$
$$
\tau = I\alpha = 2 \times \left(-\frac{\pi}{36}\right) = -\frac{\pi}{18}\,\text{N·m}
$$
Magnitude: $\dfrac{\pi}{18}\,\text{N·m}$.

## 7. Angular velocity after 5 s
Torque $\tau = Fr = 20 \times 0.20 = 4.0\,\text{N·m}$.

$$
\alpha = \frac{\tau}{I} = \frac{4.0}{0.20} = 20\,\text{rad/s}^2
$$
From rest after $t = 5.0\,\text{s}$:
$$
\omega = \alpha t = 100\,\text{rad/s}
$$

## 8. Acceleration of the two blocks (Atwood machine with massive pulley)
Let the two masses be $m_1$ and $m_2$ (assume $m_1 > m_2$).

The magnitude of the linear acceleration of each block is
$$
a = \frac{(m_1 - m_2)g}{m_1 + m_2 + \dfrac{I}{R^2}}
$$
(The angular acceleration of the pulley is $\alpha = a/R$.)

## 9. Rod with two masses about AB
Distances of the point masses from the axis AB are $r_1$ and $r_2$.
$$
I = m_1 r_1^2 + m_2 r_2^2
$$

## 10. Three particles of equilateral triangle about AX
Place A at the origin, AB along the $x$-axis. Axis AX is the $y$-axis (perpendicular to AB in the plane).

Perpendicular distances from the axis:
- A: $0$
- B: $L$
- C: $L/2$

$$
I = mL^2 + m\left(\frac{L}{2}\right)^2 = \frac{5}{4}mL^2
$$

## 11. Four particles of a square about the centre
Distance of each mass from the centre is $\dfrac{a}{\sqrt{2}}$.
$$
I = 4 \times m \left(\frac{a}{\sqrt{2}}\right)^2 = 2ma^2
$$

## Continuous mass distributions
- **(a)** Uniform rod of mass $M$, length $L$ about a perpendicular bisector: $\dfrac{1}{12}ML^2$
- **(b)** Rectangular plate of mass $M$, width $b$ (about the axis parallel to the length and through the centre): $\dfrac{1}{12}Mb^2$
- **(c)** Circular ring of mass $M$, radius $R$ about its central axis (perpendicular to the plane): $MR^2$
- **(d)** Hollow cylinder (thin cylindrical shell) of mass $M$, radius $R$ about its axis: $MR^2$
- **(e)** Uniform solid cylinder of mass $M$, radius $R$ about its axis: $\dfrac{1}{2}MR^2$
