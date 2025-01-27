**Cell dilutions**
 
Overnight cultures are ~ OD = 2 => 1e9 cells/ml

|   |   |
|---|---|
|Guava/SEA|Dilute stationary phase cultures **100 X 100** times to get 1e5 cells/ml = 100 cells/ul (within the readable range without doublets/clogging. 1-5e5/ml) -- _dilution is more important for Guava vs Sony_<br><br>- 10 ul in 1,000 ul PBS in deepwell x twice is better<br>- 2 ul in 200 ul x 2 PBS is a good dilution routine in plate reader plates (used-washed is ok~) -- small volume|
|Sony/BRC|1:100 dilution is good enough, good range of events is 5,000 events/sec ; flow rate need to note down|
|Sony sorter/Keck|O/N stationary phase cultures: 1:10 dilution?  <br>Conjugation : 1:10 dilution gives ~ 5,000 eps (which expt?) ; < 5,000 eps = good rate for sorting says chip specs. Also estimate from 1:100 dilution ~ 300 eps after coarse filtering - [S054 WW conjug](S054%20(On)%20-%20Conjug%2051%20into%20WW%20(proof%20of%20concept))|
 
**Calibration beads**
 
[Spherotech](https://www.spherotech.com/CalibrationParticles.htm) rainbow calibration particles , 8 peaks (3-4 um) - RCP-30-5A  
~ 1e7 particles/ml. Use 2 drops per 1 ml  
Details [PDF](https://www.spherotech.com/2020%20Product%20Detail%20Pages/Spherotech%20Rainbow%20Calibration%20Particles.pdf) -
 
**Gain and threshold properties**

|   |   |
|---|---|
|Cytometer/BRC : S089<br><br>![Exported image](Exported%20image%2020250102022549-0.png)|Sorter/Keck : S085 b<br><br>![Exported image](Exported%20image%2020250102022554-1.png)|
   

**Following are some of the suggestions to avoid clumping.**
 
·        Use EDTA at up to 5mM concentration (for example: ready to use 0.02% in DPBS (0.5 mM), Cat# E8008, Sigma-Aldrich Co.; or ~0.5 M in H2O, Cat#03690, Sigma-Aldrich Co.). It may help to prevent cation-dependent cell-cell adhesion  
·        Add 25-50ug/ml of DNAse I (Cat# D4513, Sigma-Aldrich Co.) and 5mM MgCl2 (Magnesium chloride hexahydrate, Cat# M2670, Sigma-Aldrich Co.) to the buffer. It may help if cells are clumping due to the cell death
 
- Could add tween-20 at 0.1% (PBST) -- recommended by Xiao for biofilm prevention in microfluidic culturing
 
Buy PBS for the cleanest experiments (without particulates)
 
Add Syto-9 or other cell permeating nuclear stains to benchmark the FSC, SSC rules to gate the populations by

- Especially handy for tiny cells (Vibrio), and probably E coli too (this was when the PBS was not clean so there were way too many particulates I guess)
- Need to threshold by FSC to remove particulars
   

**Resources for analysis (Shyam)**  
FlowJo: [OpenFlow: Introduction to Flow Cytometric Data Analysis Part I - YouTube](https://www.youtube.com/watch?v=z592Kack9B0)  
Full-spectrum cytometry [OpenFlow: Full Spectrum Flow Cytometry with the Cytek Aurora - YouTube](https://www.youtube.com/watch?v=Lg2JV9eKGt4)