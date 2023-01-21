# Experiment-08- Encoders-and-decoders 
### AIM: To implement 8 to 3 Encoder and  3to8 Decoder using verilog and validate its outputs
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## Encoders
Binary code of N digits can be used to store 2N distinct elements of coded information. This is what encoders and decoders are used for. Encoders convert 2N lines of input into a code of N bits and Decoders decode the N bits into 2N lines.

1. Encoders –
An encoder is a combinational circuit that converts binary information in the form of a 2N input lines into N output lines, which represent N bit code for the input. For simple encoders, it is assumed that only one input line is active at a time.

As an example, let’s consider Octal to Binary encoder. As shown in the following figure, an octal-to-binary encoder takes 8 input lines and generates 3 output lines.

![image](https://user-images.githubusercontent.com/36288975/171543588-bc0746df-a173-4b35-989e-5fb7d385fe8a.png)
## Figure -01 3 to 8 Encoder 


Implementation –

X = D4 + D5 + D6 + D7
Y = D2 +D3 + D6 + D7
Z = D1 + D3 + D5 + D7 
Hence, the encoder can be realised with OR gates as follows:


![image](https://user-images.githubusercontent.com/36288975/171543740-68403b82-aa93-4c98-9343-f32b14885a2e.png)
## Figure -02 3 to 8 Encoder implenentation 

 ### Decoders 
A decoder does the opposite job of an encoder. It is a combinational circuit that converts n lines of input into 2n lines of output.

Let’s take an example of 3-to-8 line decoder.
Implementation –
D0 is high when X = 0, Y = 0 and Z = 0. Hence,

D0 = X’ Y’ Z’ 
Similarly,

D1 = X’ Y’ Z
D2 = X’ Y Z’
D3 = X’ Y Z
D4 = X Y’ Z’
D5 = X Y’ Z
D6 = X Y Z’
D7 = X Y Z 


![image](https://user-images.githubusercontent.com/36288975/171543978-ee2d0671-2846-40a1-8705-507fd6287a49.png)
## Figure -03 8 to 3 Decoder 



![image](https://user-images.githubusercontent.com/36288975/171543866-5a6eace6-8683-49d7-9c4f-a7cb30ec3035.png)
## Figure -04 8 to 3 Decoder implementation 

### Procedure:





### PROGRAM 
/*
Program for Endocers and Decoders  and verify its truth table in quartus using Verilog programming.
Developed by: NIRAUNJANA GAYATHRI G R
RegisterNumber:  22008369 
![image](https://user-images.githubusercontent.com/119395610/213845782-7d308cf5-c2b9-4e7d-b5aa-06f39fb7db19.png)


*/






### RTL LOGIC :
![image](https://user-images.githubusercontent.com/119395610/213845685-09edb3d9-9ef4-47e6-b54e-59a7405aeed2.png)
![image](https://user-images.githubusercontent.com/119395610/213845694-a84e2260-5044-4fa7-bea0-93d176074d6f.png)









### TIMING DIGRAMS :
![image](https://user-images.githubusercontent.com/119395610/213845711-36c08851-9496-41c7-ac7e-9c2b2131b176.png)
![image](https://user-images.githubusercontent.com/119395610/213845731-791a2df2-9b75-4753-afd4-fd16a9932293.png)






### TRUTH TABLE :

![image](https://user-images.githubusercontent.com/119395610/213845738-92026ee9-e36e-47a0-856e-f5d8bba9e847.png)
![image](https://user-images.githubusercontent.com/119395610/213845744-badb3f8e-d5ac-4697-a31e-33f7cd6b5d72.png)






### RESULTS :


