# EXPERIMENT - 1
Question : Given that power , p= 100µ W; Perform DC Analysis, Transient Analysis and AC Analysis for the Given Circuit Designs and also check what happens when the width is increased or decreased of each mosfet;
# Design -1 :
![Screenshot 2025-02-17 101931](https://github.com/user-attachments/assets/52d87604-4c88-4d3e-92fb-c0d4273054e8)
Aim : To find DC operating point , find its gain using transient analysis and AC analysis.
Components : Mosfet , resistors , DC power supply .
Procedure :
* make the circuit connections as shown above.
* Connect the RD resistor to the drain terminal  and DC power supply to the gate terminal as well as to the resistor
* Connect the source terminal to the ground .
* Set the input voltage to 0.9v and VDD to 1.8v.
* Using formula for power ,
  P=V*I
  we will get the values of Id as ,
  Id = 5.56*10^-5A
  we have to get the output current , Id for the given circuits by adjusting the values of L and W
  Length and Width of a channel implementing new values is shown in the below figure
![Screenshot 2025-02-17 100438](https://github.com/user-attachments/assets/bc990a3d-da5a-49c2-b05b-4200d247ccc0)
1.DC Analyis :
  Preocedure :
  * we have to select the dc output print (DC op pnt ) in the Edit Simulation Command and run the simulation . 
![Screenshot 2025-02-17 100514](https://github.com/user-attachments/assets/21e5a6b7-88f2-4a5f-b28b-e5cdc91181f6)
The Below Content shows the Values obtained from the DC Analysis :
2. Transient analysis :
 Procedure :
* we have to slect the Transient analysis command in the edit simulation command
* Give the stop timeas 1msec
* Run the simulation.
The Graph below shows the response of transient analysis :
![WhatsApp Image 2025-02-17 at 15 03 18_911a70d7](https://github.com/user-attachments/assets/d19ea1f3-4c15-499a-a730-9ff76134c1b0)
3. AC Analysis :
  Procedure :
  * we to select the AC Analysis in the simulation command tab .
  * give the sweep value , number of points per decade , and frequency range


 The graph below shows the AC analysis Data of the deisgn :
    

      


   


