# GGN_clusters
For an input genome in FASTA format, the program GGN_clusters prints in bed files all clusters containing at least &lt;GGNmin> triplets of nucleotides GGN, where N is any nucleotide, separated by at most L intermediate nucleotides.

PROGRAM GGN_clusters

Author: Ugo Bastolla <ubastolla@cbm.csic.es>,

Centro de Biologia Molecular Severo Ochoa(CSIC-UAM), Madrid Spain

For an input genome in FASTA format, the program GGN_clusters prints in bed
files all clusters containing at least <GGNmin> triplets of nucleotides GGN,
where N is any nucleotide, separated by at most L intermediate nucleotides.

Furthermore, for all possible dinucleotides XYN, where N is any nucleotide, it
computes the propensity that there are two XYN triplets at distance d and the
propensity that the two nucleotides N are identical, and it prints them in text
files Cond_prob_XYN.dat

===============================================
INSTALL:

Download GGN_clusters_source.zip and run the following:

unzip GGN_clusters_source.zip

make

cp GGN_clusters (your path of binary files)

====================================================
USAGE: GGN_clusters Input_GGN_clusters
====================================================
FORMAT of the configuration file Input_GGN_clusters:

LOOP=<>    ! Max. distance between GGN triplets

GGNmin=<>  ! Min. number of GGN to call a cluster

GGNmax=<>  ! Max of min. number of GGN to call a cluster

store_GG=<0,1> ! 1=Find both triplets GGN and doublets GG

Examine_doublet=<0,1> ! 1=Examine both triplets GGN and doublets GG

print_AA=<0,1> ! 1=Find also triplets AAN and doublets AA

print_GG=<0,1> ! 1=Print GGN (default)

CHROMOSOMES:

DIR=<>  Directory with chromosome sequences

<>      Files with chromosomes

END
<>      Files with chromosomes
END
