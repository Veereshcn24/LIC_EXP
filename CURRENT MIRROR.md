#  **Current mirror circuit** 

***Introduction***
<p>
A current mirror is a circuit designed to copy a current through one active device by controlling the current in another active device of a circuit, keeping the output current constant regardless of loading. Current mirrors are widely used in analog integrated circuits, such as operational amplifiers, to provide biasing and active loads. They are essential in ensuring that the current in one part of the circuit is accurately replicated in another part, which is crucial for maintaining the stability and performance of the circuit.Current mirrors are one of the most fundamental and widely used circuits in analog electronics. They are essential components in integrated circuits (ICs) and are used in a variety of applications, including biasing, active loads, and signal processing. The primary function of a current mirror is to replicate or "mirror" a reference current from one part of the circuit to another, ensuring that the output current remains constant regardless of variations in load or other external factors.
</p>

***Theory***
<p>
The basic idea behind a current mirror is to use a reference current to generate a mirrored current. The most common implementation uses two transistors, where the base-emitter voltage of the first transistor sets the base-emitter voltage of the second transistor, thereby controlling the current through the second transistor.
</p>
<p>
Basic Current Mirror

</p>

![Screenshot 2025-03-24 004916](https://github.com/user-attachments/assets/831bdc7b-2f7c-4451-be5b-8d3f606198e3)



<p>
The simplest form of a current mirror consists of two bipolar junction transistors (BJTs) or MOSFETs. In the case of BJTs, the base and collector of the first transistor are connected together, and the base-emitter junctions of both transistors are connected in parallel. This configuration ensures that the base-emitter voltage of both transistors is the same, which in turn ensures that the collector currents are the same (assuming the transistors are identical).
</p>
<p>
For MOSFETs, the gate and drain of the first transistor are connected together, and the gates of both transistors are connected. This ensures that the gate-source voltage of both transistors is the same, leading to the same drain current (assuming the transistors are identical).
</p>

<p>
By neglecting the channel length modulation of the two  transistors the drain currents can be given as :

I<sub>REF</sub> = K'<sub>n</sub>Cox (VGS - V TH)2

and Iout = mn Cox (VGS - V TH)2

If we take ratio of two equations, we get,

= i.e. Iout = IREF
</p>


<p>
###  Circuit Diagram








  
**ADVATAGES**
  <p>
1] Does not become sensitive to PVT parameters .

 ![Screenshot 2025-03-24 002513](https://github.com/user-attachments/assets/3310f5dd-6f76-45e0-ace9-0c2b4ff571cc)

 
  
2] Rejecting voltage biasing.


