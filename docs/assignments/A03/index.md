A3 – Parametric Modeling and FEA

## Objective

The Objective is to parametrically design a circular aluminum bar that will satisfy the following specifications. We are limiting our axial deflection to 9 thousandths of an inch. We are also given a Load of from 300 to 500Lb, and a young's modulus of 8.5 to 11.5E^6 Psi. We are then tasked to pick a reasonable area for the bar. When Modeling, I chose 7075 Aluminum as it's young's modulus was very similar to my calculations. The deflection is set and since length and area inversely affect delta, I went with a smaller area so that my bar did not get too unreasonably long. Rearranging the delta= PL/AE equation, I chose a 1-inch diameter bar and then solved for the length.

<img width="2172" height="3102" alt="20260908_001257" src="https://github.com/user-attachments/assets/d391ea1f-b993-4147-bf05-4297282bd404" />

I then started my design in CAD. I started with my equations, and I wrote out my variables, again solving for the maximum allowable length of the bar. 

<img width="959" height="505" alt="Screenshot 2026-09-07 233601" src="https://github.com/user-attachments/assets/37ce9cd9-a2d6-43e6-b910-5549b6ccebbf" />

The global variable for length was then assigned to the length of the bar.

<img width="956" height="505" alt="Screenshot 2026-09-07 233701" src="https://github.com/user-attachments/assets/657f4f93-4efa-4d40-86a0-7a01e0d9008c" />




## Analyze

The first thing I did was set up my study, I assigned a fixture to the rear and used the reverse direction box to add a tension force of 400Lb to the nose of the rod.
<img width="956" height="503" alt="Screenshot 2026-09-07 232159" src="https://github.com/user-attachments/assets/e1edc974-e495-4e4d-8b55-1393f0b0e59d" />
<img width="957" height="506" alt="Screenshot 2026-09-07 232131" src="https://github.com/user-attachments/assets/94ae7631-b034-4d76-8e23-448a84bbc7e4" />

I then created a mesh and ran the study.

## Decide
<img width="959" height="503" alt="Screenshot 2026-09-07 233720" src="https://github.com/user-attachments/assets/7032e761-8a92-4ef2-b854-58b7a3bfd9e8" />

My Von Misses plot looked very strong, with low levels of stress. This gave me a very high factor of safety, over 132 times my yield strength. 

<img width="959" height="506" alt="Screenshot 2026-09-07 233821" src="https://github.com/user-attachments/assets/509aaf7a-8fe3-40e2-8c4c-4fb892419a83" />

My Deflection plot was very close to the maximum, but still fell within acceptable levels due to the small differences between my calculations and the actual vaulues.

## Communicate

Although my calculations were very close, there was still a 3.89% difference between my calculated deformation and the modeled deformation.
This is mainly attributed to the difference in the young's modulus when using a simple, rounded number in scientific notation.

I believe 3.8% to be a low enough difference to trust either calculation. However, this is because the beam is very simple and there are no geometric features affecting the stress levels. For a more complicated part I would trust SolidWorks as it is considering many more variables than I can.

below is my file
[A03](A03.SLDPRT)

