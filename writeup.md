Proportional control is to perform an operation proportional to the magnitude of the difference with the target (It refers to Cross track error). 
If the proportional gain is increased, the target value is approached quickly. However, if it is too large, an overshoot occurs to the target value and eventually causes a continuous vibration phenomenon.
The continuous vibration phenomenon occurs because the speed is too high near the target value. Therefore, introduce derivative gain（Kd) to adjust the speed too high and adjust the speed.
Even if the proportional gain and the derivative gain are adjusted, if the steady-state error offset with respect to the target value is still observed, the offset is corrected by introducing the integral gain (Ki).

$$
θ_{steer}=K_pE_{CTE}-K_i\int_{0}^{T}E_{CTE}dt-K_d\dot{E_{CTE}}
$$