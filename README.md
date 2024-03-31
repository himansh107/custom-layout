# VSD Custom-Layout
This a repository describing the summary of the custom layout course by VSD

## 16 mask CMOS process

**1. Selecting a substrate** </p>
Selection of P type substrate with resistivity of 5^50 ohms and maintain a doping level which is less than ‘well’ doping. (~ 10^15 cm-3) </p>

**2. Creating active region for transistors** </p>

- deposit a 40nm of SiO2 on subtrate
- 80nm of Si3N4
- 1um of photoresist </p>

    On the photoresist **mask1** is placed. When UV light hits the photoresist, only the unprotected part is affected. </p>

- **LOCOS - Local Oxidation Of Silicon** </p>
The **mask1** is removed and the affected part of the P-substrate is washed of with chemicals. After this, the substrate with the protection of Si3N4 is placed in a furnace. 
The heat in the furnace helps to grow the exposed parts of the SiO2. </p>

**Before LOCOS** </P>

![image](https://github.com/himansh107/custom-layout/assets/75253218/21663420-e40c-487c-88c8-53205b385339) </p>

**After LOCOS** </p>
![image](https://github.com/himansh107/custom-layout/assets/75253218/368ce2c7-7ec9-4f58-82a9-84812820602f) </p>

The growth bumps created in the locos process isolated the two transistor areas in the substrate. </p>

- Remove the Si2N4 layer (light blue layer) using hot phosphoric acid </p>

**3) N-Well and P-well formation (3rd mask used)** </p>

 - N-well is use in Nmos fabrication, Pmos used in Pmos fabrication. Both wells are not created simultaneously. 
- Photoresist is applied on the intended place for n well side and P side is exposed to ion-implantation 
- Ion implantation is done by showering P type Boron ions. This process creates the P-well
- Similarly, Nwell is created by placing the photoresist on the Pwell side and showering the N well side with N type 
- Diffuse the N-well & P-well to half width of the substrate by High temperature furnace. Pockets of N & P well will be formed. </p>
  **Image after 3rd step**
 ![image](https://github.com/himansh107/custom-layout/assets/75253218/d0d71f1a-c093-4d53-9bd3-b84eb949ac23) </p>

**4) Formation of Gate – most imp terminal of Mosfet (4th  mask used)** </p>
**(i)** Threshold voltage depends on –
  1. Cox
  2. Doping concentration </p>
    
**(ii)** Place Photoresist on N side(**mask4**). Shower P side with low energy Boron (~60eV) </p>
  1. Why low energy boron? </p>
  We want boron implant just on the surface of P side. 
  Photoresist on Pside (**mask5**). Shower P side with N type impurity (Arsenic) </p>
  
**(iii)** Original oxide etched using dilute HF solution and re grown again to give high quality oxide (~10nm thin) </p>
**(iv)** Deposit a polysilicon layer (~0.4um) over the entire substrate. Add an n type impurity over this layer to keep a low gate resistance. </p>
**(v)** use **mask6** for GATE layer deposition </p>

**Image after 4th step** </p>

![image](https://github.com/himansh107/custom-layout/assets/75253218/169ebec8-d25e-4c97-87fa-6e6e3e1d9adb) </p>

**5) Lightly doped drain (LDD) formation (mask7 & 8)** </p>

- Mask7 is applied on n well side and p well side is showered with n type ions to create a lightly doped N – implants which acts as drain 
- Mask8 is applied on p well side and n well side is showered with n type boron ion to create P implants </p>
**Image after 5th step** </p>

![image](https://github.com/himansh107/custom-layout/assets/75253218/f8647d92-47d3-47cb-8605-18c17a39a92d) </p>

**Green area is side walls used to protect some portion of LDD in the source drain formation step.**

**6) Source and drain formation** </p>
- A small amount of screen oxide layer is placed. Reason - to avoid channeling. Channeling is the direct piercing of ions through the oxide layer into the substrate without even hitting the silicon.
- **Mask9** is applied in N well and N+ implant is done on the P well side to create properly doped source and drain. 
- **Mask10** is applied on P well side and same way P+ implant (Boron) is done in the N well side. 
- Thus, source and drain are created on the N and P well sides
- Lastly High temperature annealing is done to extend the source and drain profiles  </p>

**Image after 5th step** </p>

![image](https://github.com/himansh107/custom-layout/assets/75253218/c9c8be47-a75c-4d89-8fc7-1497578ffe25) </p>

**7) Steps to form contacts and interconnects (local interconnects)** </p>
- Etch thin oxide used earlier in HF solution.
- Deposit titanium layer over the substrate using sputtering </p>
  ![image](https://github.com/himansh107/custom-layout/assets/75253218/24fe6bc4-96f7-4267-924c-f8f87d4dfac2) </p>

**Fig. -  sputtering** </p>

- Wafer heated at about 650 -700 C in N2 ambient for 60 sec.
- **Mask11** is placed on the structures which need to be kept. TiN layer formed after heating is removed through RCA cleaning (RCA is chemical solution). </p>
**Image after 7th step** </p>
![image](https://github.com/himansh107/custom-layout/assets/75253218/e0de17fe-ace9-4a9a-b6d9-67f92ab90baf)

**8) High level metal formation** </p>

- 1um of SiO2 doped with phosphorus or boron is deposited on the wafer surface. Doping of boron is done to keep the surface temperature tolerant
-	SiO2 Surface is polished
-	**Mask12** is used to protect the parts on which SiO2 layer has to be kept. Through the remaining part contact holes are drilled.
-	~10um TiN layer is deposited to isolated the wafer from upper layers.
-	Tunsgten layer is deposited as a blanket layer to bring the bottom contacts to the top.
-	Chemical mechanical polishing is done to planarize the entire deposited surface.
-	Aluminum layer deposition is done
-	**Mask13** is placed to remove etch the redundant aluminum. </p>

***0 level layer – local interconnect*** </p>
***1st layer – Aluminum interconnect*** </p>

-	Again, Sio2 layering is done. That layer is polished and a higher metal layer is deposited to extend the aluminum to _**2nd metal layer**_ (**mask14** & **15** used).
-	As we go from bottom metal layer to top metal layer the thickness of metal increases. </p>
- **Si3N2 layer is placed to protect the chip.** 
- **Mask16** is placed to drill contact holes through this protection layer. </p>

**Final fabricated CMOS** </p>
![image](https://github.com/himansh107/custom-layout/assets/75253218/72bd364d-46bb-4dbb-85d3-e9622a0d0ae5) </p>


## Corner Stitch data 

Every tile is represented by two corner stitches </p>

_**(top – right , right – top) , (bottom – left, left - bottom)**_ </p>

**Lab Activity :** </p>
 Command for seeing well corner stitch data</p>
 ```bash
  *watch well demo
```
**output** </p> 
![image](https://github.com/himansh107/custom-layout/assets/75253218/1e34d1cb-be36-47b4-984e-4c07672b502f) </p>

black circle - space tile, red circle -  well mask </p>

**Command for seeing metal1 corner stitch data** </p>

 ```bash
  *watch metal1 demo
```
**output** </p>
![image](https://github.com/himansh107/custom-layout/assets/75253218/7018cc29-6833-4d5e-a507-826ce1475e27) </p>

**Active plane is everything after removing metal1 and wells** </p>

 ```bash
  *watch active demo
```
</p>
**output** </p>
<img src="https://github.com/himansh107/custom-layout/assets/75253218/6db8dbb4-6445-4f25-bd4f-eb01edd242fa" width="400"> </p>



<img src="https://github.com/himansh107/custom-layout/assets/75253218/aa3eddb3-09b8-4854-8acc-d48317c87ed8" width="600">


## Module 2 - Connect section for circuit extraction 
</p>

The connect section of the tech file describes how different tile types are connected to each other and the electrical connections between them </p>

### Illustration 
</p>

The code below is the connect section of the .tech file. It shows one instance connections </p>
![connect section ](https://github.com/himansh107/custom-layout/assets/75253218/093cb406-036b-41d1-baf1-d92e85bd4a4e) </p>

- nwell - nwell tile 
- nsc/a - n substrate contact of the active plane 
- nsd - n substrate diffusion </p>

Writing all three seperated by comma means that they are mutually connected. Repeating the same with space in between denotes that there is a electrical flow of current between them. </p>
<img src="https://github.com/himansh107/custom-layout/assets/75253218/d162573b-c14f-46c8-b4bc-87248c894f5f" width="600">

Similarly, in the picture above the polysilicon (poly) is connected to all fets and polysilicon contact of the active plane and there is electrical current flow between these connections </p>


## Module 3 - Design Rule Check  
</p>

Lambda (λ) based design rule </p>
λ = L/2 , L = minimum feature size  </p> 

**Table of Design rules** </p>
![table of rules](https://github.com/himansh107/custom-layout/assets/75253218/30242ef8-e9df-40bc-bb95-8dfcf3fb7cd0) </p>

**Lab Activity:** </p>

**1. Minimum poly widht = 2λ** </p>

![image](https://github.com/himansh107/custom-layout/assets/75253218/e0f2d113-6c16-456e-a094-cbc0f9b8bb27) </p>

**Corrected DRC error** </p>
![image](https://github.com/himansh107/custom-layout/assets/75253218/dedb7bf4-074f-4869-97a8-483ec4d0184e) </p>

**2. Poly extension over active** </p>

Minimum = 3 λ </p>

**drc illustration** <p>

![image](https://github.com/himansh107/custom-layout/assets/75253218/662ac86a-650d-4810-a99c-b9806ea25bec) </p>


**2. Poly to diffusion spacing** </p>

minimum = 1λ </p>

**drc illustration** </p>
![image](https://github.com/himansh107/custom-layout/assets/75253218/b1f786af-661d-4176-ac3b-723efced580e) </p>

**3. Poly to n diffusion contact spacing** </p>

minimum = 1λ </p>
**drc illustration** </p>
![image](https://github.com/himansh107/custom-layout/assets/75253218/2e01d80c-f453-4497-8bb7-5cf727fd61a5) </p>

**4. ndiff/pdiff contact** 

minimum width = 4λ, height = 4λ </p>
**drc illustration** </p>
![image](https://github.com/himansh107/custom-layout/assets/75253218/e6756ca7-028e-48ee-b720-46774233ffd4) </p>

**5. Metal1 width – 3λ minimum** </p>
**6. Poly to metal spacing – n/a** </p>

**7. Poly to poly spacing** </p>

 minimum  = 3λ </p>
**drc illustration** </p>
![image](https://github.com/himansh107/custom-layout/assets/75253218/d5a575f2-e6ac-4e01-96a5-e85ab9201b78) </p>


**8. Ndc to ndc spacing** </p>

**drc illustration** </p>

![image](https://github.com/himansh107/custom-layout/assets/75253218/57021401-0a85-4605-b0aa-ed143c5903e4) </p>

ndc , ndc touching is ok </p>

**drc illustration** </p>

![image](https://github.com/himansh107/custom-layout/assets/75253218/b3286ac9-d132-410c-831c-92be9085536d)

**9. Ndiffussion contact to  p-substrate contact spacing** </p>

minimum = 2 λ </p>

![image](https://github.com/himansh107/custom-layout/assets/75253218/e436009d-074a-4a73-9f34-6acaa88743ef) </p>




