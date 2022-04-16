# genX

This is a set of R functions that infers a species tree from gene trees estimated, possibly with error, from DNA sequences.  It is based on the GLASS/Maximum Tree as implemented in STEM, but attempts to correct for the error between true and estimated gene trees using the method of clustering in general measurement error models discussed by Su et. al.  It is relatively fast and did show improved accuracy over STEM in terms of RF distance from the true species tree in simulation studies and two empirical datasets.


GLASS:
E. Mossel and S. Roch. Incomplete lineage sorting: Consistent phylogeny estimation from multiple loci. IEEE/ACM Transactions on Computational Biology and Bioinformatics, 7(1):166–171, 2010.

Maximum Tree:
L. Liu, L. Yu, and D. K. Pearl. Maximum tree: a consistent estimator of the species tree. J. Math. Biol., 60:95–106, 2010b.


STEM:
L. Kubatko, B. Carstens, and L. Knowles. STEM: Species tree estimation using maximum likelihood for gene trees under coalescence. Bioinformatics, 25(7):971– 973, 2009.

Clustering in general measurement error models:
Y. Su, J. Reedy, and R. J. Carroll. Clustering in general measurement error models. Statistica Sinica, 28(4):2337–2351, 2018.
