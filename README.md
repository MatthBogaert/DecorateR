[![CRAN checks](https://cranchecks.info/badges/summary/DecorateR)](https://cran.r-project.org/web/checks/check_results_DecorateR.html)
[![](https://www.r-pkg.org/badges/version/DecorateR?color=orange)](https://cran.r-project.org/package=DecorateR)
[![](https://img.shields.io/badge/devel%20version-0.1.1-orange.svg)](https://github.com/DecorateR)
[![](http://cranlogs.r-pkg.org/badges/grand-total/DecorateR?color=blue)](https://cran.r-project.org/package=DecorateR)


# DecorateR

`DecorateR`  allows you to build a Binary classification with DECORATE (Diverse Ensemble Creation by Oppositional Relabeling of Artificial Training Examples) (Melville and Mooney, 2005) The `DECORATE` function builds an ensemble of J48 trees by recursively adding artificial samples of the training data. Note that since `DecorateR` depends on Java there is only support for 64-bit machines.

# Installation

Before you install `DecorateR` make sure that you have installed `rJava` and `RWeka`. Also make sure that R correctly refers to the Java path. 

```
Sys.setenv('JAVA_HOME'="C:/Program Files/Java/jdk-15.0.1/")
if (!require("pacman")) install.packages("pacman")
pacman::p_load(rJava, RWeka)
```

If `rJava` and `RWeka` are correctly installed, you can install the package from CRAN.  

```
pacman::p_load(DecorateR)
```

To install the development version: 

```
pacman::p_load_current_gh("MatthBogaert/DecorateR")
```

# References

Melville, P., & Mooney, R. J. (2005). Creating diversity in ensembles using artificial data. *Information Fusion*, 6(1), 99-111. <doi: 10.1016/j.inffus.2004.04.001>
