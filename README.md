# cocov_paper
This repository contains some juypter notebooks and some small data files for the manuscript "High frequency body site translocation of nosocomial *Pseudomonas aeruginosa*". The original data for this study was produced by Thorpe *et al*. (2024) DOI: 10.1016/S2666-5247(24)00113-7 in a prospective cohort study that deep sequenced pathogens in a nosocomial setting. 

## Data Summary
Small data files can be found within the /data directory of the github page. The original metadata, (```data/fig2_translocation_simulations/clu_out_summaries_metadata.tsv``` in the notebooks) for the entire cocov study can be found within DOI: 10.1016/S2666-5247(24)00113-7 by Thorpe *et al*., in supplementary appendix 4. 

1. A whole phylogeny of all *P. aeruginosa* samples that were included within the study ```data/fig1_whole_tree/fig.1_whole_tree.tre```

2. Translocation simulations were based on combined ward metadata and clone classifcation data in the study. The code can be found within the ```src/translocation_simulations.ipynb``` jupyter notebook.
   In "Exploring Patient data" these metadata are processed to understand the diversity of clones that were found within each ward. 

   The "performing translocation simulations" section requires the supplementary appendix 4 table from Thorpe *et al* (2024) and corresponse to ```data/Extended_Data_Table3_cocov_study_data.tsv``` in the notebook. Functions needed to simulate translocations are defined at the top of the code block. An output directory is specified. 

   Some variables can be changed to match the those selected for the study. Comments can be found within the notebook.
   ```
   n_sim = 10
   tl_rate = 0.25
   tl_proportion = 1
   ```

3. The code to perform the marginla ancestral state reconstruction can be found within the ```src/cocov_ancestral_state_reconstruction.Rmd```. The tree and metadata files can be found within ```/data/fig3_translocation_direction```.




```
# All metadata from the original cocov study by Thorpe et al. 
clu_out_summaries_metadata.tsv
```