On Thu, Oct 5, 2023 at 2:26 PM Shyam Bhakta <[shyampbhakta@gmail.com](mailto:shyampbhakta@gmail.com)> wrote:  
----
 
Voigt synthetic terminators can be mildly recombinogenic. Below are the EFM Calculator predictions. Nomenclature: S4 = tVoigtS4, etc.  
With new connectors, prefer to use (S4 and maybe S12, S14) together, or (S6, S7, S12). Note that new ConL's contain S10.  
With old connectors, prefer to use S3, S4, S11, (S12) together. Note that old ConR's contain an internal S1.  
Any natural connectors with these are probably fine, as are bidirectional terminators T###. For double terminators DT##, consider which, if any, Voigt synthetic terminator(s) are annotated inside. The ones I domesticated all have only orthogonal natural terminators except for DT5 which contains S1 (and is ~13× stronger than S1 alone).  
Terminator pairs can have different homology lengths on the 5' end versus 3' end, hence their repeat in the list.
   

|   |   |   |
|---|---|---|
|Terminator pairs|Seq Identity length|Pred Recomb rate|
|S4, S6|27|3.06E-06|
|S4, S7|28|1.72E-06|
|S7, S11|27|1.40E-06|
|S1, S3|22|8.43E-07|
|S1, S3, S10|21|7.55E-07|
|S1, S10|28|6.36E-07|
|S4, S6|18|1.90E-07|
|S7, S11|20|1.53E-07|
|S1, S3, S10, S14|16|8.17E-08|
|S4, S12|16|3.41E-09|
|* events/cell/generation|||

> ￼-------------------  

I have used the Salis lab's non-repetitive parts calculator to make sure that the terminators I use with your system will have minimal recombination.  
[https://salislab.net/software/nrp_calculator_finder](https://salislab.net/software/nrp_calculator_finder)
 
-Zach
 > From <[https://mail.google.com/mail/u/0/#starred/FMfcgzGtxTBWpfqMGhSRbHSjTbjLlSWR](https://mail.google.com/mail/u/0/#starred/FMfcgzGtxTBWpfqMGhSRbHSjTbjLlSWR)>   >