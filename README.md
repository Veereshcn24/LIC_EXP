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

  ![WhatsApp Image 2025-02-17 at 15 03 20_e31b1b51](https://github.com/user-attachments/assets/eb442a20-9fb9-45e3-9a17-adeb74a1f6f7)

* Run the simulation.
The Graph below shows the response of transient analysis :
![WhatsApp Image 2025-02-17 at 15 03 18_911a70d7](https://github.com/user-attachments/assets/d19ea1f3-4c15-499a-a730-9ff76134c1b0)

3. AC Analysis :
  Procedure :
  * we to select the AC Analysis in the simulation command tab .
  * give the sweep value , number of points per decade , and frequency range

    ![WhatsApp Image 2025-02-17 at 15 03 18_d86174d4](https://github.com/user-attachments/assets/52855383-3437-483f-a512-ec331b153404)

The graph below shows the AC analysis Data of the deisgn :
![WhatsApp Image 2025-02-17 at 15 03 18_099773b4](https://github.com/user-attachments/assets/7646c925-31b0-44cd-9108-3a4dc3a45488)
# Result [Design -1]:
1. DC Analysis :
   * The caluclated drain current matches the epected value based on power and voltage , 
   Id=5.56*10^-5 A.
   * By adjusting the MOSFETS channel Dimenssion the  current requirement was successfully 
   achieved
* The circuit behaves as same as we have expected in DC Analysis .
2. Transient analysis :
  * The graph sows how the circuits behaves over time .
  * The response is smooth  , with not much  diistortions .
  * The circuits behaves well as we change the parameters , which is a good way to measuring 
  its stability.
3. AC Analysis :
  * The AC response graph graph confirmms that circuits remains same for diffrent frequency  
  range .
  * The gain (-9.94dB) and phase shift of nearly 180 degree align with theoritical expectations.
  # Inference (Design - 1):
   * we came across how the changing of length and width of a mosfet can control the drain 
     current .
   * M1 has influenced on Id , Means its width affects the output current .
  # DESIGN - 2
  ![WhatsApp Image 2025-02-17 at 15 03 20_b3dba982](https://github.com/user-attachments/assets/8db5d795-8dda-4e4b-b719-0ec36154e2be)
   Aim : To find DC operating point , find its gain using transient analysis and AC analysis.
   Components : Mosfet(M! and M@) , DC power supply .
  Procedure :
* make the circuit connections as shown above.
* Connect the DC power supplly to the gate terminal.
* Connect he source terminal tot he ground .
* Select he input voltage by obtaining VTC curve and VDD to 1.8 V .
*  Using formula for power ,
  P=V*I
  we will get the values of Id as ,
  Id = 5.56*10^-5A
  we have to get the output current , Id for the given circuits by adjusting the values of L 
  and W of MOSFET's(M1 and M2).
DC SWEEP  analysis : This  done for obtainig thr value of Vin in saturation region limits .
* We have to select he DC SWEEP in the edit simulation command
* give the values as shown below
* run the simulation
* ![WhatsApp Image 2025-02-17 at 15 03 18_41cec47d](https://github.com/user-attachments/assets/0017f1cd-35c4-42ec-9754-420d7e4d37ea)
* The below graph shows the VTC curve and the value of vin selected as 0.8vmas it is in the 
  saturation region .
  
![WhatsApp Image 2025-02-17 at 15 03 16_b4c4ad36](https://github.com/user-attachments/assets/95af7f87-0168-4d89-97bf-79f9c1a00892)


  
* Then input voltage parameters is given as ;
  
![WhatsApp Image 2025-02-17 at 15 03 15_7145ce44](https://github.com/user-attachments/assets/71370c06-8971-4573-9ccc-c4ad242570d1)

  
  * Length and Width of a channel implementing new values is shown in the below figure
  ![WhatsApp Image 2025-02-17 at 15 03 19_5223c7b4](https://github.com/user-attachments/assets/7a6a860a-1205-4947-9aa3-8e09e5e6a5a1)

![WhatsApp Image 2025-02-17 at 15 03 17_eb71dd87](https://github.com/user-attachments/assets/99904c6f-cd29-453b-9093-798703b13b53)

1.DC Analyis :
  Preocedure :
  * we have to select the dc output print (DC op pnt ) in the Edit Simulation Command
  * run the simulation
    ![Screenshot 2025-02-17 100514](https://github.com/user-attachments/assets/374246fe-a6a8-4110-a49a-74bc88c7ce44)
    The Below Content shows the Values obtained from the DC Analysis :
    ![WhatsApp Image 2025-02-17 at 15 03 16_78b25881](https://github.com/user-attachments/assets/57631b5d-1eff-454e-9d59-2acba60d814f)
2. Transient analysis :
 Procedure :
* we have to slect the Transient analysis command in the edit simulation command
* Give the stop timeas 1msec
* Run the simulation.
  
  ![WhatsApp Image 2025-02-17 at 15 03 20_4a337758](https://github.com/user-attachments/assets/71005244-3eca-4373-8fe2-41335c82c110)

The Graph below shows the response of transient analysis :
![WhatsApp Image 2025-02-17 at 15 03 16_5aafe0b4](https://github.com/user-attachments/assets/17af4699-db7c-49e8-b380-ec93f83a6bab)
3. AC Analysis :
  Procedure :
  * we to select the AC Analysis in the simulation command tab .
  * give the sweep value , number of points per decade , and frequency range

    ![WhatsApp Image 2025-02-17 at 15 03 18_d86174d4](https://github.com/user-attachments/assets/52855383-3437-483f-a512-ec331b153404)

The graph below shows the AC analysis Data of the deisgn :

![WhatsApp Image 2025-02-17 at 15 03 15_fa3a2a17](https://github.com/user-attachments/assets/0ae1a709-c23a-4174-8040-a4e1829c1035)


# Result [Design -2]:
1. DC Analysis :
   *  The caluclated drain current matches the epected value based on power and voltage , 
   Id=5.56*10^-5 A.
   * By adjusting the MOSFETS(M1 and M2) channel Dimenssion the  current requirement was 
     successfully achieved ,
     M1 : L= 500nm , W= 950nm.
     M2 : L= 300nm , W= 1020nm.
2. Transient analysis :
  * The graph sows how the circuits behaves over time .
  * The response is smooth  , with not much  diistortions .
3. AC Analysis :
  * The AC response graph graph confirmms that circuits remains same for diffrent frequency  
  range .
  * The gain (3.8dB) and phase shift of nearly 180 degree align with theoritical expectations.
# Inference (Design-2):
* The experiment validates that by appropriately selecting the MOSFET dimensions (L & W), the drain current can be precisely controlled.

* The voltage transfer characteristics (VTC) helped in selecting the correct operating voltage (0.8V) for saturation.

* Impact of Width Adjustments:

M2 has a stronger influence on Id, meaning its width significantly affects the output current. Increase in width increases Id drastically and vice-versa.
M1 has a smaller influence, meaning changes in its width result in only minor variations in Id. Increase in qidth increases Id by small amounts and vice-versa.

* The design meets the expected performance criteria and follows theoretical predictions, demonstrating its feasibility in practical applications.
 







  

    

      


   


