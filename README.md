# Signal-Processing-DTFT-and-Convolution
This project is about designing generalized MATLAB codes that perform discrete convolution and discrete-time Fourier transform (DTFT) to audio and voice signals. Signal-processing MATLAB functions like “conv”, “filter”, and “fir1” are used to manipulate the input voice signal with different filters and study the output spectrum.

### 1. Discrete Convolution
The discrete convolution deals with 2 discrete-time signals in the manner shown in equation 1. Convolutions are basically multiply-and-accumulate (MAC) operations, where one of the 2 signals is flipped around the y-axis, then is moved towards the other signal in steps. At each step, corresponding samples are multiplied and the output sample is produced by summing those products. The length of the resulted output will be the sum of the 2 signals’ lengths minus one as shown in equation 2.

![discrete_conv](https://user-images.githubusercontent.com/27668656/120939459-1651ff80-c6cd-11eb-8a6b-f3858b7b3f0d.PNG)

- Here's a video that explains the operation of discrete convolution: [Discrete time convolution](https://www.youtube.com/watch?v=W56uw9GUvxU)
- The matlab implementation of the discrete convolution can be found here: [my_conv.m](https://github.com/muhammadaldacher/Signal-Processing-DTFT-and-Convolution/blob/main/main%20codes/my_conv.m)


### 2. Discrete-Time Fourier Transform
The discrete-time Fourier transform follows equation 3. The code is implemented by using 2 for loops, the 1st loop is to go over each n and do the multiplication of the input x with the complex component, and the 2nd loop is to go over each Ω and accumulate the products. Ω represents the digital filter defined in equation 4.

![discrete_time_fourier_transform](https://user-images.githubusercontent.com/27668656/120939519-4c8f7f00-c6cd-11eb-9e1f-8dee9c1ac658.PNG)

- The matlab implementation of the discrete-time Fourier Transform can be found here: [my_dtft.m](https://github.com/muhammadaldacher/Signal-Processing-DTFT-and-Convolution/blob/main/main%20codes/my_dtft.m)

### 3. Simulation & Results:
- **(A) Convolution:**    ["PartA_convolution.m"](https://github.com/muhammadaldacher/Signal-Processing-DTFT-and-Convolution/blob/main/main%20codes/PartA_convolution.m)<br/>
This code is used to perform a simple convolution on 2 signals.<br/><br/>
![conv_example](https://user-images.githubusercontent.com/27668656/120940770-c460a800-c6d3-11eb-88ff-b4917dacca9e.png)<br/><br/>

- **(B) DTFT & implementing a low-pass filter:**   ["PartB_DTFT.m"](https://github.com/muhammadaldacher/Signal-Processing-DTFT-and-Convolution/blob/main/main%20codes/PartB_DTFT.m)<br/>
This code takes an audio file & performs DTFT to observe the frequency spectrum of this audio file. Then, by using low-pass filters, the high-frequency components are filtered out.  <br/><br/>
![dtft_filter](https://user-images.githubusercontent.com/27668656/120942252-8caa2e00-c6dc-11eb-9e0b-cdcafd59b837.png)<br/><br/>

* For More info, Check the project report: ["Report"](https://drive.google.com/file/d/1q6EvsJwwGDiYhQzKgBx9zrkdxdVo5uoH/view?usp=sharing)<br/><br/>

*****************
### References:
EE210 Lecture Notes & Material:<br/>
https://drive.google.com/drive/folders/1UaLbYzHEQJgwkm-EXSBJfqVmOckCmXtj?usp=sharing <br/>



