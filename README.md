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


