# genX

This is a set of R functions that infers a species tree from gene trees estimated, possibly with error, from DNA sequences.  It is based on the GLASS/Maximum Tree as implemented in STEM, but attempts to correct for the error between true and estimated gene trees using clustering in general measurement error models.  It is relatively fast and showed improved accuracy over STEM in terms of RF distance from the true species tree in simulation studies and two empirical datasets. 

It does require an estimate of the population scaled mutation rate theta.  While the value of theta does not affect the topology returned by STEM, not supplying a reasonably accurate estimate of it here (say, using 1) can result in negative distance estimates between species and does affect the topology.  For the simulated data that this function was tested on, theta was known.  For the empirical datasets, the function performed satisfactorily with theta estimated using the 'pegas' R package.


Papers referenced are shown below.

GLASS:  
[E. Mossel and S. Roch. Incomplete lineage sorting: Consistent phylogeny estimation from multiple loci. IEEE/ACM Transactions on Computational Biology and Bioinformatics, 7(1):166–171, 2010.](https://ieeexplore.ieee.org/document/4564437)

Maximum Tree:  
[L. Liu, L. Yu, and D. K. Pearl. Maximum tree: a consistent estimator of the species tree. J. Math. Biol., 60:95–106, 2010b.](https://link.springer.com/article/10.1007/s00285-009-0260-0)

STEM:  
[L. Kubatko, B. Carstens, and L. Knowles. STEM: Species tree estimation using maximum likelihood for gene trees under coalescence. Bioinformatics, 25(7):971– 973, 2009.](https://doi.org/10.1093/bioinformatics/btp079)

Clustering in general measurement error models:  
[Y. Su, J. Reedy, and R. J. Carroll. Clustering in general measurement error models. Statistica Sinica, 28(4):2337–2351, 2018](http://www3.stat.sinica.edu.tw/statistica/J28N5/J28N57/J28N57.html)


Not explicitly referenced, but why we attempted to improve STEM to begin with:  
[M. DeGiorgio and J. Degnan. Robustness to divergence time underestimation when inferring species trees from estimated gene trees. Syst. Biol., 63(1):66–82, 2014.](https://doi.org/10.1093/sysbio/syt059)
