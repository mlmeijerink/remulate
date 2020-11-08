# remulate (Version: 1.0.0)

### About the package
A package to generate Relational Event History Data

### Programming Languages
The package contains code written in:
* R (>= 4.0.0)
* Rcpp (>= 1.0.4.6) and RcppArmadillo (>= 0.9.860.2.0)
* C++11 (Compiler Version: GCC-8.1.0)
	
### Installing the package
To install the package in R using `devtools`:

```
library(devtools)
install_github("TilburgNetworkGroup/remulate")

# load the package
library(remulate)
```

### Example

```r
library(remulate)

form <- ~baseline(1)+ inertia(0.2,scaling="prop") + reciprocity(0.2,scaling="prop")
out <- remulateDyad(form,c(1:20),1000,memory="window",memory_param= 2)

```