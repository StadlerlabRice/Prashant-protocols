**Selecting colonies**

- GlptP is repressed by adding 0.5 - 1% glucose on plates/media - useful for screening when colours are the same
 
- PCR amplified components has never worked differently in golden gates in my experience. NEB data shows it actually works worse since restriction enzymes work better on supercoiled DNA (_but this avoids having background transformants right?_..)

_Shyam sent March 17 at 5:44 PM_
 
Reg **RSF1010** (pSS026 -> pPK061)

- One theory is that for some reason RSF1010 can't be worked with in this context. And that's why Biki and I could never get an assembly with RSF1010 to work
- Btw, I would electroporate. Off chance that chemical works poorly with RSF1010 for a combination of size and supercoiling (nicked + made from relaxed fragments) reasons. And thus high efficiency less dependent on size/hydrodynamic radius helps significantly
 
- let's kill off the gfp colonies with a selective digest (_"__I might need to incorporate a third enzyme in the gg to chew up the original plasmids.."_ )
 > From <[https://www.facebook.com/](https://www.facebook.com/)>   
Something about avoiding natural terminators -- tVoigtN1 or N2 was the context - it had repeat or two tandem terminators
 
Troubleshooting **multigene assembly**

- Double the enzyme Esp3I to 1 ul per rxn
- Increase the cycle durations - 3 min and 5 min or something ; Charris swears by isothermal
 
Troubleshooting **multiple transformants** (double transformants)  
Add less gg rxn to transformation (~1 ul?)

- Do diagnostic digests with other enzymes as well for quick confirmation of **orientation** and mixed plasmids
 
**Operons**  
Don't use BCD in operon context, it's consequences are less understood
 
For **any assembly** that is not working, try to re-transform the connector parts (and subsequently other part plasmids) to troubleshoot for any degradation/contamination etc.
 
Isothermal golden gates take longer duration but have higher fidelity (of ligase)
   

BTK initial thoughts --  
Use case

- Make a slick backbone - with terminators flanking the desired coding region
- Need flexibility to include arbitrary spacers, transposase or att sites
    
    - Can have an unused golden gate site for ad hoc cloning after assembling things through the toolkit