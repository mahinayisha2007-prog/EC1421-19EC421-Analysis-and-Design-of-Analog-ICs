# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS

![WhatsApp Image 2025-11-21 at 17 19 36_06474192](https://github.com/user-attachments/assets/57303d9b-cee7-41f7-8434-22bc8a56b881)

## HIGH-PASS

![WhatsApp Image 2025-11-21 at 17 24 34_5193a2e1](https://github.com/user-attachments/assets/df8b462e-7780-44b6-9c87-c2b524c909a5)

## BAND-PASS

![WhatsApp Image 2025-11-21 at 17 27 43_0618de79](https://github.com/user-attachments/assets/335effea-50c9-41ad-b51c-715be07bbc92)

## MODEL GRAPH:
## LOW_PASS

![WhatsApp Image 2025-11-21 at 17 19 28_3bbe85c3](https://github.com/user-attachments/assets/bd458a21-3d49-4611-b546-f07af0e13123)

## HIGH-PASS

![WhatsApp Image 2025-11-21 at 17 24 35_c11af621](https://github.com/user-attachments/assets/66ac9150-5eb7-43f5-b84a-8ce9e5421cbd)

## BAND-PASS

![WhatsApp Image 2025-11-21 at 17 27 43_838d40fc](https://github.com/user-attachments/assets/c635a837-f6b8-41fb-b55a-246d68586134)

## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS

![WhatsApp Image 2025-11-21 at 17 19 27_f7ff7205](https://github.com/user-attachments/assets/56fd4ac4-e036-43d3-9243-96b34db4fe13)

## HIGH-PASS

![WhatsApp Image 2025-11-21 at 17 24 35_30146699](https://github.com/user-attachments/assets/f70ec8ed-23d1-41e9-ba8a-ccee1e6c4555)

## BAND-PAS

S![WhatsApp Image 2025-11-21 at 17 27 44_7cd9d3d8](https://github.com/user-attachments/assets/8a20e7be-f635-4145-9611-e49dc031925a)

## GRAPH:
## LOW_PASS

![517267720-568ce42f-d2b2-4add-96b9-96c97dc983f4](https://github.com/user-attachments/assets/76219a19-d4c4-41e8-aa02-d9ff04870178)

## HIGH-PASS

![517267765-ecf5a2e5-5a4a-4953-80cc-bc583629734a](https://github.com/user-attachments/assets/4937a3c0-9ab5-4b90-bfb8-7a340cf14cc7)

## BAND-PASS

![517267989-fac62900-8ded-4646-ab9a-fc34de606003](https://github.com/user-attachments/assets/9ab14687-6120-4c6a-a256-ad87e74a2b55)

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

