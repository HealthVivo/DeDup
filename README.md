# DeDup
A merged read deduplication tool capable to perform merged read deduplication on single end data. 

[![Build Status](https://lambda.informatik.uni-tuebingen.de/jenkins/buildStatus/icon?job=DeDup)](https://lambda.informatik.uni-tuebingen.de/jenkins/view/EAGER/job/DeDup/)
[![codecov](https://codecov.io/gh/apeltzer/DeDup/branch/master/graph/badge.svg)](https://codecov.io/gh/apeltzer/DeDup)
[ ![Download](https://api.bintray.com/packages/apeltzer/EAGER/DeDup/images/download.svg) ](https://bintray.com/apeltzer/EAGER/DeDup/_latestVersion)

Author: Alexander Peltzer <alexander.peltzer@uni-tuebingen.de>

###### Method
The DeDup tool is designed to work with forward, reverse and merged reads (forward and reverse combined to make a single read).
DeDup expects the different kinds of reads to have read names that begin with one of the following prefixes:

- F_
- R_
- M_

To remove PCR duplicates we only retain a single read for a given genomic position and read direction. For M_ (merged) reads we know both the start and end of the sequenced fragment. For F_ and R_ reads we only know the start or end of the sequenced fragment becuase the read length is variable.

 
A little documentation is available at http://dedup.readthedocs.io/en/latest/
