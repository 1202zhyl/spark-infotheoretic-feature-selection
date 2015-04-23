**Information Theoretic Feature Selection Framework**

The present framework implements Feature Selection (FS) on Spark for its application on Big Data problems. This package contains a generic implementation of greedy Information Theoretic Feature Selection methods. The implementation is based on the common theoretic framework presented in [1]. Implementations of mRMR, InfoGain, JMI and other commonly used FS filters are provided. In addition, the framework can be extended with other criteria provided by the user as long as the process complies with the framework proposed in [1].

-- Main features:
* Support for sparse data (in progress).
* Pool optimization for high-dimensional.
* Improved performance from previous version.

This work has associated two submitted contributions to international journals which will be attached to this request as soon as they are accepted This software has been proved with two large real-world datasets such as:

- A dataset selected for the GECCO-2014 in Vancouver, July 13th, 2014 competition, which comes from the Protein Structure Prediction field (http://cruncher.ncl.ac.uk/bdcomp/). The dataset has 32 million instances, 631 attributes, 2 classes, 98% of negative examples and occupies, when uncompressed, about 56GB of disk space.
- Epsilon dataset: http://www.csie.ntu.edu.tw/~cjlin/libsvmtools/datasets/binary.html#epsilon. 400K instances and 2K attributes.

-- Brief benchmark results:

* 150 seconds by selected feature for a 65M dataset with 631 attributes. 
*  For epsilon dataset, we have outperformed the results without FS for three classifers (from MLLIB) using only 2.5% of original features.

Design doc: https://docs.google.com/document/d/1HOaPL_HJzTbL2tVdzbTjhr5wxVvPe9e-23S7rc2VcsY/edit?usp=sharing

References

[1] Brown, G., Pocock, A., Zhao, M. J., & Luján, M. (2012). 
"Conditional likelihood maximisation: a unifying framework for information theoretic feature selection." 
The Journal of Machine Learning Research, 13(1), 27-66.
