# DREAM-PTB-Prediction-Using-Microarray

> Preterm birth (PTB), defined as giving birth prior to completion of 37 weeks of gestation, is the leading cause of newborn deaths and long-term complications including motor, cognitive, and behavioral impairment. Approximately one third of preterm births are medically indicated due to maternal or fetal conditions; the other two-thirds are categorized as spontaneous preterm births that include spontaneous preterm labor and delivery with intact membranes (sPTD) and preterm premature rupture of the membranes (PPROM).

As a team participant of [DREAM Preterm Birth Prediction Challenge, Transcriptomics](https://www.synapse.org/#!Synapse:syn18380862/wiki/590485) Sub-challenge 2 and a course project as well, we predicted Control vs. sTPD and Control vs. PPROM using microarray data by combining differential expression, co-expression, survival analysis and classification, and explored how imbalanced data, clustering, sample time and classifiers will influence the performance. 

In the folder `data`,
- The two top tables store top 1000 differentially expression genes (sorted by P value) in Control vs. sPTD and Control vs. PPROM respectively, created in R using the package `limma`. They can be reproduced in `DREAM_Differential expression analysis.Rmd`.
- The concordance results store top survival-related genes (sorted by absolute difference between the concordance indices and 0.5, higher indicates more influential), created in Python using the library `lifelines`. They can be reproduced in `DREAM_Survival analysis.ipynb`.
- `Supplementary Table S1.xlsx` stores the results of gene ontology analysis that contains gene IDs for each significantly
regulated biological processes.
