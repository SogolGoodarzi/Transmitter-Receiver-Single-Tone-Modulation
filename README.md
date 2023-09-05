![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/7077f6eb-c0d9-4dd6-b54e-27914b638e18)# Transmitter-Receiver-Single-Tone-Modulation
## Transmitter
### Phase Modulation
1. <p align="justify"> Implement a function named pm() that accepts the signal of the frequency message and the amplitude $\Phi_{\Delta}$ (and other required inputs) as input and outputs the modulated signal using the PM method. </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/f2676f9e-e460-43df-b929-c58c4dcb55e8)

2. <p align="justify"> Write a function named nbpm() that by taking the same inputs as pm() (and other required inputs) will output a modulated signal with the narrow band approximation or the same NBPM method. </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/6496cf8f-aac3-429e-b95b-dfadbd859c58)

3. Now give the following values ​​as inputs to the above two functions and plot the outputs. Then calculate the mean square error of NBPM relative to PM.

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/a8170cbe-cf88-4ebe-be8d-14586b87f26b)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/bdf2a1b0-86b0-498b-9fd6-c9421a8f1101)

<p align="justify"> Now, to calculate the mean square error, we use the immse() function and give the output of the above functions as input to this function. The mean square error value is as follows: </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/ab7871e0-751f-4da6-af26-d5f5bdf7fe52)

4. Repeat step 3 for $\Phi_{\Delta}$ = 0.01. Compare the error found with part 3 and explain the difference.

This time we reduce the value of the parameter $\Phi_{\Delta}$ to 0.01. The output diagram of the two mentioned functions is as follows:

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/0de393d9-e7bd-4f5d-b80e-13308e681858)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/38887c99-0fc5-4ca0-ae5d-eebfa6e5720a)

**Justifying the difference in errors:**

<p align="justify"> As we learned from the relationships mentioned in the lesson, we saw that in order to obtain the narrowband phase modulation relationship, the Taylor series of in-phase and orthogonal signals of the message signal was written. With a good approximation, if the value of $\phi (𝑡)$ is smaller than 1, the first sentences of the series can be included and the subsequent sentences can be ignored. This approximation gives the correct value for the narrow band phase modulation, which is modulation with this condition has an output very close to the output of phase modulation. So, in the previous case, when $\Phi_{\Delta}$ = 10, this approximation was correct in ignoring Taylor's series sentences and caused a striking difference in the output of two functions pm() and nbpm(), but in this case, because $\Phi_{\Delta}$ = 0.01 and
is smaller than 1, so the approximation of considering the first terms of the Taylor series and ignoring the rest of the terms is correct, and we see that the output of the functions in this case are very similar. On the other hand, the error of the first state is more than the second state, which indicates that the mentioned condition for $\Phi_{\Delta}$ is not fulfilled in the first state. </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/3f571b21-010a-4204-a8a2-3ce3fd883304)

5. <p align="justify"> This time, use the ready MATLAB program (pmmod) for PM modulation and give the values ​​of sections 3 and 4 as input to the program. Finally, plot the output graphs. Compare the output shape with the functions you implemented yourself. </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/8e66ae49-61a2-4e43-b8d2-5849b023d130)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/0cdd0024-2653-4659-bac5-d5935d3b60a8)

6. Report the average error rate only for the inputs of section 3 and between the outputs of the two functions pmmode() and pm().

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/bb181bd6-e4c3-42b9-9b58-993893797680)

<p align="justify"> As it is known, this error is zero, so it can be concluded that the performance of the MATLAB ready function for phase modulation is similar to the performance of the function that we wrote using the relations of the lesson. </p>

### Frequency Modulation
7. <p align="justify"> This time, implement functions with the names fm() and nbfm() that accept the signal of the frequency message and the amplitude of the amplitude $f_{\Delta}$ (and other required inputs) as input, and respectively the modulated signals using the FM method and the narrowband approximation, or the same Output the NBFM method. </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/a9dde012-7d82-4bcc-a3ae-edc801ac1d29)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/0af67143-2d56-4a5a-9fe2-ae6d32dda068)

8. Give the following values ​​as inputs to fm() and nbfm() and plot the outputs. Then calculate the average error rate of NBFM compared to FM.

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/c755a2cd-8596-42f7-91d6-b322a562b732)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/714ebcc2-3010-424d-a3ce-ecceb8ad9c05)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/0eb59062-e465-4d14-bfb0-817ca3e718f6)

9. For $f_{\Delta}$ = 0.01, we do the same as the previous part. The output graphs are as follows:

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/6083cc6a-e4d1-41c7-8fa5-591bdc737098)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/66b4e93d-01ed-4a7c-ac04-49604a80eb7f)

<p align="justify"> As it is known, the calculated error value for $f_{\Delta}$ = 10 is higher than the value of this error for $f_{\Delta}$ = 0.01. The reason for this is the same justification as we said for the phase modulation part. In the case of phase modulation, we said that if $\Phi_{\Delta}$ is much smaller than 1, the Taylor series approximation is correct. In this section, it can also be said that when $2\pi f_{\Delta}$ is much smaller than the value of 1, it is approximated for the Taylor series, the in-phase and orthogonal part of the message signal is correct, so for $f_{\Delta}$ = 0.01, we see that with a very good approximation, the two output signals are similar and the error is very low, but for $f_{\Delta}$ = 10, because the mentioned condition is not true, the error value is higher. </p>

