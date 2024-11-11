# Kalman-Filter-Study

#### 1.1. Parameter Configuration:
- **Process Dispersion (Q)**: 1
- **Measurement Dispersion (R)**: 10
- **Initial Covariance Matrix (P)**: 1
- **Initial State (x)**: 0
-  **Constant Signal Component (offset)**: 10
-  **Total Modeling Time (total_time)**: 1

#### 1.2. Filtering Results:
The graph shows that the Kalman filter estimate follows the true signal well and significantly reduces the noise compared to the noisy signal. The filter successfully smooths the values but follows slow changes in the signal due to the high level of measurement noise.

#### 1.3. Analysis of Variance:
The reduction in variance after filtering indicates the effectiveness of the filter in reducing noise for the selected parameter values.

#### 1.4. General Conclusions:
For this case, the filter performs well with a process variance level of **Q = 1** and a measurement variance of **R = 10**. Lowering **R** can make the filter more sensitive to fluctuations, but also noisier. Increasing **Q** allows for faster adaptation to changes, but increases the noise level in the estimate.

![Screenshot 1](https://github.com/Sun-95/Kalman-Filter-Study/blob/main/screenshots/1.png)


#### 2.1. Parameter Configuration:
- **Process Dispersion (Q)**: 0.1
- **Measurement Dispersion (R)**:  5
- **Initial Covariance Matrix (P)**: 0.5
- **Initial State (x)**: 5
-  **Constant Signal Component (offset)**: 0
-  **Total Modeling Time (total_time)**: 0.5

#### 2.2. Analysis of Variance:
The Kalman filter significantly reduced the variance of the noise after processing the signal, indicating the effectiveness of the smoothing, achieving a result with a significantly lower noise level.

#### 2.3. General Conclusions:
The Kalman filter with Q = 0.1 and R = 5 successfully reduces the noise level, but may slightly dampen the instantaneous signal fluctuations due to the lower process variance. The R parameter determines the sensitivity of the filter to the measurements—decreasing R will make the filter more sensitive, but more prone to noise. Increasing Q will result in faster adaptation to changes in the signal, but will also increase the noise level in the smoothed signal. The current settings therefore provide good smoothing, although the R and Q settings can be adapted for a better balance between sensitivity and stability.

![Screenshot 2](https://github.com/Sun-95/Kalman-Filter-Study/blob/main/screenshots/2.png)


#### 3.1. Parameter Configuration:
- **Process Dispersion (Q)**: 5
- **Measurement Dispersion (R)**: 20
- **Initial Covariance Matrix (P)**: 10
- **Initial State (x)**: -5
-  **Constant Signal Component (offset)**: 2
-  **Total Modeling Time (total_time)**: 15

#### 2.2. Analysis of Variance:
The results show a significant reduction in variance after filtering, demonstrating the ability of the Kalman filter to smooth out noise, although a value of R = 20 makes the filter less sensitive to changes in the measurements.

#### 2.3. General Conclusions:
For this example, a filter with parameters Q = 5 and R = 20 provides sufficient noise smoothing while maintaining the stability of the filtered signal. Decreasing R would make the filter more sensitive to instantaneous changes in the measurements, but could also increase the noise level. Conversely, increasing Q would allow the filter to adapt to sudden changes faster, but with increased fluctuations in the filtered values. These settings provide the best balance between smoothing and accuracy, but different Q and R values ​​can be selected for better results for different conditions.

![Screenshot 3](https://github.com/Sun-95/Kalman-Filter-Study/blob/main/screenshots/3.png)






