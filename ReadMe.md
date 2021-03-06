### [R/qtl2](http://kbroman.org/qtl2)

[R/qtl2geno](https://github.com/rqtl/qtl2geno):
[![Build Status](https://travis-ci.org/rqtl/qtl2geno.png?branch=master)](https://travis-ci.org/rqtl/qtl2geno) <br/>
[R/qtl2scan](https://github.com/rqtl/qtl2scan):
[![Build Status](https://travis-ci.org/rqtl/qtl2scan.png?branch=master)](https://travis-ci.org/rqtl/qtl2scan) <br/>
[R/qtl2plot](https://github.com/rqtl/qtl2plot):
[![Build Status](https://travis-ci.org/rqtl/qtl2plot.png?branch=master)](https://travis-ci.org/rqtl/qtl2plot) <br/>
[R/qtl2convert](https://github.com/rqtl/qtl2convert):
[![Build Status](https://travis-ci.org/rqtl/qtl2convert.png?branch=master)](https://travis-ci.org/rqtl/qtl2convert)

[Karl Broman](http://kbroman.org)

[R/qtl2](http://kbroman.org/qtl2) (aka qtl2) is a reimplementation of
the QTL analysis software [R/qtl](http://www.rqtl.org), to better
handle high-dimensional data and complex cross designs. It is split
into [qtl2geno](https://github.com/rqtl/qtl2geno) (for calculating
genotype probabilities, imputations, and genetic maps),
[qtl2scan](https://github.com/rqtl/qtl2scan) (for QTL genome scans and
related calculations), and
[qtl2plot](https://github.com/rqtl/qtl2plot) (for data visualization).
A further package, [qtl2convert](https://github.com/rqtl/qtl2convert),
contains functions for converting data among the R/qtl2,
[DOQTL](https://www.bioconductor.org/packages/release/bioc/html/DOQTL.html),
and [R/qtl](http://rqtl.org) formats, for example to convert genotype
probabilities produced by DOQTL to the format needed by qtl2scan, or
to convert qtl2scan results to the format produced by `scanone` in
R/qtl, so that they may be graphed with the R/qtl functions.

---

### Installation

R/qtl2 is early in development and so is not yet available on
[CRAN](http://cran.r-project.org).

You can install R/qtl2 from [GitHub](https://github.com/rqtl).

You first need to install the
[devtools](https://github.com/hadley/devtools) package, plus a set of
package dependencies: [yaml](https://cran.r-project.org/package=yaml),
[jsonlite](https://cran.r-project.org/package=jsonlite),
[data.table](https://cran.r-project.org/package=data.table),
and [RcppEigen](https://github.com/RcppCore/RcppEigen).
(Additional, secondary dependencies will also be installed)

    install.packages(c("devtools", "yaml", "jsonlite", "data.table", "RcppEigen"))

Then, install R/qtl2 using `devtools::install_github()`.

    library(devtools)
    install_github(paste0("rqtl/qtl2", c("geno", "scan", "plot", "convert")))

---

### Vignettes

- [user guide](http://kbroman.org/qtl2/assets/vignettes/user_guide.html)
- [input file formats](http://kbroman.org/qtl2/assets/vignettes/input_files.html)
  (see also the [sample data files](http://kbroman.org/qtl2/pages/sampledata.html))
- [developer guide](http://kbroman.org/qtl2/assets/vignettes/developer_guide.html)
- [HMM benchmarks](http://kbroman.org/qtl2/assets/vignettes/hmm_benchmarks.html)
- [linear regression benchmarks](http://kbroman.org/qtl2/assets/vignettes/linreg_benchmarks.html)

---

#### License

[Licensed](LICENSE) under [GPL-3](http://www.r-project.org/Licenses/GPL-3).
