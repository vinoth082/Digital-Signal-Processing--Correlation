# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM:

% INPUT SIGNAL-1
a = input('enter the starting x(n)');
x = input('Enter the x(n) sequence');
n = a : 1 : length(x) + a - 1;
figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')

% INPUT SIGNAL-2
b = input('enter the starting y(n)');
y = input('Enter the y(n) sequence');
m = input('enter the ending y(n)');
n1 = b : 1 : length(y) + b - 1;

figure(2)
stem(n1,y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')

% DISCRETE AUTO CORRELATED SIGNAL
Out1 = xcorr(x,x);
n2 = a - m : 1 : length(Out1) + a - m - 1;
figure(3)
stem(n2,Out1)
xlabel('Time')
ylabel('Amplitude')
title('Discrete auto correlated waveform')

% DISCRETE CROSS CORRELATED SIGNAL
Out2 = xcorr(x,y);
n3 = a - m : 1 : length(Out2) + a - m - 1;
figure(4)
stem(n3,Out2)
xlabel('Time')
ylabel('Amplitude')
title('Discrete cross correlated waveform')

## OUTPUT:

<img width="703" height="622" alt="image" src="https://github.com/user-attachments/assets/4bc2caf7-e8ff-4221-a79b-7a22fc49ce38" />
<img width="751" height="688" alt="image" src="https://github.com/user-attachments/assets/fc2471f3-5674-427b-9c67-a1b25b513788" />
<img width="762" height="658" alt="image" src="https://github.com/user-attachments/assets/fd53d9ee-3c66-462a-a349-1b8caa4166cf" />
<img width="783" height="690" alt="image" src="https://github.com/user-attachments/assets/af1ec2e5-9666-4ee1-b1ff-e2718a6a1e6f" />

## RESULT:
<img width="1280" height="593" alt="image" src="https://github.com/user-attachments/assets/38e664d7-9ddd-405c-85e9-c02e96c0272b" />

