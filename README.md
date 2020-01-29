# SautuaPMS2020

The alignments for the maximum likelihood (ML) and Bayesian phylogenetic analyses as well as the resulting inferred phylogenies are contained in this repository. The input files and resulting trees are contained in folders for the ML and Bayesian analyses, resepctively.

Below is information regarding methods pertinent to the data in this repository. These methods are an excerpt from the manuscript submitted to Plant Management Science (PMS).

Title: Fungicide resistance in Cercospora species causing Cercospora leaf blight and purple seed stain of soybean in Argentina

Authors: Francisco J Sautua<sup>a</sup>, Vinson P Doyle<sup>b</sup>, Paul P Price<sup>c</sup>, Alejandro Porfiri<sup>d</sup>, Paula Fernandez<sup>e,f</sup>, Maria M Scandiani<sup>g</sup>, Marcelo A Carmona<sup>a,*</sup>

<sup>*</sup> Correspondence to: Marcelo M Carmona, Cátedra de Fitopatología, Facultad de Agronomía, Universidad de Buenos Aires, Av. San Martín 4453, C.A.B.A, C1417DSE, Argentina. E-mail: carmonam@agro.uba.ar 

<sup>a</sup> Universidad de Buenos Aires, Facultad de Agronomía, Cátedra de Fitopatología, Buenos Aires, Argentina;

<sup>b</sup> Department of Plant Pathology and Crop Physiology, LSU AgCenter, Baton Rouge, LA 70803;

<sup>c</sup> Macon Ridge Research Station, LSU AgCenter, Winnsboro, LA 71295;

<sup>d</sup> Independent consultant

<sup>e</sup> Consejo Nacional de Investigaciones Científicas y Técnicas, Ciudad Autónoma de Buenos Aires, Argentina

<sup>f</sup> Instituto de Biotecnología, Centro de Investigaciones en Ciencias Agronómicas y Veterinarias, Instituto Nacional de Tecnología Agropecuaria, Hurlingham, Argentina

<sup>g</sup> Centro de Referencia de Micología (CEREMIC), Facultad de Ciencias Bioquímicas y Farmacéuticas, Universidad Nacional de Rosario, Rosario, Argentina.

Methods (Phylogeny-related)

## Methods
### Fungal isolates

From 2014 to 2019, isolates of Cercospora spp. were obtained from symptomatic soybean leaves and seeds sampled from commercial soybean fields throughout Argentina and Santa Cruz, Bolivia. The isolation was performed according to the method used and described by Price et al. (2013, 2015a). In Argentina, Cercospora isolates had been exposed mainly to carbendazim and QoI + DMI mixtures, whereas in Bolivia they had been exposed to QoI, DMI, SDHI, MBC and multisite fungicides such as mancozeb. In all, 516 single-conidium isolates of Cercospora spp. were collected from 67 locations in 9 different provinces in Argentina (Supplementary Figure 1) and 38 isolates were obtained from Santa Cruz, Bolivia (Sautua et al., 2019a). Isolates were maintained on potato dextrose agar (PDA; Britania, Buenos Aires, Argentina) at 25°C with a 16h light : 8h dark cycle and preserved with three different storage methods: a) in cryovials with sterile water at 4°C, b) in PDA slants covered with sterile mineral oil at room temperature and c) in 20% glycerol at -40°C. All isolates are deposited in the fungal culture collection of the Plant Pathology Department of the University of Buenos Aires (FAUBA, Argentina). For the present study, 62 Argentinean and 3 Bolivian isolates from different locations were chosen to represent surveyed areas equitably (Table 1). To this end, the total sample in Argentina was divided into 3 regions: northwest, center and southeast (green, yellow and orange in Supplementary Figure 1, respectively). Within each area the isolates were chosen at random. Of the total sample from Bolivia, an isolate of each species determined in a previous study (Sautua et al., 2019a) was chosen at random. Thus, in total, the present study included 65 isolates for the in vitro fungicide sensitivity tests and the exploration of mutations that confer resistance to fungicides. Of these 65 isolates, 42 were chosen to perform a phylogenetic analysis to determine the species identity.

### DNA extraction

