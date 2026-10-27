# A7 – Finite Element Analysis

## Objective
The Objective this week is to conduct finite element analysis to our A06 bracket design. We will be running an inner and outer loop process where we document convergence and analyze our study results to make changes to the bracket. We use the formula 2*[X_i-X_f]/[X_i+X_f] to calculate our mesh convergence. After attaining convergence, I was able to analyze the results of my static study to make geometry changes giving us a much stiffer and stronger bracket.

## Analyze
I began by setting up my static study on my A06 bracket

<img width="770" height="343" alt="Screenshot 2026-10-26 204704" src="https://github.com/user-attachments/assets/fc3c7039-f074-4127-8968-5afbddb96d2f" />

I ended up shifting from a full roller as the design had required to a fixed geometry on the top plates so that SolidWorks had a fully restrained model.

After running my first study even with a very coarse mesh it became instantly clear to me, even with lots of design work our full product can behave very differently.

<img width="532" height="311" alt="Screenshot 2026-10-26 210510" src="https://github.com/user-attachments/assets/2edf4c2b-13b3-441e-b061-f617b9b75da3" />

This is the coarse mesh version of my first draft and even with a coarse mesh my safety factor was extremely low at 0.46, this indicates the bracket would instantly fail under loading.

I had to edit my mesh quality 3 times for such a flimsy part to attain convergence, but my third attempt showed a 0.49% convergence at a 0.42 safety factor.

<img width="2076" height="2980" alt="20261026_231040" src="https://github.com/user-attachments/assets/389237f6-e705-4bc4-b788-4bd1e8036752" />

From here I had a working system, and I began to make decisions about my part's geometry.

## Decide
I carefully analyzed the results from my first FEA and I saw two main areas of issue. The first was the lever arm connecting the rod to the body of the part, its where my low safety factor came from. The second, is that the whole rest of my part was fully green, meaning i had lots of wasted mass in other areas. So the first step was pull some mass from areas of the part that I could, and then I put an additional support on the lever arm.

<img width="667" height="367" alt="Screenshot 2026-10-26 224856" src="https://github.com/user-attachments/assets/cbdc0052-c7d4-4273-8123-10b1cbdab2c9" />

I reduced my mesh size to begin with, and since I had a much more well supported part the second time I ran the mesh I had a 6.4% error, and so I had effectively achieved convergence. I believe if this was my final part I would have started even higher, but as a middle step I could easily see my areas of issue. 
I tried for some time to reduce the stress concentrations that built up at the base of the body, but I ultimately found that adding mass to the base of the part increased our stiffness to an acceptable level.
for my third run, I trimmed the edges of the part further and reduced the size of the lever-arm and the rod to its minimum dimension. my first run showed that the part had a much more consistent stress-level throughout. My second showed a convergence error of 2.8%, showing my design and my system was effectively optimized for the part I was working on.
final stress levels:

<img width="666" height="344" alt="Screenshot 2026-10-26 232129" src="https://github.com/user-attachments/assets/897f7782-cbd1-4bc9-ab67-c071b09aa65a" />


## Communicate
I thought I had parametrically designed the part to function in an optimized manner, but I was extremely wrong. My first real data after convergence showed my part was LESS THAN HALF as strong as it should be. Finite Element Analysis is an extremely powerful tool that allowed me to nearly triple my strength and stiffness, and reduce my weight by roughly 50%. I was surprised How much a convergence error changed my data, but I had a effective tool to optimize that as well.

Below I've embedded my CAD file, optomized:



