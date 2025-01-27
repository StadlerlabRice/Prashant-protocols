Excellent tutorial on how to understand .fcs files and general principles of analyzing it - [OpenFlow: Introduction to Flow Cytometric Data Analysis Part I](https://www.youtube.com/watch?v=z592Kack9B0) using FlowJo; part II uses FACS express   Terminology

- Region is a simple region in a plot
    
    - Gates are frequently hierarchical
- Gate is a combination of region   
   

Steps to data analysis

1. Check quality of data : parameters uniform over time
    
    - right click -> inspect on FlowJo (time axis is in sec) ; R's FlowAI and FlowClean
    - _If there is a gap for some duration of time, does that suggest clogging?_
2. Data exploration
    
    1. Use case: subsetting the correct population, ex : healthy cells or viability gating : Looks like mammalian cells' health influences scattering quite a bit (_death reduces FSC, increase SSC_), _not sure about bacteria though_
    2. FSC - SSC gating : debris is 10 K; cells are 60 - 1,200 K for the mammalian cells being shown
    3. **Tip**: _If the dominant channel of the fluorophore is saturated (which means voltage/gain was too high), look at a different channel_
    4. Linked plots: use "L" button for layouts, which are responsive to changes in the gating of the plot being explored; FCS express can do backgating - where you draw a gate but have it not be as a child of any gate
3. Gating order : Tip : it is easier to gate on bivariate scatter plots than on histograms with multi peaks
    
    1. Viability plot or FSC-SSC : Trying to gate for cells generously by excluding sureshot debris (_this improves statistics of % cells in further sub-regions_)
    2. Doublet discrimination : F/SSC A and H proportional for single cells : _Makes the region more generous to not loose any cells due to random variation_
        
        1. For more stringency if looking for rare cells, use FSC-A vs SSC-W
    3. Drag gate to all samples or sample group and press shift to toggle through the same open plots for all samples doing visual QC
4. Visuals :
    
    1. Layouts can create batch report - looping over each sample
    2. To overlay multiple samples visually, can select all regions at the same level and concatenate into a new .fcs file opened in flow automatically
5. Statistics: Put specific statistics such as mean, median, SD, CV etc. for each channel within a region . Use Table editor
    
    1. Can add formulas that combine stats of various regions for the same population
6. Saving : Flowjo workspace stores the gating data and the pointer to the data ; Archive stores both in a self contained file 
Voltage/signal tip : 2,00,000 is the max of the linear range for detection in usual machines
    

Questions

- Are there any resources for bacterial flow cytometry or is it just too simple to not warrant such?
    
    - Complications I see are : smaller cells, closer to debris
    - Analysis is simpler, which could be easier to automate