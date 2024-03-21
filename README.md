# Eucs_phylo_traits

The following is code used to measure functional trait correlations with and without phylogenetic adjustment, phylogenetic signal, and differences in traits between taxa employing different fire-response strategies. Started August 2020 and completed December 2023. Collaborators: Antoinette Portelli, Peter Vesk, and Saras Windecker. Results published in 'From mallees to mountain ash, specific leaf area is coordinated with eucalypt tree stature, resprouting, stem construction, and fruit size' authored by Antoinette M. Portelli, Saras M. Windecker, Laura J. Pollock, Will. C. Neal, William K. Morris, Rohan Khot and Peter A. Vesk (found at https://doi.org/10.1071/BT23028).

In order for the following scripts to run, input data and output folders must have the same relative locations to the Scripts folder as they do in this repository. I.e. All notebooks must be in a folder named 'Scripts', input data files must be in an adjacent folder named 'Input_data', there must be adjacent 'Intermediate_Tree_Building_Products', and the folder where all outputs are to go must be another adjacent folder named 'Output_figures'. 'Output_figures' must also have a folder within it called 'Potential_trees_and_results'.

Notebooks (also called scripts interchangeably throughout this project) are designed to be run in numerical order with or without clearing the environment between each script/notebook. The exception is the order of notebooks beginning with '2', '3', and '3a', which are part of the process of building the phylogenetic tree used in this analysis. If readers would like to skip over the tree building process and associated checks and decision-making contained in notebooks 2 and 3a (i.e. also the construction of supplementary Table S3.1 of the manuscript), a newick file of the final version of the phylogenetic tree used in all subsequent analyses can also be found in the Input_data folder (final_tree.txt). This allows notebooks to be run in the order 1, 2 (line 1283 onwards only), 3, 4, 5, 6, and 7 instead with identical results (though some supplementary figures and tables may be missing).

If running all scripts, script 1 can be run followed by the first 1183 lines of script 2 before things get a bit complicated. The first 650 lines of the notebook '3a_Phylogenetic Signal for 14 potential trees_final.Rmd' must then be run (as instructed in that script) before continuing with  the remainder of notebook '2_Building_Tree_Using_Thornhill_and_Bayly_Trees_final.Rmd' (lines 1186-end). Notebook '3_Phylogenetic Signal Calculations.Rmd' must then be run completely before the remainder of notebook '3a_Phylogenetic Signal for 14 potential trees_final.Rmd' (lines 655-end) can be run. In summary, scripts are run in the following order: 1, 2 (lines 1-1183), 3a (lines 1-650), 2 (lines 1186-end), 3, 3a (lines 655-end), 4, 5, 6, 7.

The data file, 'median_data_ms_ver2.csv', published on Zenodo (location: https://doi.org/10.5281/zenodo.8313641) does also contain all data used in the analysis, but contains only untransformed data and excludes several variables that may be useful for intermediate data handling. Scripts will not recognise this data object.
