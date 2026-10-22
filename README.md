# StateFlow-Chart-_-Traffic-Light----Simulink
This project is targeted at exploring the Stateflow library of the Matlab/Simulink. 

This Stateflow Chart models a traffic light. The light switches between red, yellow, and green based on a timer. If a fault occurs, the light stops cycling and flashes red.

## Task 1
The light switches between red, yellow, and green based on a timer. If a fault occurs, the light stops cycling and flashes red.
To see the chart behavior more clearly, you can change the animation speed of the chart.
Then click the Debug tab in the toolstrip, and use the dropdown menu to change the Animation Speed setting from Fast to Medium.

## Task 2
The transition conditions determine the timing of the traffic light. 
To modify the condition, change the condition after(10,sec) to after(15,sec). This changes the duration of a green light to 15 seconds. 
To save time, set Animation Speed to Fast.

<img width="436" height="292" alt="Screenshot (849)" src="https://github.com/user-attachments/assets/f15ff198-3e76-4a38-b1aa-044e36207d35" />

## Task 3
Since Stateflow charts are blocks in a Simulink model, the chart receives and sends data using ports, like other Simulink blocks. For example, you can connect the output of a Stateflow chart to a Scope block to visualize the output signals.
Branch the red signal to the Assessment Block, and then click run to assess that signal.
<img width="919" height="568" alt="Traffic_light - Stateflow" src="https://github.com/user-attachments/assets/de3d1f3f-9ca3-46cd-9512-0d741df846c1" />

# Temporal Logic
Stateflow supports using temporal logic conditions based on elapsed time. A common temporal logic operator, which has been considered already, is after(N,sec), where N is the wait time in seconds. Charts in Simulink track time according to the simulation time of the model. 

## A PLOT TWIST 
Let me design a chart that contains the states and transitions that describe a traffic light. Then, add delays to the transitions as follows:

Stop → Go: 3 seconds
Go → PrepareToStop: 10 seconds
PrepareToStop → Stop: 3 seconds

<img width="439" height="639" alt="Stateflow Chart _ Traffic Light" src="https://github.com/user-attachments/assets/9c7cee24-011d-47c6-8302-2b708bd12c40" />

<img width="1102" height="848" alt="Graphical representation" src="https://github.com/user-attachments/assets/3b5b963c-7444-451f-a608-779940087c86" />

# Fault Response in the Model

I am also consider a more practical traffic light which involves fault detaction. 
Note that you can navigate to the Simulink model to see how the traffic light behaves in response to faults at various times. The Scope block shows you the fault signal. To choose a different test case, double-click the Signal Editor block. 
NB: The file is found in the link below 
https://github.com/Ebenzbelo/StateFlow-Chart-_-Traffic-Light----Simulink/blob/main/Project/Fault%20Response%20Project%20-%20Traffic%20Light.slx
