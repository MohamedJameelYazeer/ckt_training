# INTEL.CKT.TRAINING(2023)

## Day 1(WW01.4'23)- Fundamental of VLSI Design and Overview or Sand to Silicon

 <details>
<summary>Learning</summary>
<br>
 
 ### Intro : Steps to create GITHUB REPO :



### Analog VLSI CKT Design , Presenter : Prof Santunu Sarangi

1)Basic Unix

2)Analog Design - sch drawing tools

3)Digital - Verilog, EDA,synthesis,etc

4)Book reference : Fundamentals of electric circuit, Charles K.Alexander & Matthew N.O Sadiku


### Fundamental VLSI :Overview of Sand to Silicon

What is VLSI?
1) Motherboard --> Chip --> Waver --> Die
2) Die contain of : 
 - Microcontroller, memory,analog and digital circuit. --> Implemented of VLSI.
3) Good Design must fullfill following requirement :
 - Functionality (Performance, low power)
 - Low Cost
 - Timely execution
 4) Design quality checks :
 - Testability
 - Yield
   What is yield? 
   - percentage of the actual number of chip produced on one wafer.  (number of chip working)
   - % Yield = (good die/ total die) X 100 %
 - Realibility (EOS,ESD,noise,crosstalk,etc)
 
 <br>
</details>

<details>
<summary>Assignment</summary>
<br>

[assign1.pdf](https://github.com/MohamedJameelYazeer/ckt_training/files/10430412/assign1.pdf)
[assign1.pdf](https://github.com/MohamedJameelYazeer/ckt_training/files/10430413/assign1.pdf)

<br>
</details>

 ## Day 2(WW02.1'23)- Details of IC Manufacturing Process
 
 <details>
<summary>Learning</summary>
<br>
 
 ### Analog IC Design Process
 1) Electrical Design(Schematic design) :
    - It is a starting to the Analog design, which is designer start with defining the specification of the circuit/schematic.
    - Followed by circuit drawing and verifiying the design using Analog design schematic tools such as Virtuoso,Presto and etc.
    - Besides specifications requirement, robustness of the design can be ensure by reliability test(EOS, Aging,RV,etc).

2) Physical Design(Layout Design) :
   - Process of representing electrical design(schematic) in layout.
   - Start with physical design such as floorplan, placement and routing.
   - Followed by the physical verification - Check LVS, DRC rule.
   - Lastly is parasitic extraction, whereby extracting the layout so that design can be validate with RC parasitic.

3) Test Design :
   - Process of coordinating,planning and implementing the Analog Design performance.
   - Type of test : Functional,Parametric,static, dynamic.
   
4) Flow chart of Analog Design process as below :

![image](https://user-images.githubusercontent.com/122240906/211698970-2c723d32-8229-45f1-b3cd-f2ce3b22ef5e.png)

5) Analog IC Design Process and Relation with CAD and PDK

![image](https://user-images.githubusercontent.com/122240906/211699618-aaeab87b-a51e-4562-bbfc-2aed9ea77a48.png)

6) Keynote : Designer should always design a practical circuit based on the device limit, technology constraints and physical implementations in order to meet the criteria of high performance, low power and low cost. Therefore the understand of layout design is important to minimize the iteration in design process.

 ### CMOS Technology
 
 1) Comparison of BJT and Mosfet :
 ![image](https://user-images.githubusercontent.com/122240906/211700541-34105d9c-b730-4ff7-923b-9d05bfd1c8e0.png)
 

 ### CMOS Fabrication Process 
 
 1) Process steps :
    Wafer Formation(sand to silocon) --> Photolithography --> Well and Channel Formation --> Sio2 Deposition --> Isolation 
    --> Gate Oxide Creation --> Gate and Source/Drain Formations --> Contacts and Metalizations --> Passivation --> Metrology.
    
    
    (a) Wafer Formation
    - wafer cut from boule, cylindrical ingots of single crystal silicon.
    - some amount of impurities added to the melt to provide the crystal.
    - A seed crystal is deep into the melt to initiate crystal growth.
    - Seed gradually withdrawn from the melt and simultaneously rotated.
    - The seed withdrawal and rotation rates determines the diameter of ingot.
        <img width="172" alt="image" src="https://user-images.githubusercontent.com/122240906/212214940-d13af078-c3f8-4ea1-8dc3-7fc2f2c47825.png">
        <img width="415" alt="image" src="https://user-images.githubusercontent.com/122240906/212215077-b5d40c15-8944-4692-9339-b91157748812.png">
    
    (b) Photolithography
       - patterning process.
       - wafer coated by the photoresist and subjected to selectiv illumination through the photomask.
       - photomask is constucted with chromium.
       - used UV light to expose- the photorist.
       <img width="218" alt="image" src="https://user-images.githubusercontent.com/122240906/212219497-5ec17755-ee07-48a0-85dc-3ebb57cb4a30.png">

    (c) Well and Channel Formation
    - Nwell : pmos bule in a n-well, nmos place in p substrate.
    - Pwell : nmos bule in a p-well, pmos place in  n substrate.
    - Twin well : emergence of nwell process.
    - Triple well : provide isolation between analog and digital blocks in mixed signal chips. used to isolate high density dynamic memory for logic.

    (d) Silicon Dioxide(Sio2)
    - Oxidation achived by heating the silicon wavef in oxidizing atmostphere.

    (e) Isolation
    - to avoid interaction between devices.
    - form thick oxide by LOCOS process - Local Oxidation of Silicon
        
    (f) Gate Oxide
    - Form gate oxide for transistor. 
    - gate also consist thin gate layer oxide.

     (g) Gate and Source/Drain Formations.
     - Grow gate oxide to accommodate gate/drain/source --> deposit polysilicon --> patter polysilicon --> etch exposed gate oxide --> implant pMos/nMOS source&drain region.

     (h) Contact and Metallization
     - Make contact cut to source/drain/gate according to contact mask.-hole etched in dielectric after source/drain formation.
     - make from alluminium, copper or tungsten.

     (i) Passivation
     - Final process is adding a protectiove glass layer.
     - to prevent ingress of contaminants.
      
      (j) Metrology
      - Measurement process to give feedback to manufacturing process.
