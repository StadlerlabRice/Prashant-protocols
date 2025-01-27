**Goal**: I want to sequence a full plasmid (4 kb) in low throughput; what's the best way - quickest. Put resources and workflow here

- Sample requirements : Concentration, volume
- Consumables needed
- How many times can the flow cell be used     
**Ligation sequencing kit (1 h)**  
SQK-LSK110 (for multiplex : use SQK-LSK109) : 600$ / 6 rxn !!! SOO expensive; ==just for the adapters==

> From <[https://store.nanoporetech.com/us/catalog/product/view/id/488/s/ligation-sequencing-kit110/category/28/](https://store.nanoporetech.com/us/catalog/product/view/id/488/s/ligation-sequencing-kit110/category/28/)>  

- Input : 1 ug ds DNA
- dA tailing (NEBnext end repair) + ligation with adapters
 
|   |   |
|---|---|
|![Machine generated alternative text:High molecular weight gDNA Optional fragmentation or size selection End-prep and nick repair 60 min Ligation of sequencing adapters Loading ](Exported%20image%2020250102022408-0.png)|**For plasmid sequencing**<br><br>  <br>  <br>  <br><br>_Skip these_<br><br>  <br>  <br>  <br><br>Blunting (if restriction digest)  <br>A tailing<br><br>  <br>  <br><br>T4 DNA Ligase|

Full protocol on Zotero
 
**NEB components**

- NEBNext® [Ultra™ II End Repair/dA-Tailing Module](https://www.neb.com/products/e7546-nebnext-ultra-ii-end-repair-da-tailing-module#Product%20Information) : $250/24 rxn : requires .5-1 ug DNA (individual modules require more..)
    
    - [End repair module](https://www.neb.com/products/e6050-nebnext-end-repair-module#Product%20Information) : $90/20 rxn : requires 1-5 ug DNA : to blunt-end DNA having 5′ phosphates, and 3′-hydroxyls :: _Can skip if using Q5 PCR products that are gel/column purified…_
    - [NEBNext® dA-Tailing Module](https://www.neb.com/products/e6053-nebnext-da-tailing-module#Product%20Information) : [protocol](https://www.neb.com/protocols/0001/01/01/nebnext-da-tailing-module-protocol-e6053) - $100/20 rxn : requires 1-5 ug DNA : Klenow fragment (3'-5' exo-)
- NEB [Blunt/TA ligase master mix](https://www.neb.com/products/m0367-blunt-ta-ligase-master-mix#Product%20Information) : 100$/50 rxn
    
    - Or NEBNext [quick DNA ligase module](https://www.neb.com/products/e6056-nebnext-quick-ligation-module#Protocols,%20Manuals%20&%20Usage) : **318$/20 rxn** : same input requirement ; uses **quick** T4 DNA ligase (what is this quick thing?). [Protocol](https://www.neb.com/protocols/0001/01/01/nebnext-quick-ligation-module-protocol-e6056) ; 15 min, 20oC ;; TOO EXPENSIVE :(
    - Just get regular T4 DNA ligase, probably need to use at a higher concentration?

alternate/combined

- [NEBNext](https://www.neb.com/products/e7180-nebnext-companion-module-for-oxford-nanopore-technologies-ligation-sequencing#Product%20Information) Companion module - 920$/24 rxn : too expensive and unnecessary
 
**Cheapest, ad-hoc options, non-standardized**

1. Ideal scenario would be to use a blunt digesting enzyme, else digest with any enzyme and
    
    1. Only difference is that the dNTPs are separate here compared to premixed in the end repair module
2. ([A-tailing](https://www.neb.com/applications/cloning-and-synthetic-biology/dna-end-modification/a-tailing)) : Adding A to 3' end. Can use either [Klenow (exo-)](https://www.neb.com/protocols/2013/11/06/a-tailing-with-klenow-fragment-3-5-exo) w NEBbuffer2 or [Taq pol](https://www.neb.com/protocols/2013/11/01/a-tailing-with-taq-polymerase) w thermopol buffer. Need to buy separate dATP ([openwetware](https://openwetware.org/wiki/Addition_of_3%27_A_overhangs_to_PCR_products)) 
Esther's question - do these add a single A or multiple?

5. [Terminal transferase](https://www.neb.com/protocols/0001/01/01/a-typical-dna-tailing-reaction) can add any number of nucleotides (any N) depending on the concentration
6. What about Taq? Which seems to add only A? 
SrfI and SwaI - blunting 8 cutters : Use these to avoid end prep with a blunting enzyme!? - Shyam
      

--------------------------------------  
Joining nanopore account  
Esther's account

14. Name: Rice University
15. Number: #C028422 
-------  
More sample prep reagents  
[https://nanoporetech.com/products/prepare/dna-library-preparation](https://nanoporetech.com/products/prepare/dna-library-preparation)
 
--just use end end repair module;([quick blunting](https://www.neb.com/products/e1201-quick-blunting-kit#Product%20Information): 86$/20rxn) DNA is blunted using T4 DNA polymerase (NEB #M0203) which has both 3´→ 5´ exonuclease activity and 5´→ 3´ polymerase activity. T4 Polynucleotide Kinase (NEB #M0201) is included in the enzyme mix for **phosphorylation of the 5´ends** of blunt-ended DNA for subsequent ligation into a cloning vector. This kit is optimized for blunting up to 5 µg of DNA in a single reaction. _Already have individual enzymes, figure out ratio and buffer?_
            

**Rapid barcoding using taransposase (10 min protocol)**  
[https://store.nanoporetech.com/us/rapid-barcoding-kit.html](https://store.nanoporetech.com/us/rapid-barcoding-kit.html) ; [Detailed protocol](https://community.nanoporetech.com/docs/prepare/library_prep_protocols/rapid-barcoding-sequencing-sqk-rbk004/v/rbk_9054_v2_revaa_14aug2019/equipment-and-consumables?devices=minion)

- Comes with 12 barcodes
- Input requirement : 400 ng of high molecular weight gDNA (>30 kb)
    
    - Would need higher mass for shorter DNA or could scale down reagent volumes..?
 ![Barcoded transposome 5 min Cleavage and addition of barcoded transposase adapters Pooling ot barcoded libraries and attachment ot sequencing adapters 5 min Loading gDNA ](Exported%20image%2020250102022409-1.png)  

- Esther said we have this kit and is not using it anymore - Dec, 2021
 
---------------------------------------------------------------------  
**Notes: Rapid barcoding kit**

- Esther says : only works for gDNA larger than 30 kb
- Shyam says this might be easily optimized for shorter things by reducing the reaction time  
a follow-up on this (quoting email sent from nanopore team):
 
Hello Ester, 
 
Thank you for the follow-up questions. Using **long fragments** as the input for the RBK (rapid barcoding) kit is our recommendation, so that the read length won’t be too short. But customers can choose to use any length as they see feasible or suitable for their data analysis goals. The website ==www.protocols.io== is independent from Oxford Nanopore. The protocols there are not official ones but may have worked well for the authors. I would recommend that you contact them if you’d like to try something similar.Best regards,Yan
 > From <[https://app.slack.com/client/TS7BYTGSW/search/search-4160f216-964b-422f-b396-d851924d7950/thread/DT34FN0UD-1616780072.021900](https://app.slack.com/client/TS7BYTGSW/search/search-4160f216-964b-422f-b396-d851924d7950/thread/DT34FN0UD-1616780072.021900)>   
-----------------
   

**From:** ==ONT Customer Services <====support@nanoporetech.com====>==  
**Sent:** ==Monday, April 5, 2021 9:34:40 PM==  
   
Hello Esther, 
 
For clarity, I'd like to make a distinction between the RBK004 and **RBK110.96** chemistry. The latter has a new type of Rapid Adapter (RAP-F). As compared with RAP in RBK004, RAP-F consumes much less fuel during sequencing, which helps maintain the throughput of short fragments and read quality. 
 
==You can see the release note for RBK110.96 here,== ==https://community.nanoporetech.com/posts/rapid-barcoding-kit-96-rel== ==, and it's official protocol for 1.2 kb COIVD amplicon sequencing here,== ==https://community.nanoporetech.com/protocols/pcr-tiling-of-sars-cov-2-virus-with-rapid-barcoding-sqk-rbk110/v/pctr_9125_v110_reva_24mar2021?devices=minion== ==.== 
 
I hope this helps with your decision on the kits. 
 
Best regards,
 
Yan
 
---  
**From:** ==ONT Customer Services <====support@nanoporetech.com====>==  
**Sent:** ==Tuesday, March 30, 2021 2:59 PM==  
**To:** ==esther.lou@outlook.com== ==<====esther.lou@outlook.com====>==  
**Subject:** ==RE: FW: tech support on a ONT kit [ ref:_00D20N1PA._5004L6Lhrg:ref ]==  
   
Hello Ester, 
 
==Thank you for the follow-up questions. Using long fragments as the input for the RBK kit is our recommendation, so that the read length won't be too short. But customers can choose to use any length as they see feasible or suitable for their data analysis goals. The== ==website== ==www.protocols.io== ==is independent from Oxford Nanopore. The protocols there are not official ones but may have worked well for the authors. I would recommend that you contact them if you'd like to try something similar.==
 
Best regards,
 
Yan  
--------------  
Hi Yan,
 
Umm I am confused about the kit. The reason I ask is because people are using this RAPID protocol (a way to multiplex COVID19 genome:==https://www.protocols.io/view/ncov-2019-sequencing-protocol-rapid-barcoding-1200-bh7hj9j6==) and they used the ONT SQK-RBK004 (you can check the "material" tab), but the amplicon size is only 1200 bp.
 
Esther

- Quoted test : To enable faster, easier sequencing of SARS-COV2 genomes with fewer steps than current methods, we use multiplexed 1200 base pair PCR amplicons with the Oxford Nanopore RAPID barcoding...

---  
------------ Original Message ---------------  
From: ONT Customer Services [==support@nanoporetech.com==]  
Sent: 15/03/2021 19:58  
To: ==esther.lou@outlook.com==  
Subject: RE: FW: tech support on a ONT kit [ ref:_00D20N1PA._5004L5wIcG:ref ]
 
Hello Esther,
 
It's nice to hear from you. The **rapid barcoding kit**, RBK004, ==requires long fragments as the input, > 30 kb ideally==, which is typical for gDNA rather than for amplicons. That's why there is no such a RBK004 protocol.
 
The reason behind this requirement is that the Rapid chemistry uses transposase to randomly cut the input fragments and then add the sequencing adapters to the cut-ends. When short input is used, the resulting fragments and then the read length can be much shorter than the input length.
 
How long is your amplicon? Also, what's the goal of your analysis. Some customers have used ~ 10 kb input and the resulting read length seemed suitable for their applications.
 
Best regards,
 
Yan  
---