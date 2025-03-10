# EXPERIMENT 3 - DIIFRENTIAL AMPLIFIER 
AIM: To analyze and design the DC,AC,Transient analysis of Common Source NMOS Amplifier
# Introduction:
It is the basic configuration of the MOSFET(Metal oxide semiconductor field effective transistor) where the input is given to the gate terminal and output is driven form the drain terminal and the source is grounded .This amplifier will give the significant gain which is ideally 1 and this amplifier will act as the buffer amplifier which as 180 degree phase shift. DC Analysis is used to determine the Q point in such a way that the transistor is operating in the saturtaion region. The AC analysis is used to determine the gain, amplifiers frequency response and the bandwidth of the amplifier.

# Design Question
Design differential amplifier for the following specifications
____
|Parameters |Vdd| P | Vicm | Vocm | Vp |
| ------------- | ------------- |
|Secifications| 2.5V| <=3MW | 1.3V| 1.4V | 0.5V|
____




Perform DC analysis transient analysis and frequency response and extract the required parameters


# Theory
A Differential Amplifier is an funadamental electronic circuit designed to amplify the difference between the two input signals while rejecting an Common-Mode signals that are present on the both input signals. This characteristic makes it highly effective in applications requiring noise reduction. The Differential amplifier typically consists of a pair of transistors configured in a symmetrical manner,allowing it to obtain high common-mode rejection ratio(CMMR)

