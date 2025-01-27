> [!caution] This page contained a drawing which was not converted.   

List of BTK parts needed to

|
|
==Part type== ==Plasmid number== ==Name== ==Description, comments==
==
Constitutive promoter  
(2)
==pSPB605|GlpT promoter  <br>BBa_[J72163](http://parts.igem.org/Part:BBa_J72163)|Source: [http://parts.igem.org/Part:BBa_K2560002](http://parts.igem.org/Part:BBa_K2560002)|
=="==pSPB673 pCon100 (2)|Bba_J23100 (high strength)|(J23119 is the [strongest](http://parts.igem.org/Promoters/Catalog/Anderson) in the collection but not in Shyam's parts; although I'm making it att flanked)<br><br>- I assume these to work in Vmax because it is present in [Marburg collection](http://2018.igem.org/Team:Marburg/Part_Collection)|
==  
==pSPB676 pCon51 (2)|Bba_J23108 (medium strength)||
==  
==pSPB679 pCon01 (2)|Bba_J23103 (low strength)||
==  
==|||
==Broad host promoters (2) or (23)==Starts with HW in IGEM 2018 folder|pIG009 (36709 HW 8) :: moderate expression in hosts tested in UBER|Starts with HW in IGEM 2018 folder; has 12 different variants|
==  
==|pIG007 (34701 HW 5) :: high expression in some hosts tested in UBER||
==  
==|pSPB930 / pIG004 (29572) :: only HW expression data (below)||
==  
==pSPB814, 816|HW 29572|High expression in e coli observed in colonies (PK)|
==  
==|||
|||||
==RBS (3)==pSPB459|[BBa_B0034](http://parts.igem.org/Part:BBa_B0034)|Elowitz RBS, with context of BBa_J61002.|
==BCDs (3)==\|<br>\|<br>==pSPB455==<br>==pSPB456==<br>==pSPB457==<br>==pSPB458==<br>==  <br>==|\|   \|<br>\|---\|<br>\|_BCD2 Str01_\|<br>\|_BCD1 Str02_\|<br>\|_BCD10 Str07_\|<br>\|_BCD15 Str10_\|<br>\||\|   \|<br>\|---\|<br>\|Bicistronic design 2, strength 1\|<br>\|Bicistronic design 1, strength 2\|<br>\|Bicistronic design 10, strength 7\|<br>\|Bicistronic design 15, strength 10\|<br>\||
==  
==|||
==RBS broad host==||Do we need different shine dalgarno sequences for each organism? (genus?)<br><br>- It's mostly conserved, so let's try E. coli ones first<br>- List the anti-shine dalgarno sequences of organisms of interest for quick reference (pseudomonads, etc.)|
|||||
==CDS (4)==pSPB451 (4)|sfGFP||
==  
==|mScarlet-I 2V||
==  
==pSS02|MHT-mCherry2||
==  
==|mgreenlantern||
==  
==pSPB956|CymR.AM|Marionette one|
|||||
==Terminators (5)==|||
==  
==pSPB469 (5)|tvoigtN1|Use synthetic terminators for shorter, more reliable (recombination) behaviour|
||pSPB472 (5)|tvoigtN7||
==Connectors (1) and (6)==pSPB501 (1)  <br>pSPB520 (6)|conLS  <br>conRE|\|   \|   \|<br>\|---\|---\|<br>\|pSPB503\|==ConL2==pSPB512\|==ConR2====  <br>==<br>\|pSPB504\|==ConL3==pSPB513\|==ConR3== ==Not ideal but functional, digest with Esp3I (NotI is broken)==<br>\|pSPB505\|==ConL4==pSPB514\|==ConR4====  <br>==|
==Connectors for multi-gene assembly==pSPB539  <br>pSPB546|conL'S  <br>conL'E|L'2 and R'2 are decent too|
|||||
==Resistance (7)==pSPB412 (7)|ChlR||
||Others|Search on cloning log SPB..||
==Extra elements (8)==pSPB616 TonBt (8)|Bidirectional terminator :: spacer|Insulates ori from resistance marker|
==  
==pPKSS?|LasR cassette|Might want it between the connectors with IR if integrating :: Himar1 transposase element will be in (8).|
||||_Proposed assembly:_  <br>_conLS - int8 - conR2 … conL2 - LasR - conR3 … conL3 - Plas-ORF - conRE … (7) ChlR … (8) Ptet-Himar1 … (9) oriT … RSF1010 (oriR)_<br><br>  <br><br>_Donor will have_ _tetR_ _(or other repressor) on genome_|
==Origins (9)==pSPB418 (9)|P15A|p15A derivative pACYC works in Vmax (narrow host range)|
==  
==|pMB1||
==  
==pSPB416 (9)|pUC ori|pMB1 derivative; high copy|
==Broad host origins==pSPB449 (9)|RSF1010<br><br>  <br><br>Is this the same as RSF1030? No, 1030 is narrow host. 1010 is broad host.|Shyam claims really broad host range (incl. yeast!)<br><br>- pSPB448 includes Mob|
==  
==pSPB478 (9)|pBBR1|==
Shyam recently made it work (29/12/20 )
- pSPB479 is mob+
==
==  
==pSPB480|RK2|Medium host range - mostly gram -ve|
==  
==|pWV01|==Pretty high copy number==
==Part vectors (broad host)==||==
pSS026 : ~sfgfp-ChlR-RSF1010mob- (7-9.1)  
pSS037 : ~sfgfp-AmpR-pBBR1.mob (7-9.1)  
pSS039 : ~sfgfp-AmpR-RSF1010mob+ (7-9.1)  
pSS061 : ~sfgfp-ChlR-RSF1010mob+  
… till pSS067 --->
==
|Test plasmids|pSPB816  <br>pSPB817|mob+ mKate2  <br>mob- mKate2||
|Sequencing primers|AB17 == DZ239  <br>AB18 == DZ238|: in <- [ConL]  <br>: in <- [ConR]||
|Connectors in Shyam's box|28/4/21||![Exported image](Exported%20image%2020250102022245-0.png)|
|Plasmid aliquots|||30/4/21<br><br>![Exported image](Exported%20image%2020250102022247-1.png)|
    
Other literature
 
|   |   |
|---|---|
==RBS==Bba_[J95015](http://parts.igem.org/wiki/index.php?title=Part:BBa_J95015) :: catcaacggagg<br><br>  <br><br>Some options from iGEM ::  <br>[BBa_K2918014](http://parts.igem.org/Part:BBa_K2918014)  <br>[BBa_K1419003](http://parts.igem.org/wiki/index.php?title=Part:BBa_K1419003)|_Note: The SD sequence is complementary to the 3' end of the 16S rRNA. Its consensus sequence is 5'-UAAGGAGG-3' which is followed by an initiation codon, most commonly AUG. (About 8% of start sites use GUG, whereas UUG and AUU are rare initiators present in autogenously regulated genes). The optimal spacing between the SD sequence and the start codon is 8 nt, but translation initiation is severely affected only if this distance is reduced below 4 nt or increased above 14 nt. [Shine, J. and Dalgarno, L. (1975) Eur. J. Biochem. 57, 221.]_  <br>_An additional mRNA feature affecting translation initiation is the downstream box (DB), located after the initiation codon and complementary to bases 1469-1483 of the 16S rRNA. DBs consensus sequence is: 5'-AUGAAUCACAAAGUG-3'._|
 
Strong core promoters from E. coli are more likely to work in broad hosts

- Shyam 20/1/20
 
Questions for Shyam

1. Are the 8bp NotI sites present in every connector?
    
    1. If so, do they not facilitate recombinogenic loss of fragments between the repeats? In evolutionary timescales
2. Are the pCons numbered by strength, pCon1 is the strongest?
    
    1. 100 is the strongest
3. What is the name of the standard casette vector
    
    1. 438, 439
4. Do you have (23) Harris wang elements?
    
    1. Yes, they are in IGEM 2018 box which isn't in Bennett lab currently  
Check for palindromic repeats within IR sites - for pGT-Ah1
 
Other possible parts

|   |   |
|---|---|
|pCym|Strong basal promoter (in E. coli)|
 
Tips

- Allow few h at 4oC for maturation for ?? (slowly maturing) Fluorescent protein?

Wang promoters testing data

![E. coli MG1655 E. coli DHIOB E. coli Nissle E. coli BL21 Shewanella oneidensis Pseudomonas putida ID 5 6 7 8 x 103 16 14 12 10 8 6 4 2 10 O (D o (D o o o o o ](Exported%20image%2020250102022249-2.png)  

What do these ID numbers correspond to? ~ strength : Individual parts here - [http://parts.igem.org/Part:BBa_K2540010](http://parts.igem.org/Part:BBa_K2540010)
 ![Strength S Strength 8 Strength 6 Strength 10 Strength 7 Figure 5: mKate2 expression with broad host range regulatory elements across strains. mKate2 expression constructs with regulatory elements were transformed into four E. coli strains (MG1655, BL21 , Nissle 1917, DHIOB). p. putida , and S, oneidensls Cells were grown in LB and fluorescence measured after 24 hours of incubation. Error bars show 4/- | s_d. across three replicates. ](Exported%20image%2020250102022251-3.png)

[http://2018.igem.org/Team:Rice/Results](http://2018.igem.org/Team:Rice/Results)

|
|
==Plasmid== ==HW #== ==IGEM strength==
==pSPB927==HW16415||
==pSPB928==HW18567|==7==
==pSPB929==HW21117|1|
==pSPB930==HW29572|==10==
==pSPB931==HW31399||
==pSPB932==HW31422|==9==
==pSPB933==HW34701|==5==
==pSPB934==HW35539||
==pSPB935==HW36709|==8==
==pSPB936==HW36850|3|
==pSPB937==HW37769||
==pSPB938==HW24025|4|

![Translation Selected harris wang promoters pspag36 pSPB92g IDV_p9 pspgg31 pspg930 pspag33 p IDV_p10 pSPB935 pspag34 pSPBg32 pspag37 pSPBg38 pspa92B protein (logl O) organism ](Exported%20image%2020250102022252-4.png)

Plotting data subset from original paper : [Johns et al 2018](https://www-nature-com.ezproxy.rice.edu/articles/nmeth.4633)

All the HW in Shyam's box

Many 7-9.1 vectors from SS:: some Broad host range tooD

|   |   |   |
|---|---|---|
|![Machine generated alternative text:o o o o o o o o o o pss037 "sfgfp-AmpR-p88R1.mob+ (7-91) Last modified 4 minutes ago pss038 sfgfp-AmpR-RK20ri did not clone Last modified 3/8/2021 pss039 "sfgfp-AmpR-RSF1010mob+ (7-91) Last modified 4 minutes ago pSS040 sfgfp-AmpR-pUC Last modified 2/2212021 pSS041 sfgfp-AmpR-pMB1 Last modified Ills,'2021 pss042 sfgfp-AmpR-p15A Last modified 4/22/2021 pss043 sfgfp-AmpR-pSCIOl (1-6M) Last modified 3110/2021 pss044 sfgfp-KanR-p88R1mob+ Last modified pss045 sfgfp-KanR-RK20ri-oriT(lncP) did not clone Last modified 3/7/2021 pss046 sfgfp-KanR-pUC-oriT(lncP) Last modified 217/2021 pss047 sfgfp-KanR-p1SA-oriT(lncP) ](Exported%20image%2020250102022253-5.png) ![Machine generated alternative text:o o pss048 sfgfp-KanR-p88R1mob+-oriT(lncP) Last modified pss049 Last modified ](Exported%20image%2020250102022254-6.png)|![Machine generated alternative text:o o o o o o o o o o pssoso sfgfp-KanR-pMB1-oriT(lncP) Last modified pSS051 sfgfp-KanR-pSCIOl-oriT(lncP) Last modified pss052 Last modified 2/8/2021 pss053 did not clone Last modified 4/9/2021 pss054 sfgfp-ChLR-RK20n-oriT(lncP) Last modified 3/18/2021 pssoss did not clone Last modified pss056 sfgfp-AmpR-RK20ri-oriT(lncP) Last modified 2/3/2021 pss057 sfgfp-AmpR-p88R1mob+ Last modified pss058 sfgfp-AmpR-p88R1mob+-oriT(lncP) Last modified pss059 did not clone Last modified 3/7/2021 ](Exported%20image%2020250102022258-7.png)|![Machine generated alternative text:o o o o o o o o o o pSS060 sfgfp-ChlR-p88R1mob+-oriT(lncP) Last modified 3/8/2021 pSS061 Last modified pss062 did not clone Last modified 3/7/2021 pss063 did not clone Last modified pss064 pcfnmpch8-8SMT1-AmpR-plJC Last modified 4/30/2021 pSS065 sfgfp-ChlR-p15A-oriT(lncP) Last modified 3/15/2021 pss066 sfgfp-Ch'R-pSCIOl-oriT(IncP) (I-Sri) Last modified 3/15/2021 pss067 sfgfp-Ch'R-pM81-oriT(IncP) Last modified 4/4/2021 pss068 mScarlet I-AmpR-p1SA Last modified 3/26/2021 pss069 J23119-synRdS-pheS-tVojgtS4-kanR- Last modified 3/28/2021 ](Exported%20image%2020250102022300-8.png)|