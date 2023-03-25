Common files in 5 folders, namely, buylla_RSCN_2010A, buylla_RSCN_2013, buylla_RSCN_2017, buylla_RSCN_2020, zhou
- node_num: the number associated with each node in the network
- inedges: a dictionary, where a key is a node and it's value is a list of its inputs
- attractors_\<model_name\>: the biological attractors that each of the models recover (only high auxin levels attractors are given for the RSCN models); model_name is the folder name

Each of the 5 folders corresponds to one Boolean network. Of the 5 Boolean networks, 2 are used for performing the statistical analysis, namely zhou and buylla_RSCN_2010A. Both have similar folder structures and so we provide the contents for buylla_RSCN_2010A network.

### buylla_RSCN_2010A (model 'A' from Azpeitia et al., 2010)
The details for the sub folders within this folder are also provided as READMEs in those subfolders only for this model.
- atleast: folder with data for the ensemble Root<sub>sc-NCF</sub> that recovers *atleast* the given biological fixed points
- exact: folder with data for the ensemble Root<sub>sc-NCF</sub><sup>*</sup> that recovers *exactly* the given biological fixed points
- buylla_RSCN_2010A.bnet: BoolNet file for the ne twork
- edges_buylla_RSCN_2010A.txt: the edges of the network
- signs: the regulatory signs of the inputs at each node in the same order as the inedges

The 3 other folders for the 2013 RSCN, 2017 RAM and 2020 RSCN Boolean models have similar folder structures and so we provide the contents for buylla_RSCN_2020 network.

### buylla_RSCN_2020 (RSCN model from García-Gómez et al., 2020)
- MFPT_hier_buylla_RSCN_2020_10000.pkl: partial hierarchies obtained using MFPT with 10000 trajectories
- MFTP_MST_info_buylla_RSCN_2020_10000.pkl: MFTP matrix and the Minimum Spanning Arborescence (as a class file) using 10000 trajectories
- MST_hier_buylla_RSCN_2020_10000.pdf: image of the Minimum Spanning Arborescence obatained from the MFTP_MST_info_buylla_RSCN_2020_10000.pkl file
- RSCN2020_best_models.txt: the model obtained by running the ipython notebook provided in the code folder
- expected_hierarchy_buylla_RSCN_2020.txt: the expected hierarchy of fixed points provided as pairwise inequalities
- buylla_RSCN_2020.bnet: BoolNet file for the 2020 model
- gene_BF_dict.pkl: dictionary where a key is a gene and its value is the set of BFs possible at that gene after imposing fixed point constraint and sc-NCF (except ARF5 which allows for sc-RoFs)
- org_BF_list.pkl: List of BFs encoded as integers for the original model proposed in García-Gómez et al., 2020

### computational
- NCF_perms: each file in this folder contains a list of NCFs for a given number of inputs, the signs of which are activatory 
- RoF_perms: each file in this folder contains a list of RoFs for a given number of inputs, the signs of which are activatory
- UF_perms: each file in this folder contains a list of UFs for a given number of inputs, the signs of which are activatory

### References
Azpeitia, E., Benítez, M., Vega, I., Villarreal, C., & Alvarez-Buylla, E. R. (2010). Single-cell and coupled GRN models of cell patterning in the Arabidopsis thaliana root stem cell niche. BMC systems biology, 4(1), 1-19. \n

García-Gómez, M. L., Ornelas-Ayala, D., Garay-Arroyo, A., García-Ponce, B., Sánchez, M. D. L. P., & Álvarez-Buylla, E. R. (2020). A system-level mechanistic explanation for asymmetric stem cell fates: Arabidopsis thaliana root niche as a study system. Scientific reports, 10(1), 1-16.

### CITATION
A. Subbaroyan, P. Sil,  O. C. Martin & A. Samal. Leveraging Developmental Landscapes for Model Selection in Boolean Gene Regulatory Networks. bioRxiv. https://doi.org/10.1101/2023.01.08.523151
