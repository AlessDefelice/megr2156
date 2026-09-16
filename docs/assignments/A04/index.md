# A4 – Motor Mount

## Objective
This week we are tasked with designing a motor mount for an electric motor.
the Bracket is L shaped, connecting to a wall on one side and housing the motor on the other.
We are instructed to design based on beam deflection, and stresses incurred due the load on the motor's shaft.
Before I did any calculations, I drew out an FBD, and picked some baseline geometry to allow the part to function as intended.


## Analyze
I used the Machinery's Handbook to find the beam deflection and stress calculations, and solved for the Area Moments of inertia required by by design.
I used a few assumptions to streamline the process. The base was a function of the height, using the rough dimensions as a baseline.
I also negated the compressive stress from the force, focusing on the bending effects of the moment. 

<img width="2252" height="4000" alt="20260915_201033" src="https://github.com/user-attachments/assets/148d4223-fd2d-4d18-98e5-4e2dbddc1b20" />

<img width="2252" height="4000" alt="20260915_201039" src="https://github.com/user-attachments/assets/5cd3ae55-ca21-4190-b619-d0620d5a6735" />

I Had to perform this calculation twice, independently verifying the bending stress and deflection.


## Decide
I then went back to the original view of the part and edited my dimensions. I found the base min to be 2.4mm and I then chose 2.5 to use a nice square design. I calculated my safety factor to be 1.157, allowing the part to function as intended but leaving little room for error.

## Communicate
I found an effective way to define the dimensions of my part using the stress and deflection approximations found in the machinery's handbook.
My factor of safety is reasonably low. reflecting on my design, I would include a min FS of 1.5 in my calculations, allowing me to create a more real-world product.