# Circuit - 1 [With Rss]
![WhatsApp Image 2025-03-08 at 23 27 28_db8cb205](https://github.com/user-attachments/assets/bcf76ae7-76b4-40c7-96ef-ee92a336a51f)

# Design 

* Assume M1 and M2 are perfectly identical
* Vicm1 = Vicm2 = Vicm
* RD1 = RD2 = RD
* ID1 = ID2 = Iss/2
* VGS1 = VGS2 =VGS
* Vocm1 = Vocm2 = Vocm = 1.4V
 <br> Vicm = Vp + VGS </br>
       1.3 = 0.5 + VGS </br>
       1.3-0.5 = VGS </br>
       <table>
       <td>V<sub>GS</sub> = 0.8V</td>
       </table>
- we can conclude that VGS >= Vth , M1 and M2 are in ON state
- Given P = 3mW we can calucalate Iss
- Iss = P/VDD
- Iss = 3mW/2.5V
- Iss = 1.2mA
- we known that ID = Iss/2
       <table>
       <td>I<sub>D</sub> = 1.2mA</td>
       </table>
- Rss = Vp/I<sub>ss</sub> = 0.5/1.2m
    <table>
     <td>R<sub>ss</sub> = 0.416K</td>
     </table>
- V<sub>ocm</sub> = V<sub>DD</sub> - I<sub>D</sub>*R<sub>D</sub>
- R<sub>D</sub> = (V<sub>DD</sub> - V<sub>ocm</sub>)/I<sub>D</sub>
  - R<sub>D</sub> = (2.5 - 1.4)/0.6m
   <table>
     <td>R<sub>D</sub> = 1.833K</td>
     </table>
- we can conclude V<sub>ocm</sub> >= V<sub>GS</sub> - V<sub>th</sub>
   - V<sub>ocm</sub> = 0.8 - 0.36
   <table>
       <td>V<sub>ocm</sub> >= 0.44V</td>
      </table>
<br>Therefore M1 and M2 are in saturation region</br>
**DC ANALYSIS:-**


![WhatsApp Image 2025-03-08 at 23 27 27_198d79a7](https://github.com/user-attachments/assets/ddd76a31-62aa-414c-b39a-f99fb0693200)

## when the V<sub>icm</sub> level is 100mV lesser than the given value(1.3V)
- V<sub>icm</sub> will be 1.3 - 0.1 = 1.2V

![WhatsApp Image 2025-03-09 at 00 29 54_68ab410d](https://github.com/user-attachments/assets/81cc1856-77b0-42b7-ae50-e94f6b9bc282)
* We can conculde that when we decrease  the V<sub>icm</sub> then
    <br>**The **V<sub>ocm</sub>** will increase.**</br>
    <br>**The **I<sub>D</sub>** will decrease.**</br>
    <br>**The **A<sub>v</sub>** will decrease.**</br>
    <br>**The total current **I<sub>ss</sub>** will decrease.**</br>
    <br>**The nodal voltage **Vp** will decrease.**</br>

## when the V<sub>icm</sub> level is 100mV greater than the given value(1.3V)
- V<sub>icm</sub> will be 1.3 + 0.1 = 1.4V
![WhatsApp Image 2025-03-09 at 00 30 53_e3a881cb](https://github.com/user-attachments/assets/fd62799d-e4ee-451f-8e3b-bb1f5fb94b1b)
 


* We can conculde that when we inrease  the V<sub>icm</sub> then
    <br>**The **V<sub>ocm</sub>** will decrease.**</br>
    <br>**The **I<sub>D</sub>** will increase.**</br>
    <br>**The **A<sub>v</sub>** will increase.**</br>
    <br>**The total current **I<sub>ss</sub>** will increase.**</br>
    <br>**The nodal voltage **Vp** will increase.**</br>

 <table>
     <tr>
        <td>V<sub>icm</sub> (V)</td>
        <td>V<sub>ocm</sub> (V)</td>
        <td>I<sub>D</sub> (mA)</td>
        <td>V<sub>p</sub> (V)</td>
        <td>I<sub>ss</sub> (mA)</td>
        <td>A<sub>v</sub> (V/V)</td>
     </tr>
     <tr>
       <td>1.2</td>
       <td>1.54</td>
       <td>0.52</td>
       <td>0.434</td>
       <td>1.04</td>
       <td>4.069</td>
     </tr>
     <tr>
       <td>1.3</td>
       <td>1.4</td>
       <td>0.6</td>
       <td>0.5</td>
       <td>1.2</td>
       <td>5</td>
     </tr>
     <tr>
       <td>1.4</td>
       <td>1.25</td>
       <td>0.67</td>
       <td>0.566</td>
       <td>1.3</td>
       <td>2.799</td>
     </tr>
  </table>
- **Transisent Analysis:**
  - A<sub>v</sub> = -g<sub>m</sub>*R<sub>D</sub>
    - g<sub>gm</sub> = (2*I<sub>D</sub>)/(V<sub>GS</sub> - V<sub>th</sub> )
    - g<sub>gm</sub> = (2*0.6m)/(0.8-0.36)
    - g<sub>gm</sub> = 2.77m
  - A<sub>v</sub> = - 2.7m * 1.83K
    <table>
      <td>A<sub>v</sub> = - 4.99V/V</td>
    </table>
- simulation

 ![WhatsApp Image 2025-03-09 at 00 19 20_b442cab2](https://github.com/user-attachments/assets/51ce51e2-d7b7-4012-9fb5-27d87c6fe055)

- from simulation the differential gain will be A<sub>vdm</sub> = (V<sub>ocm1</sub> - V<sub>ocm2</sub> )/(V<sub>icm1</sub> - V<sub>icm2</sub>)
   -  A<sub>vdm</sub> = 452.87mV/100mV
  <table>
     <td>A<sub>vdm</sub> = 4.528V/V</td>
     </table>
 - To find Max and Min Swing 
     - V<sub>icm min</sub> = V<sub>th</sub> + Vp
     - V<sub>icm min</sub> = 0.36 + 0.5
     - V<sub>icm min</sub> = 0.86V
     - V<sub>icm max</sub> = V<sub>DD</sub> - (I<sub>D</sub>*R<sub>D</sub>) + V<sub>th</sub>
     - V<sub>icm max</sub> = 2.5 - (0.6m*1.833k) + 0.36
     - V<sub>icm max</sub> = 1.7602V
     - V<sub>icm</sub>max swing = (0.86 + 1.7602)/2
       <table>
         <td>V<sub>icm</sub>max swing = 1.310V</td>
       </table>
    - V<sub>ocm min</sub> = V<sub>ov1</sub> + v<sub>p</sub>
    - V<sub>ocm min</sub> = 0.8 - 0.36 + 0.5
    - V<sub>ocm min</sub> = 0.94V
    - V<sub>ocm max</sub> = V<sub>DD</sub> - I<sub>D</sub>*R<sub>D</sub>
    - V<sub>ocm max</sub> = 2.5 - (0.6m*1.83K)
    - V<sub>ocm max</sub> = 1.4V
    - V<sub>ocm</sub>maxswing = (0.94 + 1.4)/2
     <table>
        <td>V<sub>ocm</sub>maxswing = 1.17V</td>
      </table>
 - simulation
      
      ![Image](https://github.com/user-attachments/assets/5019afc3-c582-403e-b1ae-2bf3fe4e3e52)
   - we can verify by the graph
   - the wave is starting from 1.325V and reached till 2.498V
   - therefore 2.948 - 1.325 = 1.173V which is equal to the calculated value V<sub>ocm</sub>maxswing.
  
**Range of an V<sub>icm</sub>**
 <table>
    <td>V<sub>GS1</sub> + Vp <= V<sub>icm</sub> <= min(V<sub>DD</sub> - (I<sub>D</sub>*R<sub>D</sub>) + V<sub>th</sub> , V<sub>DD</sub>(when one mosfet is off))</td>
  </table>
      
- **AC Analysis:**
  - we got A<sub>v</sub> = -4.99V/V
  - A<sub>vdB</sub> = 20log(A<sub>v</sub>)
  - A<sub>vdB</sub> = 20log(4.99)
  <table>
    <td>A<sub>vdB</sub> = 13.96 dB</td>
  </table>
  - we need to calculate 3dB gain
  - 3dB gain = A<sub>vdB</sub> - 3dB
  - 3dB gain = 13.96 - 3
  <table>
    <td>3dB gain = 10.96 ~ 11dB</td>
  </table>
- Simulation
  
 ![Image](https://github.com/user-attachments/assets/2cc56e65-1255-42f5-8fa3-2e9352151be6)
- From the graph the gain is 13.180 dB
- The 3 dB bandwidth will be 19.433 GHz 

  

