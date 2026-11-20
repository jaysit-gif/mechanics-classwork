# Rotational Dynamics: Class-work Solutions (Set 2)

MEC101 (Mechanics) class work: pure rolling, torque, work and angular momentum.
Problems 1 to 11 in full, step by step. Final answers are boxed.

## Contents
- [Standard moments of inertia used](#standard-moments-of-inertia-used)
- [1. Sphere rolling down an incline](#1-sphere-rolling-down-an-incline)
- [2. Cylinder suspended by two strings](#2-cylinder-suspended-by-two-strings)
- [3. Force at the top of a sphere](#3-force-at-the-top-of-a-sphere)
- [4. Cylinder rolling down an incline](#4-cylinder-rolling-down-an-incline)
- [5. Revolutions of a rolling wheel](#5-revolutions-of-a-rolling-wheel)
- [6. Angular momentum of the pulley-and-masses system](#6-angular-momentum-of-the-pulley-and-masses-system)
- [7. Disc rotating about a diameter](#7-disc-rotating-about-a-diameter)
- [8. Block pulled up an incline by a spinning wheel](#8-block-pulled-up-an-incline-by-a-spinning-wheel)
- [9. Solid cylinder with a falling block](#9-solid-cylinder-with-a-falling-block)
- [10. Work done by a constant torque](#10-work-done-by-a-constant-torque)
- [11. Work done by a variable torque](#11-work-done-by-a-variable-torque)
- [Summary of answers](#summary-of-answers)

---

## Standard moments of inertia used

| Body | Axis | $I$ |
|---|---|---|
| Solid sphere, mass $m$, radius $R$ | through centre | $\tfrac{2}{5}mR^2$ |
| Solid cylinder / disc, mass $m$, radius $R$ | cylinder axis (through centre, perpendicular to disc) | $\tfrac12 mR^2$ |
| Uniform disc, mass $m$, radius $R$ | any diameter | $\tfrac14 mR^2$ |

Rolling without slipping: $v_{cm} = \omega R$ and $a_{cm} = \alpha R$.

---

## 1. Sphere rolling down an incline

**Given:** solid sphere, mass $m$, radius $R$, incline angle $\theta$, pure rolling. $I = \tfrac25 mR^2$.

Let $a$ be the acceleration down the incline and $f$ the static friction acting up the incline (at the contact point).

**Translation (along the incline):**
$$
mg\sin\theta - f = ma \tag{1}
$$

**Rotation about the centre** (only friction has a torque about the centre):
$$
fR = I\alpha = \tfrac25 mR^2\cdot\frac{a}{R}
\;\Rightarrow\; f = \tfrac25 ma \tag{2}
$$

Put (2) in (1):
$$
mg\sin\theta = ma + \tfrac25 ma = \tfrac75 ma
\;\Rightarrow\; a = \tfrac57 g\sin\theta
$$

Friction:
$$
f = \tfrac25 m\cdot\tfrac57 g\sin\theta = \tfrac27 mg\sin\theta
$$

**Minimum coefficient of friction.** The normal force is $N = mg\cos\theta$. Pure rolling needs $f \le \mu N$:
$$
\tfrac27 mg\sin\theta \le \mu\, mg\cos\theta
\;\Rightarrow\; \mu \ge \tfrac27\tan\theta
$$

$$
\boxed{a = \tfrac57 g\sin\theta,\qquad f = \tfrac27 mg\sin\theta\ (\text{up the incline}),\qquad \mu_{\min} = \tfrac27\tan\theta}
$$

---

## 2. Cylinder suspended by two strings

**Assumed setup (standard HC Verma figure, not available here):** the cylinder (mass $m$, radius $R$) hangs from two vertical strings wrapped around it, with the upper ends fixed to the ceiling. As the cylinder falls, the strings unwind, so it rotates about its axis while its centre moves down. $I = \tfrac12 mR^2$. Each string has tension $T$.

**Translation (downward positive):**
$$
mg - 2T = ma \tag{1}
$$

**Rotation about the centre** (the two tensions act at distance $R$ from the axis):
$$
2T\cdot R = I\alpha = \tfrac12 mR^2\cdot\frac{a}{R}
\;\Rightarrow\; 2T = \tfrac12 ma \tag{2}
$$
The no-slip condition between string and cylinder gives $\alpha = a/R$, because the top points of the cylinder at the string contact are momentarily at rest.

Put (2) in (1):
$$
mg = ma + \tfrac12 ma = \tfrac32 ma \;\Rightarrow\; a = \tfrac23 g
$$

**(a) Tension in each string:**
$$
T = \tfrac14 ma = \tfrac14 m\cdot\tfrac23 g = \tfrac{mg}{6}
$$

**(b) Speed after falling $h$** (starts from rest, constant $a$):
$$
v^2 = 2ah = \tfrac43 gh \;\Rightarrow\; v = \sqrt{\tfrac{4gh}{3}}
$$

*Energy check:* $mgh = \tfrac12 mv^2 + \tfrac12 I\omega^2 = \tfrac12 mv^2 + \tfrac14 mv^2 = \tfrac34 mv^2$, so $v^2 = \tfrac43 gh$. ✔

$$
\boxed{T = \frac{mg}{6}\ \text{(each string)},\qquad v = \sqrt{\frac{4gh}{3}}}
$$

---

## 3. Force at the top of a sphere

**Given:** solid sphere, mass $m$, radius $R$, on a rough horizontal plane. A horizontal force $F$ acts tangentially at the highest point. Pure rolling. $I = \tfrac25 mR^2$.

Let the sphere accelerate with $a$ in the direction of $F$. Take friction $f$ at the contact point to act forward (in the direction of $F$); if the result is negative, it acts backward.

**Translation:**
$$
F + f = ma \tag{1}
$$

**Rotation about the centre.** $F$ at the top gives torque $FR$. Friction at the bottom, pointing forward, gives torque $fR$ in the opposite sense:
$$
FR - fR = I\alpha = \tfrac25 mR^2\cdot\frac aR
\;\Rightarrow\; F - f = \tfrac25 ma \tag{2}
$$

Add (1) and (2):
$$
2F = \tfrac75 ma \;\Rightarrow\; a = \frac{10F}{7m}
$$

Subtract (2) from (1):
$$
2f = \tfrac35 ma = \tfrac35\cdot\frac{10F}{7} = \frac{6F}{7}
\;\Rightarrow\; f = \frac{3F}{7}
$$
The result is positive, so friction acts **forward, in the same direction as $F$**.

$$
\boxed{a = \frac{10F}{7m},\qquad f = \frac{3F}{7}\ (\text{in the direction of }F)}
$$

---

## 4. Cylinder rolling down an incline

**Given:** solid cylinder released from rest at the top of an incline of angle $\theta$ and length $l$; rolls without slipping. $I = \tfrac12 mR^2$.

**Method 1: energy conservation.** Height lost: $h = l\sin\theta$. Friction does no work in pure rolling, so
$$
mgl\sin\theta = \tfrac12 mv^2 + \tfrac12 I\omega^2
= \tfrac12 mv^2 + \tfrac12\left(\tfrac12 mR^2\right)\frac{v^2}{R^2}
= \tfrac34 mv^2
$$
$$
v^2 = \tfrac43 gl\sin\theta
$$

**Method 2: kinematics (check).** Same steps as problem 1 with $I=\tfrac12 mR^2$ give $a = \tfrac23 g\sin\theta$. Then $v^2 = 2al = \tfrac43 gl\sin\theta$. ✔

$$
\boxed{v = \sqrt{\tfrac43\, g\, l\sin\theta}}
$$

---

## 5. Revolutions of a rolling wheel

**Given:** perimeter $= 2\pi R = 220\ \text{cm} = 2.2\ \text{m}$, speed $v = 9\ \text{km/h}$.

Speed in SI units:
$$
v = 9\times\frac{1000}{3600} = 2.5\ \text{m/s}
$$

In pure rolling, the wheel advances one perimeter per revolution, so
$$
\text{revolutions per second} = \frac{v}{2\pi R} = \frac{2.5}{2.2} = \frac{25}{22}\approx 1.14
$$

$$
\boxed{\approx 1.14\ \text{rev/s}\ \left(=\tfrac{25}{22}\right)}
$$

---

## 6. Angular momentum of the pulley-and-masses system

**Given:** masses $M > m$ hang on either side of a pulley (radius $r$, moment of inertia $I$) over a light string that does not slip. Released from rest. Find the angular momentum about the pulley axis when $M$ has descended $h$.

Let the common speed of the masses be $v$, so the pulley's angular speed is $\omega = v/r$.

**Energy conservation** (system starts from rest; $M$ falls $h$, $m$ rises $h$):
$$
(M-m)gh = \tfrac12 (M+m)v^2 + \tfrac12 I\frac{v^2}{r^2}
$$
$$
v^2 = \frac{2(M-m)gh}{(M+m) + I/r^2}
= \frac{2(M-m)g h\, r^2}{I + (M+m)r^2}
$$

**Angular momentum about the pulley axis.** Each moving mass has angular momentum $mvr$ about the axis (the velocity is perpendicular to the lever arm $r$), and the two add in the same sense:
$$
L = Mvr + mvr + I\omega = (M+m)vr + \frac{Iv}{r} = \frac{v}{r}\left[I + (M+m)r^2\right]
$$

Substitute $v$:
$$
L = \frac{1}{r}\sqrt{\frac{2(M-m)gh\,r^2}{I+(M+m)r^2}}\;\left[I+(M+m)r^2\right]
= \sqrt{2(M-m)\,g\,h\,\left[I+(M+m)r^2\right]}
$$

$$
\boxed{L = \sqrt{2(M-m)\,g\,h\,\bigl[I + (M+m)r^2\bigr]}}
$$

---

## 7. Disc rotating about a diameter

**Given:** $m = 200\ \text{g} = 0.2\ \text{kg}$, $R = 4.0\ \text{cm} = 0.04\ \text{m}$, $\omega = 10\ \text{rad/s}$, axis along a diameter.

Moment of inertia about a diameter:
$$
I = \tfrac14 mR^2 = \tfrac14(0.2)(0.04)^2 = 8\times10^{-5}\ \text{kg m}^2
$$

Kinetic energy:
$$
K = \tfrac12 I\omega^2 = \tfrac12(8\times10^{-5})(10)^2 = 4\times10^{-3}\ \text{J}
$$

Angular momentum:
$$
L = I\omega = (8\times10^{-5})(10) = 8\times10^{-4}\ \text{kg m}^2/\text{s}
$$

$$
\boxed{K = 4\times10^{-3}\ \text{J},\qquad L = 8\times10^{-4}\ \text{kg m}^2\text{/s}}
$$

---

## 8. Block pulled up an incline by a spinning wheel

**Assumed setup (standard HC Verma figure, not available here):** the wheel (radius $r$, moment of inertia $I$) turns freely on a fixed axle at the top of the incline. The string is wrapped around it and runs parallel to the incline to the block (mass $M$). The incline is **smooth** (no friction), and the string does not slip. The wheel initially spins at $\omega$ so that the block moves **up** the incline.

Initially the block's speed is $v_0 = \omega r$. The block stops when all initial kinetic energy has gone into gravitational potential energy (the incline is smooth, so no energy is lost to friction). Let the block travel a distance $d$ up the incline, a height $d\sin\theta$.

$$
\underbrace{\tfrac12 I\omega^2}_{\text{wheel}} + \underbrace{\tfrac12 M(\omega r)^2}_{\text{block}} = Mg\,d\sin\theta
$$
$$
d = \frac{(I + Mr^2)\,\omega^2}{2Mg\sin\theta}
$$

$$
\boxed{d = \frac{(I + Mr^2)\,\omega^2}{2\,M g\sin\theta}}
$$

---

## 9. Solid cylinder with a falling block

**Given:** solid cylinder $M = 4\ \text{kg}$, $R = 0.2\ \text{m}$, fixed horizontal frictionless axle through its centre. Block $m = 2\ \text{kg}$ on a light string wound around the cylinder, released from rest, falls $h = 2\ \text{m}$. Use $g = 9.8\ \text{m/s}^2$ (values for $g = 10\ \text{m/s}^2$ given after).

Moment of inertia of the cylinder:
$$
I = \tfrac12 MR^2 = \tfrac12(4)(0.2)^2 = 0.08\ \text{kg m}^2
$$

**Acceleration.** Block: $mg - T = ma$. Cylinder: $TR = I\alpha = I\,a/R$, so $T = \tfrac12 Ma$. Then
$$
mg = ma + \tfrac12 Ma \;\Rightarrow\; a = \frac{mg}{m + M/2} = \frac{2(9.8)}{2+2} = 4.9\ \text{m/s}^2
$$

**1. Speed of the block just before reaching the ground:**
$$
v = \sqrt{2ah} = \sqrt{2(4.9)(2)} = \sqrt{19.6} \approx 4.43\ \text{m/s}
$$

**2. Angular velocity of the cylinder:**
$$
\omega = \frac vR = \frac{4.427}{0.2} \approx 22.1\ \text{rad/s}
$$

**3. Tension in the string:**
$$
T = m(g - a) = 2(9.8 - 4.9) = 9.8\ \text{N}
\qquad(\text{check: } \tfrac12 Ma = \tfrac12(4)(4.9) = 9.8\ \text{N}\ ✔)
$$

**4. Potential energy of the block** (lost during the fall, which is what turns into kinetic energy):
$$
\Delta U = mgh = 2(9.8)(2) = 39.2\ \text{J}
$$

**5. Kinetic energies:**
$$
K_{\text{block}} = \tfrac12 mv^2 = \tfrac12(2)(19.6) = 19.6\ \text{J}
$$
$$
K_{\text{cylinder}} = \tfrac12 I\omega^2 = \tfrac12(0.08)(22.136)^2 = 19.6\ \text{J}
$$
Total $= 39.2\ \text{J} = mgh$ ✔ (energy conserved).

$$
\boxed{v \approx 4.43\ \text{m/s},\quad \omega \approx 22.1\ \text{rad/s},\quad T = 9.8\ \text{N},\quad \Delta U = 39.2\ \text{J},\quad K_{\text{cyl}} = K_{\text{block}} = 19.6\ \text{J}}
$$

**If $g = 10\ \text{m/s}^2$:** $a = 5\ \text{m/s}^2$, $v = \sqrt{20}\approx 4.47\ \text{m/s}$, $\omega \approx 22.4\ \text{rad/s}$, $T = 10\ \text{N}$, $\Delta U = 40\ \text{J}$, $K_{\text{cyl}} = K_{\text{block}} = 20\ \text{J}$.

---

## 10. Work done by a constant torque

**Given:** $\tau = 5\ \text{N m}$, $\Delta\theta = 4\ \text{rad}$.

$$
W = \tau\,\Delta\theta = 5\times 4 = 20\ \text{J}
$$

$$
\boxed{W = 20\ \text{J}}
$$

---

## 11. Work done by a variable torque

**Given:** $\tau = 3\theta^2$ (N m), $\theta$ from $0$ to $2$ rad.

$$
W = \int_0^{2}\tau\,d\theta = \int_0^{2} 3\theta^2\,d\theta = \Big[\theta^3\Big]_0^{2} = 8 - 0 = 8\ \text{J}
$$

$$
\boxed{W = 8\ \text{J}}
$$

---

## Summary of answers

| # | Answer |
|---|---|
| 1 | $a = \tfrac57 g\sin\theta$, $f = \tfrac27 mg\sin\theta$, $\mu_{\min} = \tfrac27\tan\theta$ |
| 2 | $T = mg/6$ per string, $v = \sqrt{4gh/3}$ |
| 3 | $a = 10F/(7m)$, $f = 3F/7$ forward |
| 4 | $v = \sqrt{\tfrac43 gl\sin\theta}$ |
| 5 | $25/22 \approx 1.14$ rev/s |
| 6 | $L = \sqrt{2(M-m)gh\,[I+(M+m)r^2]}$ |
| 7 | $K = 4\times10^{-3}$ J, $L = 8\times10^{-4}$ kg m²/s |
| 8 | $d = (I+Mr^2)\omega^2/(2Mg\sin\theta)$ |
| 9 | $v \approx 4.43$ m/s, $\omega \approx 22.1$ rad/s, $T = 9.8$ N, $\Delta U = 39.2$ J, $K_{\text{cyl}} = K_{\text{block}} = 19.6$ J |
| 10 | $20$ J |
| 11 | $8$ J |
