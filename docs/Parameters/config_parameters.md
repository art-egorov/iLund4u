# Configuration file parameters


iLund4u configuration file allows detailed customization of the tool's parameters.

***Note:***  
You can copy the *lovis4u_data* folder that contains the config files to your wiking directory with `ilund4u --data` command and safely edit and use them without affecting 'internal' config. If you want to use a copied config file, use `-c path_to_config`.



##### Detailed description is under construction...

---

**;[Data Loading and processing]**  
default_transl_table = 11  
gff_CDS_name_source = product  
min_proteome_size = 15  
proteome_uniqueness_cutoff = 0.7  
proteome_similarity_cutoff = 0.7  
leiden_resolution_parameter_p = 0.5  
min_proteome_community_size = 10  
circular_genomes = True  
variable_protein_cluster_cutoff = 0.25  
conserved_protein_cluster_cutoff = 0.75  
neighbours_max_distance = 8  
neighbours_one_side_max_size = 5  
neighbours_min_size = 5  
island_neighbours_similarity_cutoff = 0.65  
leiden_resolution_parameter_i = 0.55  
deduplicate_proteomes_within_hotspot = True  
hotspot_presence_cutoff = 0.3  
hotspot_signature_presence_cutoff = 0.75  
hotspot_similarity_cutoff = 0.65  
leiden_resolution_parameter_h = 0.55  
protein_search_target_mode = group  

**;[mmseqs parameters]**  
mmseqs_cluster_mode = 0  
mmseqs_cov_mode = 0  
mmseqs_min_seq_id = 0.25  
mmseqs_c = 0.8  
mmseqs_s = 7  
mmseqs_search_qcov = 0.6  
mmseqs_search_tcov = 0.6  
mmseqs_search_fident = 0.2  
mmseqs_search_evalue = 1e-5  

**;[pyhmmer hmmscan parameters]**  
hmmscan_query_coverage_cutoff = 0.7  
hmmscan_hmm_coverage_cutoff = 0.5  

**;[visualisation]**  
show_hmmscan_hits_on_full_proteomes = True  
lovis4u_hotspot_vis_figure_width = 8  
lovis4u_hotspot_mm_per_nt = 0.0125  
lovis4u_proteome_mm_per_nt = 0.005  
index_only_for_hypothetical_proteins = auto  
island_size_cutoff_to_show_index_only = 7  
max_number_of_seqs_to_redefine_order = 300  

**;[HMM]**  
hmm_defence= {internal}/HMMs/DefenceFinder_CasFinder  
hmm_virulence =  {internal}/HMMs/VFDB  
hmm_anti_defence = {internal}/HMMs/dbAPIS_Acr  
hmm_amr = {internal}/HMMs/AMRFinderPlus  
database_names = Defence,Virulence,Anti-defence,AMR  

**;[Other paths]**  
mmseqs_binary = {internal}/bin/mmseqs_mac/bin/mmseqs  
category_colours = {internal}/category_colours_proteome_groups.tsv  

**;[Output]**  
verbose = True  
debug = False  
output_dir = ilund4u_{current_date}  

**;[URLs]**  
hmm_models = https://data-sharing.atkinson-lab.com/iLund4u/HMMs.tar.gz  
plasmids_db = https://data-sharing.atkinson-lab.com/iLund4u/iLund4u_DB-plasmids.tar.gz  
phages_db = https://data-sharing.atkinson-lab.com/iLund4u/iLund4u_DB-phages.tar.gz  
