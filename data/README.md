Common files in all 5 folders:
node_num: the number associated with each node in the network
inedges: a dictionary, where a key is a node and it's value is a list of its inputs
attractors_<model>: the biological attractors that each of the models recover (only high auxin levels attractors are given for the RSCN models)

Of the 5 folders here 2 of them are used for performing the statistical analysis of which we provide the folder structure for buylla_RSCN_2010A. The zhou folder has a similar folder structure and hence is not provided in this README. 

### buylla_RSCN_2010A (model 'A' from Azpeitia et al., 2010)
- signs: the regulatory signs of the inputs at each node in the same order as the inedges
- atleast: folder with data for the ensemble Root<sub>sc-NCF</sub> that recovers *atleast* the given biological fixed points
- exact: folder with data for the ensemble Root<sub>sc-NCF</sub><sup>*</sup> that recovers *exactly* the given biological fixed points
- buylla_RSCN_2010A.bnet: BoolNet file for the network
- edges_buylla_RSCN_2010A.txt: the edges of the network

The 3 other folders are for the 2013 RSCN, 2017 RAM and 2020 RSCN Boolean models. The contents of the buylla_RSCN_2020 folder are provided and is similar to the contents of buylla_RSCN_2013 and buylla_RSCN_2017, hence these 2 are not provided in this README.

### buylla_RSCN_2020 (RSCN model from Garcia-Gomez et al., 2020)
-MFPT_hier_buylla_RSCN_2020_10000.pkl: partial hierarchies obtained using MFPT after 10000 iterations
-MFTP_MST_info_buylla_RSCN_2020_10000.pkl: 
-MST_hier_buylla_RSCN_2020_10000.pdf: file of the 
-RSCN2020_best_models.txt: the model obtained by running the ipython notebook provided in the code folder
-expected_hierarchy_buylla_RSCN_2020.txt: the expected hierarchy of fixed points provided as pairwise inequalities
-buylla_RSCN_2020.bnet: BoolNet file for the 2020 model
-gene_BF_dict.pkl: dictionary where a key is a gene and its value is the set of BFs possible at that gene after imposing fixed point constraint and sc-NCF (except ARF5 which allows for sc-RoFs)
-org_BF_list.pkl: BFlist provided in the original model proposed in Garcia-Gomez et al., 2020