10. <p align="justify"> This time, use MATLAB's fmmod (fmmod) tool for FM modulation and give the values ​​of the parameters 8 and 9 as input, give the input to this curve and plot the shape of the output graphs. Compare the output shape with the functions you implemented yourself. </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/19c51aca-09b5-4be5-885e-3db7ba6aae65)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/4b2f8064-4c61-4e51-aac1-0ff3c74dc988)

11. Now we get the mean square error for $f_{\Delta}$ = 10 as follows:

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/bcda07b4-ed07-420e-8a81-90863abf0764)

<p align="justify"> As it is known, this error is small, so it can be said that the frequency modulation with the function we wrote is similar to the modulation performed by the ready-made function of MATLAB with a good approximation. </p>

12. <p align="justify"> Change $\Phi_{\Delta}$ and $f_{\Delta}$ in the interval [0,1] )with an arbitrary and small enough step length) and calculate the mean square error for two normal and narrowband modulations (the use of ready-made MATLAB software for modulation is not allowed). Assuming that the maximum acceptable error is 1%, report the maximum $\Phi_{\Delta}$ and $f_{\Delta}$ . </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/3c45bc09-e382-4402-844c-9f1583cd174c)

<p align="justify"> Considering that the maximum accepted error is equal to 1%, then we must find the phase in which the error value is 0.01 or less but has the highest value. With the find command, it is possible to calculate the maximum phase in a suitable way. </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/91cd7570-554c-4734-ab83-ac68caad7492)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/aa234eb5-c8fb-4ba1-8441-580fe1f3e1b9)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/6962cc39-699e-438c-b8a1-70e6ca377a51)

## Receiver
### Frequency Modulation

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/fde0db2a-841b-4d19-8660-8f6d9d8e1b2a)

1. <p align="justify"> We know that the output of the above circuit is a multiplier of the message. Report this coefficient by writing the mathematical relations of the block diagram above for an arbitrary message m(t). </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/96d50b43-3fe1-4c4b-9e90-87c71f869463)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/542a17de-8801-485e-9dde-a0e9f59bd598)

2. <p align="justify"> Write a function named fdm() that takes the FM signal frequency and amplitude $f_{\Delta}$ and the sampling frequency (and other inputs of your choice) as input and output the revealed message using the block diagram method. Note that the output should not be a multiple of the message and you must correct the output according to the coefficient you mentioned in section 1. </p>

<p align="justify"> We have implemented the desired function step by step using the given block diagram. First, we have put a variable named shifted-xc for the derivative block, which actually represents the shift of xc findings, or better said, it contains the sentences that are supposed to participate in the definition of the derivative in the differential term. Then, in the next step, we calculate the result of the difference of this variable from the xc values ​​themselves, and finally divide it by the length of the steps between the two xc values. The length of xc steps is equal to the inverse of the sampling frequency value, which represents the same point distance as defined in the definition of the variable t for the previous sections. The implementation of the derivative is done using the following relationship: </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/8abd71a6-d5e9-48fa-b3f8-41e26ad6bd30)

<p align="justify"> Now, for the envelope detector block, we use the function (envelope) in MATLAB. The outputs of this function give the upper and lower ranges, which here, due to the symmetry of the message signal, it does not matter which one of these outputs is ignored. To remove the DC value of the signal, we must subtract the DC term, $A_c w_c$ from the output of the function envelope(). Finally, we divide the resulting output by k to obtain the original signal. The process mentioned in the function written in the code file can be seen: </p>

3. Input the output of fm() in part 8 of the transmitter section to fdm() and compare the output with the original message signal.

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/99fc90bf-5535-4371-bf23-3b0c1040be5c)

<p align="justify"> According to this diagram and the diagram of the original message signal, it is clear that the output signal of the function is correctly recovered and a signal similar to the original message signal can be found in the output. In terms of amplitude and period, we can see that both the original signal and the recovered signal are similar, so the function we have written is correct. </p>

4. This time, take the help of MATLAB's fmdemod() function for demodulation and repeat part 3. Compare the output with your written function output.

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/d07293bc-8c69-4786-bb5c-32921d755c71)

### Phase Modulation
5. <p align="justify"> If we want to use the block diagram of the previous part to reveal the PM signal, what block should we add to the end of it? Plot your proposed block diagram in your work report and write its mathematical relationships to reveal the PM signal. If there is a coefficient of the message in the output, report this coefficient. </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/07303927-62ea-41a3-9178-2ee8cabed06a)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/4ce9f946-a328-4a63-a643-4bc408111ff1)

6. <p align="justify"> Simulate this new block and implement a function called pdm() with the help of fdm() that takes the PM frequency signal and the amplitude of $\Phi_{\Delta}$ and the sampling frequency (and other required inputs) as input and outputs the primary message signal. Note that the output should not be a multiple of the message and you must correct the output according to the coefficient you mentioned in section 5. </p>

