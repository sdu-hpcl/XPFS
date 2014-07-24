#MPFS

*  A new method to search PROSITE profile on XEON Phi.

##Introduction
* XPFS is a high performance database searching method based on the Intel(R) MIC platform. We have used a two-level parallelization scheme: the thread level coarse-grained and VPU level fine-grained parallelism to implement our algorithm. We gain 3 times faster than PFSearchV3 on the Xeon Phi 7110p.

##Installation and Usage
* Query profiles and database are needed to run XPFS. Profiles can be downloaded at [ftp://lausanne.isb-sib.ch/pub/software/unix/pftools/pftoolsV3/pftoolsV3.PROSITE.tar.gz]. And databse should be in FASTA format.

#### Run XPFS 
  * `./XPFS -t nCpus -T nMics <queryProfile> <database>` 
  * nCPUs : number of cpu thread; nMICs : number of Xeon Phi cards (Currently only one card supported)
  * for more details, you can run :
  * `./XPFS -h`


##Reference

##Authors and Contributors
* Weiguo Liu is the corresponding author.

##Support or Contact
* If you have any questions, please contact: Weiguo,Liu ( weiguo.liu@sdu.edu.cn).
