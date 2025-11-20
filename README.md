# EXP 1 A : COMPUTATION OF DFT USING DIRECT AND FFT

# AIM: 

To Obtain DFT and FFT of a given sequence in SCILAB.


# APPARATUS REQUIRED: 
PC installed with SCILAB. 

# PROGRAM: 
// DISCRETE FOURIER TRANSFORM 

clear; 

clc; 

close;

xn = [0.5 0.5 0.5 0.5 0 0 0 0] 
 
n1=0:1:length(xn)-1; 

subplot(2,2,1); 

plot2d3(n1,xn); 

xlabel('Time n'); 

ylabel('Amplitude'); 

title('Input Sequence'); 
 
Xk = fft(xn); 
 
K1=0:1:length(Xk)-1; 

magnitude=abs(Xk) 

subplot(2,2,2); 

plot2d3(K1,magnitude); 

xlabel('frequency(Hz)'); 

ylabel('magnitude(gain)'); 

title('magnitude spectrum'); 

angle = atan(imag(Xk),real(Xk)) 

subplot(2,2,3); 

plot2d3(K1,angle); 

xlabel('frequency(Hz)'); 

ylabel('Phase'); 

title('Phase spectrum') 

y= ifft(Xk) 
 
n2=0:1:length(y)-1; 

subplot(2,2,4) 

plot2d3(n2,y) 

xlabel('Time n'); 

ylabel('Amplitude'); 

title('Inverse FFT OF X(K)');

# OUTPUT: 


![WhatsApp Image 2025-11-20 at 19 52 58_4e415905](https://github.com/user-attachments/assets/365f785d-4cc8-492d-983b-cf25554f9da9)



![WhatsApp Image 2025-11-20 at 19 53 15_26059ddd](https://github.com/user-attachments/assets/3097e757-ff83-4175-b900-2febf256de97)




# RESULT: 


Thus,The DFT and FFT of the given sequence is obtained using SCILAB.