<p align="justify"> Because a part of the block diagram plotted in the previous part has been added by the fdm() function, it is enough to first send the modulated PM signal to the fdm() function and give the output to the last block, the integral trap, and it is done with the cumtrapz() command and the resulting output is the signal of the desired and recovered message. </p>

7. Input the output of pm() in part 3 of the sender section to pdm() and compare the output with the signal of the original message.

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/82bdab02-73ea-467a-83a0-fd1165b5624f)

8. This time, take help from MATLAB's ready-made function pmdemod() for demodulation and repeat part 7. Compare the output with your written function.

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/2d19ec6d-5826-4569-bb9e-c025dd757df8)

<p align="justify"> We can see that the output of the MATLAB function and our function are not the same. The reason is that the value of $\Phi_{\Delta}$ was too large in this case. So, it can be said that if the value of this parameter in the modulated signal is smaller than a certain limit, the output of the MATLAB function will match the output of our function with a good approximation. </p>

<p align="justify"> The MATLAB function works in such a way that it uses the phase detector or Phase Comprator for phase demodulation. As we have seen in this section, since the demodulation of a signal modulated by the PM method may not be done correctly, then it can be said that one of the applications of modulating messages in this way is in the field of sending military and confidential messages, because demodulation is difficult to create such messages and often times, like this section, the correct answer will not be the result. Due to the difficulty of phase demodulation, it can be said that FM modulation is used in most other fields, such as the same radio signals, which, if you look carefully, have never seen a PM signal in this field. </p>

## Tone Modulation
<p align="justify"> A message signal that has only one specific frequency and is modulated by using phase-frequency modulators will be called single-tone modulated signal. For example, for a sinusoidal message with modulation index, the modulated $\beta$ signal will be obtained as follows: </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/c3b34119-664e-4ed3-bb0e-f2a5f6a5814d)

<p align="justify"> As you know, with the increase in the order of the bessel wave for a narrow-band signal ($\beta$ >>1), the value of the bessel wave tends to be higher. For this reason, it is not necessary to calculate all the sentences in the above sentences. On the other hand, we know that by increasing the value of $\beta$, the size of the reward will increase to a higher order and will no longer be negligible. </p>

1. Consider the following message signal:

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/8e096bf1-696e-432e-aa45-f755d39f9b7a)

For the following values of $\beta$ modulate the signal and plot the spectrum in Hz.

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/371eee4e-0594-4ef5-988b-0e9956c13778)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/12a75ca6-12bb-4854-a119-2a4596735b8f)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/9863e860-c492-4aea-b108-200ad347811a)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/b238a772-dae9-4dc9-a39c-76e6030379a3)

**The reason for widening the frequency range:**

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/90ef07d6-a971-454e-8f8e-1c2e5be64723)

<p align="justify"> Since the value of $f_m$ does not change and has a constant value of 10 Hz and $A_m$ is also constant, so with the increase of beta, the value of $f_{\Delta}$ also increases and as it was said in the lesson, in this case the bandwidth will increase. According to the graphs above, it can be seen that with the increase of the beta bandwidth of the Fourier transform, the output signals have increased. </p>

2. <p align="justify"> According to the approximate bandwidth of the modulated signal, choose N in such a way that the functional expansion of the signal can be approximated as below, then for the modulation indexes of paragraph 1, use the expansion below to modulate the signal and plot its frequency spectrum. Compare the spectra plotted in part 1 with part 2. For this, it is recommended to plot and analyze two spectra in one graph. </p>

<p align="justify"> For this part, we have to implement the right side of the given equation, so we need to use Bessel functions. For the code of this section, we implement the given relation with a loop so that we implement the relation for different n's that we obtained later through Bessel functions. </p>

<p align="justify"> First, we need to find the appropriate N according to the bandwidth of the signals in the previous part. For this purpose, we can use the graph of the Bessel function for different levels, and based on the beta value we have, we can get the level needed to implement this relationship. </p>

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/88691a43-35f4-45ab-ab23-207845a5260a)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/a45a241f-9229-4baa-a82f-1cace0070967)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/95e3e04b-1ef4-48db-989f-f02d34b494b8)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/bc44c837-95b2-4f69-9c85-8e0d392267e8)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/2fa46131-c4d6-4c12-8e8c-b32487132f82)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/8832a15e-d0a7-4f44-a1aa-f8c0c4501693)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/3f24d56a-75db-4cae-92b7-be0a16f2ad31)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/cdd866cb-259e-437c-9442-72bfd12d19f7)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/3190d972-2112-4aa3-9752-515696a6eb15)

![image](https://github.com/SogolGoodarzi/Transmitter-Receiver-Single-Tone-Modulation/assets/125180530/887a355a-63ab-4097-bc99-80c571196027)

**Overall result:**

<p align="justify"> According to the graphs plotted and the similarity between them, it can be concluded that the two sides of the given equality are equivalent for single-tone signal modulation, so it can be said that the expansion we wrote using Bessel functions to modulate the signal (that is, the same expression on the right side of the equality), works well for single-tone signal modulation and can be used for male modulation. </p>