For DNA extraction, liquid cultures of isolates were initiated by placing small pieces of mycelium into 250-mL flasks containing 50 mL potato dextrose broth (FDA, 2004). The initial mycelium was carefully scraped with a sterile needle from the aerial mycelia of cultures growing on PDA plates. The liquid cultures were incubated for 3 days in the dark with constant shaking provided by a standard shaker. After incubation, mycelia were recovered with a strainer and approximately 600 mg of tissue was transfered to a sterile 1.5 mL microcentrifuge tube. Genomic DNA was extracted following the Dellaporta protocol (Dellaporta et al., 1983). Quantification and quality control of extracted DNA was performed with a Nanodrop spectrophotometer (Thermo Fisher Scientific, Waltham, MA, USA) and afterwards diluted to a working concentration of 12 ng µL-1.

 

### Isolate identification

#### actA, cmdA, gapdh, his3 and tef1 amplification and sequencing

Forty two isolates were chosen to be characterized by sequencing portions of five nuclear loci (actin (actA), calmodulin (cmdA), glyceraldehyde-3-phosphate dehydrogenase (gapdh), histone 3 (his3) and translation elongation factor 1-α (tef1)) (Supplementary Table 1) and aligning them with data from 379 other isolates in Groenewald et al. (2013) and Bahkshi et al. (2018) (see 2.4.2). Fragments of actA, cmdA, gapdh, his3 and tef1 genes were amplified from genomic DNA with the primers described in Table 2. The protocols and PCR conditions were those previously described (see references in Table 2). All PCR products were purified and sequencing services were performed by Macrogen Inc. (Seoul, South Korea, www.macrogen.com). Sequencing reactions were carried out with the same primers as in the PCR amplifications.

 

#### Model testing, phylogenetic analysis and species assignment

Sequences were edited and contigs assembled in Geneious 8.1.3. Each locus was aligned using iterative refinement methods implemented in MAFFT v. 7 (Kuraku et al., 2013; Katoh et al., 2019) with the G-INS-I algorithm, a 200PAM/k=2 scoring matrix, gap penalty of 1.53 and offset of 0.0. Individual locus alignments were concatenated into a multilocus alignment including data from the nuclear ribosomal internal transcribed spacers (nrITS) published by Groenewald et al. 2013, actin, cmdA, his3, translation elongation factor 1, and gapdh. Septoria provencialis CPC_12226 was included as an outgroup. The maximum likelihood phylogeny for each gene and the concatenated alignment were estimated using the parallel AVX version of RAxML v. 8.2.12 (Stamatakis 2014) specifying the GTR model of nucleotide evolution and a Γ distribution on rate heterogeneity across sites. Bipartition support was estimated with 1000 bootstrap replicates for each analysis (mpirun raxmlHPC-MPI-AVX -f a -x 12345 -p 12345 -# 1000 -m GTRGAMMA). Prior to Bayesian inference, the best-fit model of nucleotide evolution and best partitioning scheme across alignments was estimated in Partition Finder 2 (Lanfear et al. 2016) specifying the greedy algorithm (Lanfear et al. 2012) with linked branch lengths and using the corrected Akaike information criterion for selecting the best-fit model among the set of models considered for MrBayes. The joint posterior distribution of parameter values and tree topologies for the concatenated, partitioned multilocus dataset was estimated in MrBayes v. 3.2.6 (Ronquist et al. 2012) with four replicate Markov chain Monte Carlo (MCMC) runs, four Metropolis-coupled chains per run (one cold and three heated), and 2.5 million generations per run with a sampling frequency of 1000. Convergence was determined by observing a standard deviation of split frequencies below 0.1 and effective sample sizes (ESS) above 200 for most parameters, discarding the first 50% of samples as burnin. The majority-rule consensus phylogeny was computed using SumTrees v. 4.3.0 in Dendropy v. 4.3.0 (Sukumuran and Holder, 2010). The bipartitions with a posterior probability equal to or greater than 0.85 were mapped, if present, to the maximum likelihood phylogeny alongside the maximum likelihood bootstrap support values greater than 50%. All alignments and phylogenetic trees have been deposited to a Github repository (https://github.com/vinsondoyle/SautuaPMS2020). Species assignments were based on the results of the concatenated phylogenetic analyses and comparisons with each single locus phylogenetic analysis.
