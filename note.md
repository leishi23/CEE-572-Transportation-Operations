# CEE 572 Transportation Operations

## Lecture 1: Time-space Diagram

- **Time-space diagram**: a graphical representation of the movement of vehicles through a section of roadway over time.
- **Space Equation**: $x = f(t)$
  - When $a$ is constant, $x = x_0 + v_0t + \frac{1}{2}at^2$, $x = \frac{v^2 - v_0^2}{2a}$
  - When $a$ is not constant, $a(v) = \frac{dv}{dt}$, i.e. $\int_{v_0}^{v} \frac{dv}{a(v)} = \int_{t_0}^{t} dt$
    - If $a(v) = \alpha - \beta v$, $t = \frac{1}{\beta} \ln \left( \frac{\alpha - \beta v_0}{\alpha - \beta v} \right)$, $v(t) = \frac{\alpha}{\beta}(1 - e^{-\beta t}) + v_0 e^{-\beta t}$, $x(t) = \frac{\alpha}{\beta}t - \frac{\alpha}{\beta^2}(1 - e^{-\beta t}) + \frac{v_0}{\beta}(1 - e^{-\beta t})$

<!-- new page -->
<div style="page-break-after: always;"></div>

## Lecture 2: Traffic Stream Properties

### Traffic Stream Definitions
- **Headway**: the time between the passage of the front of one vehicle and the front of the following vehicle. (inter-arrival time)
- **Spacing**: the distance between the front of one vehicle and the front of the following vehicle. (separation distance)
- **Flow**: the number of vehicles passing a point in a given time period.
  - $q(T, x) = \frac{m}{T}$ (vehs/time)
  - $T \approx \sum_{i=1}^{m} h_i$ (time), $q(T, x) = \frac{m}{\sum_{i=1}^{m} h_i} = \frac{1}{\bar{h}}$ (vehs/time), where $\bar{h}$ is the average headway or average time between vehicles.
- **Density**: the number of vehicles per unit length of roadway.
  - $k (L, t) = \frac{n}{L}$ (vehs/distance)
  - $L \approx \sum_{i=1}^{n} s_i$ (distance), $k(L, t) = \frac{n}{\sum_{i=1}^{n} s_i} = \frac{1}{\bar{s}}$ (vehs/distance), where $\bar{s}$ is the average spacing or average distance between vehicles.

### Traffic Stream Relationships
For steady-state traffic flow, the following relationships hold:
- $m = n$ (number of vehicles entering a section of roadway is equal to the number of vehicles leaving the section of roadway)
$$ q \cdot T = k \cdot L $$
$$ q = k \cdot \frac{L}{T} = k \cdot v $$

### Stationary vs. Homogeneous Traffic Streams
- **Stationary Traffic Stream**: traffic flow does not change over time (but may change over space)
  - Constant headway: $h_i = h$, $q = \frac{1}{\bar{h}}$
- **Homogeneous Traffic Stream**: traffic flow does not change over space (but may change over time)
  - Constant spacing: $s_i = s$, $k = \frac{1}{\bar{s}}$