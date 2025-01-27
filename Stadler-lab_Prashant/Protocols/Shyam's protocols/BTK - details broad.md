Part definitions

|
|
  ==Type== ==5' BsaI >== ==< 3' BsaI==
==ConL== ==1== ==ACGG== ==CTTC==
==Promoter== ==2== ==CTTC== ==CGAC==
==Ribozyme== ==3a== ==CGAC== ==TCAG==
==5′ UTR / RBS== ==3b== ==TCAG== ==AATG==
==CDS 1== ==4a== ==AATG== ==TTCC==
==CDS 2== ==4b== ==TTCT== ==ATCC==
==CDS 3== ==4c== ==ATCC== ==TGGC==
==Terminator / 3' UTR== ==5== ==TGGC== ==GCTG==
==ConR== ==6== ==GCTG== ==TACA==
==Selection Marker== ==7== ==TACA== ==GAGT==
==TF/Custom== ==8== ==GAGT== ==CCAA==
==3' Homology== ==9a== ==CCAA== ==GGTC==
==Cond. Origin== ==9b== ==GGTC== ==GATA==
==5' Homology== ==9c== ==GATA== ==ACGG==

   
**ATG:** Start codon is included in the connector, remove it from the CDS part
 
**Part type overhangs**

|   |   |   |   |   |   |
|---|---|---|---|---|---|
|**Name**|**BTK Type**|**5' BsaI**|**3' BsaI**|**5' Primer Overhang >**|**3' Primer Overhang >**|
|**ConL**|**1**|ACGG|CTTC|gtCGTCTCactcgACGG|caCGTCTCactctGAAG|
|**OpConL**|**12**|ACGG|CGAC|gtCGTCTCactcgACGG|caCGTCTCactctGTCG|
|**Promoter**|**2**|CTTC|CGAC|gtCGTCTCactcgCTTC|caCGTCTCactctGTCG|
|**Promoter a**|**2a**|CTTC|CGCA|gtCGTCTCactcgCTTC|caCGTCTCactctTGCG|
|**Promoter b**|**2b**|CGCA|CGAC|gtCGTCTCactcgCGCA|caCGTCTCactctGTCG|
|**RBS/5'UTR**|**3**|CGAC|AATG|gtCGTCTCactcgCGAC|caCGTCTCactctCATT|
|**Ribozyme Insulator**|**3a**|CGAC|TCAG|gtCGTCTCactcgCGAC|caCGTCTCactctCTGA|
|**RBS**|**3b**|TCAG|AATG|gtCGTCTCactcgTCAG|caCGTCTCactctCATT|
 
< stop-start:

```
tA
A
TG

ggT
TCC

ggA
TCT

























```

ATG  
< GlySer: ggTTCC  
< GlySer: ggATCT

Enzymes used and entry vectors
 
|
|
==# of constituents== ==# of the final part== ==Stage====
Type IIs  
restriction enzyme
====Entry vectors (to make a part at this level)== ==More entry vectors==
|Pcr pdts|0 = parts|Part assembly|Esp3I (Thermo)|pSPB430-pUC19-ChlR-{sfGFP}dropout|-|
|0's|1 = casettes|Cassette assembly  <br>(combine parts 0)|BsaI-HF.V2|pSPB438 ~sfgfp AmpR pUC (7-9.0) <old name: 1-6r.0>|- pSPB439-p15A-AmpR **(1-6r.0)**<br>- pSPB780 ~gfp ChlR RSF1010.mob (1-6r.0)<br>- pSPB868- ~gfp KanR RSF1010.mob (1-6r.0)|
|1's|0 (or 2) = multigenes (MG)|Multigene assembly (combine parts 1)|Esp3I (Thermo)||- pSPB781 ~gfp ChlR tVoigtN17 RSF1010.mob (1-6r.1)|
||..|||||
 
**Note**: 1-6r.1 is the same as newer convention 7-9.1 - Here 1-6r means that 1-6 segment drops out to leave the 7-9 go into the next level  
The parts of a level (let's say 0) combine to make a part of the next level (say 1)
 ![A. S— DNA "Level I" g. Level O Level 1 Level O Level I 1 day I day If 1 day ](Exported%20image%2020250102022236-0.png)   ![Construct Verification • Al/ assemblies: Notl sites flanking • Multigene assemblies: Sbfl sites in scars separating tx units • Super-multigene assembly: Ascl sites separate roDT multigenes Notl Sbfl Sbfl Notl Sbfl O ](Exported%20image%2020250102022238-1.png)
 
**Naming explanations - Shyam**
 
That's not the right use of the term "vector". Vector is the contiguous span of backbone elements, in the BTK case (7–9). So "Dropout vectors" are vectors (7-9) with a GG dropout part, thus all BTK vectors are dropout vectors, since (7-9) aren't ever made without a dropout. **Dropout** **PARTS** are (1-6r.0) for BsaI, (1-6r.1) for Esp3I.
 > From <[https://www.facebook.com/messages/t/520859181](https://www.facebook.com/messages/t/520859181)>