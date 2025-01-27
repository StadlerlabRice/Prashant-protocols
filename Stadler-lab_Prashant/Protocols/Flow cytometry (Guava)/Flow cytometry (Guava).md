> [!caution] This page contained a drawing which was not converted.   

Guava Flow cytometry @ Bennett lab training guidelines : David Zong

![Exported image](Exported%20image%2020250102022524-0.jpeg)  

Cell counts should be between 100-500 cells per ul. Can OD the cultures and dilute appropriately
 
--------------------------------------------------------------  
Guava SEA training  
24/11/20  
**Steps**

1. Empty the external waste vial, fill up the ICF fluid in the other vial;
    
    1. check for precipitates/clumps in the existing fluid and discard completely + rinse in water
2. Run Guava-clean cycle (once) - takes 15 mins
    
    1. Put a vial of DI water for capillary shutdown    
![Exported image](Exported%20image%2020250102022525-1.jpeg)  
![Exported image](Exported%20image%2020250102022532-2.jpeg)  

**Consumables for Guava**

1. This is the [flow cell](https://www.emdmillipore.com/US/en/product/Guava-Flow-Cell-HT-Systems,MM_NF-0500-2260) used. Seems discontinued now
2. A more recent flow cell for [HT systems](https://www.luminexcorp.com/guava-easycyte-flow-cytometers/#order) (CN-0448-01) on [Fishersci](https://www.fishersci.com/shop/products/flow-cell-for-guava/NC1704092) : 635$
3. Instrument cleaning fluid - [ICF](https://www.luminexcorp.com/guava-instrument-cleaning-fluid-icf/#order) : 4200-0140 ([Fisher](https://www.fishersci.com/shop/products/NC1691769/NC1691769#?keyword=luminex%20Guava%20icf)) : 60$
4. EasyCheck beads ([Fisher](https://www.fishersci.com/shop/products/guava-easycheck-kit/NC1695457#?keyword=luminex%20Guava%20icf)) : 400$  
**Spectral information**  
Guava easyCyte HT BG system is a flow cytometer for performing flow cytometry experiments.  
It is equipped with 2 lasers: Blue 488 nm (150 mW) and Green 532 nm (100mW) with 8 fluorescent detection channels, forward and side scatter.

> From <[SEA](https://research.rice.edu/sea/instruments/biosea/flow-guava-easycyte-ht-bg-flow-cytometer)>   
|
|
==> Emission colour  
====> Emission/band  
====Excitation==
==Green-B== ==512/18==Blue 488 laser|
==Yellow-B== ==575/25==|
==Red-B== ==695/50==|
==NIR-B== ==785/70==|
==Yellow-G== ==575/25==Green 532 laser|
==Orange-G== ==620/52==|
==Red-G== ==695/50==|
==NIR-G== ==785/70==|
   

Calibration beads

- Sony and Spherotech have the same values (in file : calibration_beads_sony.csv)
- Spherotech has only these 5 channels, and Sony has 9 listed in their data sheets

|   |   |   |   |   |
|---|---|---|---|---|
|FITC|PE|PE-TR|PE-Cy5|APC|
|mGL|||||
 
**Syto-17** cannot be excited with these lasers :(  
SYTO 17 is a fluorescent compound with an excitation peak at 619 nm and an emission peak at 638 nm

> From <[https://www.aatbio.com/fluorescence-excitation-emission-spectrum-graph-viewer/SYTO_17](https://www.aatbio.com/fluorescence-excitation-emission-spectrum-graph-viewer/SYTO_17)>   
(archived) Order [Syto9](https://www.thermofisher.com/order/catalog/product/S34854?gclid=Cj0KCQjwlMaGBhD3ARIsAPvWd6jkgGjPPAtHB4Z2Okwiq7ZV1ZA40-_vHCx8RDrA-q89M1IxFGBUMIgaAmbDEALw_wcB&ef_id=Cj0KCQjwlMaGBhD3ARIsAPvWd6jkgGjPPAtHB4Z2Okwiq7ZV1ZA40-_vHCx8RDrA-q89M1IxFGBUMIgaAmbDEALw_wcB:G:s&s_kwcid=AL!3652!3!447292198736!b!!g!!&cid=bid_pca_iva_r01_co_cp1359_pjt0000_bid00000_0se_gaw_dy_pur_con#/S34854?gclid=Cj0KCQjwlMaGBhD3ARIsAPvWd6jkgGjPPAtHB4Z2Okwiq7ZV1ZA40-_vHCx8RDrA-q89M1IxFGBUMIgaAmbDEALw_wcB&ef_id=Cj0KCQjwlMaGBhD3ARIsAPvWd6jkgGjPPAtHB4Z2Okwiq7ZV1ZA40-_vHCx8RDrA-q89M1IxFGBUMIgaAmbDEALw_wcB:G:s&s_kwcid=AL!3652!3!447292198736!b!!g!!&cid=bid_pca_iva_r01_co_cp1359_pjt0000_bid00000_0se_gaw_dy_pur_con), or [Syto 13](https://www.thermofisher.com/order/catalog/product/S7575?SID=srch-srp-S7575#/S7575?SID=srch-srp-S7575) (cheaper, [works w E coli](https://journals-asm-org.ezproxy.rice.edu/doi/10.1128/AEM.64.7.2681-2685.1998?url_ver=Z39.88-2003&rfr_id=ori:rid:crossref.org&rfr_dat=cr_pub%20%200pubmed))
   

Comparison to Sony/BRC  
Guava can do 500 cells/ul x 0.59 ul/sec = 300 events/sec = 18,000 cells/min  
Sony can do 5,000 events/sec :: So if you need lots of events (> 20,000), better use the Sony
 
*Fill the capillary resting tube  
with water

1. Make sure cleaning fluid (ICF) is > 1/4th
    
    1. Empty the waste container

EasyCheck

**Explanation of terms**

|   |   |
|---|---|
|(FSC) Forward scatter|<relative size, larger size => higher FSC> : FSC intensity is proportional to the diameter of the cell, and is primarily due to light diffraction around the cell.<br><br>> From <[flowjo](http://flowjo.com/learn/flowjo-university/flowjo/before-flowjo/58)>|
|(SSC) Side scatter|Side scatter measurement provides information about the internal complexity (i.e. granularity) of a cell. The interface between the laser and intracellular structures causes the light to refract or reflect. Cellular components that increase side scatter include granules and the nucleus (1). <br><br>> From <[https://www.flowjo.com/learn/flowjo-university/flowjo/before-flowjo/58](https://www.flowjo.com/learn/flowjo-university/flowjo/before-flowjo/58)>|
|Backscatter|In some machines, backscatter is used in the place of SSC|

A good ppt to introduce flow cytometry concepts : [biochem.uni-frankfurt.de/](https://www.biochem.uni-frankfurt.de/fileadmin/user_upload/courses_practicals/BCII_GSH_Vortrag07.pdf);  
Tabor lab flowcal intro - [https://benchling.com/pub/tabor-flowcal](https://benchling.com/pub/tabor-flowcal)