# Kalman-Filter-Study

#### 1.1. Parameter Configuration:
- **Process Dispersion (Q)**: 1
- **Measurement Dispersion (R)**: 10
- **Initial Covariance Matrix (P)**: 1
- **Initial State (x)**: 0

#### 1.2. Filtering Results:
The graph shows that the Kalman filter estimate (green line) follows the true signal (blue dashed line) well and significantly reduces the noise compared to the noisy signal (orange line). The filter successfully smooths the values but follows slow changes in the signal due to the high level of measurement noise.

#### 1.3. Analysis of Variance:
The reduction in variance after filtering indicates the effectiveness of the filter in reducing noise for the selected parameter values.

#### 1.4. General Conclusions:
For this case, the filter performs well with a process variance level of **Q = 1** and a measurement variance of **R = 10**. Lowering **R** can make the filter more sensitive to fluctuations, but also noisier. Increasing **Q** allows for faster adaptation to changes, but increases the noise level in the estimate.

![Screenshot 1](https://github.com/Sun-95/Kalman-Filter-Study/blob/main/screenshots/1.png)