<br>
</details>

<details>
<summary>Assignment</summary>
<br>
 
 [assign2.pdf](https://github.com/MohamedJameelYazeer/ckt_training/files/10430418/assign2.pdf)


<br>
</details>

 ## Day 3(WW02.3'23)- CMOS Fabrication Process in DSM and UDSM Tech
 
<details>
<summary>Learning</summary>
 <br>
 
 ### Submicron CMOS Process
 
 Disadvantages :
 - pn junction usage, to isolate transistor becomes impractical as transistor size decrease.
 - LOCOS disadvantage; bird's beak effect, the surface area loss to this encroachment.
 - LOCOS advantage; simple flow, high oxide quality due to LOCOS structure thermally grown.
 <img width="230" alt="image" src="https://user-images.githubusercontent.com/122240906/212546268-fd095a42-b0ae-415b-8110-8f77ff25f676.png">
 

  ### Sallow Trench Isolation (STI) Process
  
  - Preffered isolation process for deep-submicron process --> No Bird's beak(reduced active to active spacing).
  - Much suitable for the increase density in small area.
  - Disadvantages : a lot of process steps.
  
  <img width="248" alt="image" src="https://user-images.githubusercontent.com/122240906/212547601-465f2e9a-49bd-49a6-9882-4aa22e381faa.png">

   
  ### Deep Submicron (DSM) and Ultra Deep Submicron(UDSM) CMOS Technology
  
 - Type of resistor in DSM CMOS Technology.
 <img width="476" alt="image" src="https://user-images.githubusercontent.com/122240906/212549423-199d416a-bb3c-4340-abee-d252582c85ae.png">

 - Type of capacitor in DSM CMOS Technology.
 <img width="542" alt="image" src="https://user-images.githubusercontent.com/122240906/212549447-1b9c71f8-cc40-4eb4-b3ac-4baca19d7ebe.png">

- DSM Fabrication Process

<img width="439" alt="image" src="https://user-images.githubusercontent.com/122240906/212549198-38427377-ee5b-47b9-86b8-7dcebab5f13e.png">
 
- DSM vs UDSM
<img width="666" alt="image" src="https://user-images.githubusercontent.com/122240906/212550430-ebb41b06-4d04-464f-b5be-ba36f13f702d.png">

<br>
</details>

<details>
<summary>Assignment</summary>
<br>
6. What are the advantages of ultra-deep submicron process over deep submicron process?
  <br> Advanates of UDSM is Improved Ion/Ioff ratio, Reduyced Cg, Higher Ion and Lower Ioff, active power reductions, reductions in interconnect density, the room for more metal are possible in USDM, higher swtiching speed, higher cut-off freq. <br>
7. What is the difference between LOCOS and STI process?
<br> LOCOS is traditional isolation tech in submicros which had advantages of simple fabrication process and high oxide quality and Bird's peak effect is one of the disadvantages of LOCOS. But STI allows closer spacing of transsistors by removing depletion region at surface and can elimate bird's effect. <br>
8. Why for body connection a heavily doped n+ or p+ is used?
<br>Body is highly doped to make it almost a matel to matel connection else it may acts as schotty barrier diode <br>
9. What is use of silicide and poolside?
<br> To reduce the resistance of the bulk diffusions and polysislion and to form resistive contacts with material on which it is deposited <br>
10. Which process steps used for control threshold voltage and punch-through effect? 
<Thru Implants <br>
11. Draw a top view, front view and 3D view of a CMOS inverter and annotate the length
and width of both PMOS and NMOS transistor.
<br>
![image](https://user-images.githubusercontent.com/121996056/212796633-c5844ae9-c3b1-4ea7-baef-e2548324cbc4.png)
3D will upload later.
<br>
12. Why sidewall spacer are used in DSM technology?
<br>To prevent the part of source and drain next to the channel from becoming heavily doped.<br>
13. What are the advantages of Deep N-well technology over n-well technology?
<br>Can use to reduce substrate noise couplings <br>
14. What is passivation layer?
<br> Glass protection layer to protect whole device. Vut where done at the specific places to connect metals going out<br>
15. What is Bird’s beak in LOCOS process and what is the impact on the transistor
performance?
When performing LOCOS steps for thermal oxidation growth, a bird's beak effect is commonplace and surface area will be reduced. 
 
<br>
</details>

 ## Day 4(WW02.5'23)- Metal Oxide Semiconductor(MOS) Structure
 
<details>
<summary>Learning</summary>
<br>
 
  ### Metal Oxide Semiconductor(MOS) Device Structure
  
 - MOS junction - A capacitor
                - No current-voltage relationship, on capacitor-voltage relationship.

<img width="157" alt="image" src="https://user-images.githubusercontent.com/122240906/212551398-9b7349ed-0a32-4dcb-99f5-e4b7d3e06128.png">

### Metal Oxide Semiconductor(MOS) Fabrication

- Process to create SiO2 on top of silicon, called Oxidation.
- Process to deposit poly-silicon on top of SiO2 called Metallization.

### Ideal MOS Junction or Capacitor

 - No charge in the device if V=0
 - Substrate is uniformly doped.
 - All charge is 0 (Interface charge, Trapped charge, Fixed charge, mobile charge, etc..)
 <img width="256" alt="image" src="https://user-images.githubusercontent.com/122240906/212551717-4dd1b5a6-e029-4c2c-aa53-95a7c4d78dc1.png">
 - 4 condition in ideal case: 

 (1) Accumulation Mode (v<0)
  - Accumulation occurs when voltage applied less than the flatband voltage.
  - The negative charge on the gate attracts holes from the substrate to the oxide-semiconductor interface.
  - Pile of majority carrier at the interface.
  - Charge at the surface directly proportional to voltage
<img width="224" alt="image" src="https://user-images.githubusercontent.com/122240906/212552359-49da06c0-d23e-4c0f-b561-d24501d73f9e.png">

(2)  Depletion Mode ( V > 0)
  -  More positive voltage than the flatband voltage is applied, a negative charge builds up in the semiconductor
  -  The depletion layer width further increases with increasing gate voltage.
 
 (3) Strong Inversion Mode (V > and equal Vt)
  - at Vt, channel form at the surface of semiconductor due to inversion charges.
  - Before Vt, charge come from negatively charged ionized acceptors.
  - After Vt, more charge comes from electron rather that depleting the holes.
  - More negetive charge required for semiconductor is comes from the mobile electron.
  - this negetive charge emerged to the oxide-semiconductor interface, this charge is due to minority carriers, so called inversion layer.
  
 (4) Flatband
  - Refers to fact that the energy band diagram of the semiconductor is flat, which implies that no charge exists in the semiconductor.
  
### C-V Characteristic of MOS Structure

<img width="349" alt="image" src="https://user-images.githubusercontent.com/122240906/212553498-ca33966c-27fa-4fa7-b9d0-f41e2a3b68eb.png">

 

<br>
</details>

<details>
<summary>Assignment</summary>
<br>
 Assignment: Metal-Oxide-Semiconductor Structure 
<br>1. What are the main differences between ideal and real MOS structure? 
	Flat band voltage is zero for ideal but for real mos, it is the ratio of fixed charge and oxide thickness. Threshold voltage is different between both different due to addition of Vfb in real mos.
<br>2. What are the different modes of operation in a MOS junction? 
	Accumulation, Depletion & Weak Inversion and Strong Inversion.
<br>3. What is the difference between weak inversion and strong inversion of a MOS junction? 
	Depletion/weak inversion mode voltage is between 0 and Vth and for strong inversion, it is higher than vth. And Inversion layer strongly formed in strong inv oxide and depletion region.
<br>4. What is metal-to-semiconductor work function?
	Theoretically, it is the quantity which is the difference of work functions in the metal and the semiconductors.
<br> 5. For a heavily n-doped poly-silicon metal and a p-substrate semiconductor, what will be the metal-to-semiconductor work function? Positive or negative? -ve
<br>6. For a heavily p-doped poly-silicon metal and a n-substrate semiconductor, what will be the metal-to-semiconductor work function? Positive or negative? +ve
<br>7. What is threshold voltage of a MOS junction? Express threshold voltage for a non-ideal MOS junction.
	Threshold voltage is the voltage at which I starts to flow b/w Source and Drain. Otherwise, transistor begin conductive path.
<br>8. If the oxide (SiO2) increases for a MOS structure, the threshold voltage will increase or decrease? 
	Cox and Vth are indirectly proportional. So higher Cox, lower Vth.
<br>9. Instead of a lightly doped p-substrate, if you use a heavily doped p-substrate in a MOS structure then what will be the change in threshold voltage? Will it increase or decrease? Increase  
<br>10. Describe, why MOS capacitance stay minimum at very high frequency and back to high value at low frequency. 
Reason is the formation of inversion layer. For higher frequency, switching happens frequently which makes the electron-hole pair at the depletion regions

<br>
</details>
  
