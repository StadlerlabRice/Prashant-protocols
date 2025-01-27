> [!caution] This page contained a drawing which was not converted.   

Protocol for **LGC SAB beads** : [Manual](https://biosearchtech.a.bigcontent.io/v1/static/manual_SBXSAB_sbeadex-sab-sequencing-application-beads)  
Kit capacity : (533 runs of 50 ul DNA cleanup, dual size selection / 20 ml kit)
 
**DNA Cleanup** (> 100 bp : _removes primers and other PCR reagents_)

1. Prep : Bring beads to room temperature
    
    1. Mix beads, fully resuspend
    2. Have enough beads : ~35 ul per sample
    3. Make 75% ethanol (400 ul per cleanup) : 1,125 ul ethanol, 375 water = 1.5 ml
2. Binding: For x vol DNA, add ==1.5x vol of beads== (_See table below for excluding fragments 100 to 500 bp_). Add water to make DNA to 50 ul atleast (min = 50 ul DNA + 75 ul beads)
    
    - For RAM constructs, use ==0.7x volume== of beads (50 ul DNA + 35 ul beads) _since we want ~ 500 bp product_
    - Incubate 5 min ; shake every min~
    - Bring magnet into contact for 1 m. Aspirate supernatant with pipette, discard
3. Washing : Separate magnet, add 200 ul of 75% ethanol, mix thoroughly
    
    1. Incubate 2 m, periodic shaking every 30 sec~ (_optional shaking_)
    2. Bring magnetic contact for 1 m, discard supernatant with aspiration
4. Repeat washing second time
5. Dry bead pellet in open tube for 5 minutes
6. Elution : Add > 30 ul elution buffer (provided) and mix thoroughly
    
    1. Incubate 5 min ; shake every min~
    2. Bring magnetic contact for 1 m
    3. Transfer eluate to a new tube with pipette
 
Image of the workflow

![Exported image](Exported%20image%2020250102022328-0.png)   
**Size selection tables**

![Exported image](Exported%20image%2020250102022329-1.png)   
Dual size selection

![Exported image](Exported%20image%2020250102022331-2.png)   
---------------------------  
**References and product survey -**
 
Original paper - [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC307455/pdf/nar00022-0218.pdf](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC307455/pdf/nar00022-0218.pdf)  
DeAngelis, Margaret M., David G. Wang, and Trevor L. Hawkins. "Solid-phase reversible immobilization for the isolation of PCR products." _Nucleic acids research_ 23.22 (1995): 4742.
 
Explainer blog - [http://core-genomics.blogspot.com/2012/04/how-do-spri-beads-work.html](http://core-genomics.blogspot.com/2012/04/how-do-spri-beads-work.html)
   

Esthers protocol - [https://www.protocols.io/view/dna-size-selection-1kb-and-clean-up-using-an-optim-dm6gpyppgzpn/v1](https://www.protocols.io/view/dna-size-selection-1kb-and-clean-up-using-an-optim-dm6gpyppgzpn/v1)
   

**Vendors** -  
(Esther's choice) Ctyva Sera mag speed EAD carboxylate modified magnetic particles (hydrophobic) - 15 ml/500$  
Get speedbeads for 700$ : 45152105050250

- (old) 24152105050250 - [https://www.cytivalifesciences.com/en/us/shop/molecular-and-immunodiagnostics/magnetic-beads-and-kits/sera-mag-speedbeads-and-sera-mag-carboxylate-modified-magnetic-particles-p-05936](https://www.cytivalifesciences.com/en/us/shop/molecular-and-immunodiagnostics/magnetic-beads-and-kits/sera-mag-speedbeads-and-sera-mag-carboxylate-modified-magnetic-particles-p-05936)
   

Highly cost-effective alternative to AMPure XP beads in PCR and NGS clean-up and size selection applications  
[5 ml for 233$ ~125 dual side size selections of 50 ul DNA ] or ==20 ml/ 360$ :== NAP45002 : 533 preps of 50 ul

> From <[https://shop.biosearchtech.com/sequencing/ngs-kits-and-workflows/clean-up-and-size-selection-beads/sbeadex-sab-%28sequencing-application-beads%29/p/NAP45002](https://shop.biosearchtech.com/sequencing/ngs-kits-and-workflows/clean-up-and-size-selection-beads/sbeadex-sab-%28sequencing-application-beads%29/p/NAP45002)>  

User manual : [https://biosearchtech.a.bigcontent.io/v1/static/manual_SBXSAB_sbeadex-sab-sequencing-application-beads](https://biosearchtech.a.bigcontent.io/v1/static/manual_SBXSAB_sbeadex-sab-sequencing-application-beads)
 
Other options discussed here -  
[https://www.reddit.com/r/labrats/comments/c349gr/has_anyone_tried_any_less_expensive_alternatives/?utm_medium=android_app&utm_source=share](https://www.reddit.com/r/labrats/comments/c349gr/has_anyone_tried_any_less_expensive_alternatives/?utm_medium=android_app&utm_source=share)
 
cube biotech magnetic beads -- search
   

Instead of AMPure, we've switched to a more affordable option, a drop-in replacement for AMPure, MagBio HighPrep PCR beads
    
---------------  
**Processing steps for beads purification (for robot)**

1. Add 35 ul of beads from a reservoir to fresh plate (plate B) (_beads need to be freshly vortexed_)
2. Transfer 50 ul of PCR amplified products (from plate A) into the above plate and mix 10 times
3. Incubate for 5 min (_5 min from the first transferred sample?_)
4. Turn on the magnet (or move the sample plate onto a magnet), hold for 1 min
5. Remove the supernatant and discard. Separate samples from magnet
6. Add 200 ul of 75% ethanol and mix by pipetting 10 times
7. incubate 2 m and turn on the magnet for 1 min
8. Discard supernatant and repeat 6-8 one more time
9. Dry the bead pellet in open tube for 5 min
10. Add 30 ul of elution buffer and mix throughly by pipetting 10x
11. Incubate 5 min, turn on magnet for 1 m
12. Transfer elution into a fresh plate.