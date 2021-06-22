# PLC Project: 5 Way Switch Lamp

## Objective
The purpose behind this project is to get a hands-on introduction to Ladder Logic and ZelioSoft2. The objective is to write a PLC program to control a lamp’s state (ON/OFF) through the input of 5 switches.

## Environment
- PLC
- ZelioSoft2


## Procedure
1. Create a new project file using the largest PLC prototype (biggest number of input and output, 120 lines of code). Use the ladder entry layout to put the design components on.
2. Start by naming/commenting 5 switches (switch1, switch2 …) in the input section in ZelioSoft2. These will be the inputs used for the design.
3. Name one lamp (Q1) in the output section. This will be the only output used for this design.
4. Place the components on the ladder entry based on the planned design logic as shown below. The main focus while creating the program is to make sure to decrease the number of code lines and also the number of elements used. The final number of code lines I obtained is 6.
5. It is crucial while developing the code to write on each line comments explaining the program step by step so that if this project is handed over to another colleague it becomes easy to understand, work upon and perhaps develop further.


![1](https://user-images.githubusercontent.com/86275885/122980696-55d84700-d36f-11eb-8e73-da3b7ac18dd3.png)


## Discussion
The Ladder code is tested by running a simulation on ZelioSoft2 using the “Run” button on the top right. The simulation will pop 2 panels one for input switches and one for output lights. We can then try a series of combinations using the 5 input switches intended for the design and validating the outcome
by checking if the light on the intended output lamp is being turned ON or staying OFF accordingly. A sample run is shown below.

- Lamp ON simulation:

![2](https://user-images.githubusercontent.com/86275885/122980921-9b950f80-d36f-11eb-8062-8d71ebbba1ab.png)
![3](https://user-images.githubusercontent.com/86275885/122980944-a0f25a00-d36f-11eb-9788-7bb6f059563c.png)
![4](https://user-images.githubusercontent.com/86275885/122980958-a485e100-d36f-11eb-9cfe-a9428fb3d88d.png)


We can notice that the lamp is ON and the red line represents successful logic flow from left to right. Q1 is ON and the pressed switches (ON) are I1, I2 and I4 (switch1, switch2 and switch4) which represent 3 ON switches, an odd number. This validates the intended logic design for this project.

- Lamp OFF simulation:

![5](https://user-images.githubusercontent.com/86275885/122981167-d5661600-d36f-11eb-907f-d6a5224a7e5d.png)
![6](https://user-images.githubusercontent.com/86275885/122981177-d7c87000-d36f-11eb-8760-b7fd0cf3fc33.png)
![7](https://user-images.githubusercontent.com/86275885/122981187-d9923380-d36f-11eb-87ba-3c19a790992b.png)



We can notice that the lamp is OFF and the red line representing the logic flow from left to right is broken on way to reach lamp. Q1 is OFF and the pressed switches (ON) are I2 and I4 (switch2 and switch4) which represent 2 ON switches, an even number. This validates the intended logic design for this project as it requires an odd number of ON switches in order to turn ON the lamp (Q1 output light).

We can try on various cases to fully test the design. The designed logic must validate all theoretical cases in order to be 100% working. This can be verified by running several tests.


## Conclusion
This project introduced us to ZelioSoft2 and its various components. We built a simple project to get a grasp of the Ladder programming language. The efficiency of the design can be observed by looking at the number of line codes and elements used, of course, the design must be as efficient and compact as possible and most importantly must be 100% working. This aspect comes handy for later larger projects where we cannot afford to waste lines out of the total available 120 lines. 
