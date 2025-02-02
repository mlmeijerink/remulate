# remulate

remulate is a R library to generate dynamic temporal networks based on Relational Event Models.

### Programming Languages
The package contains code written in:
* R (>= 4.0.0)
* Rcpp (>= 1.0.4.6) and RcppArmadillo (>= 0.9.860.2.0)
* C++11 (Compiler Version: GCC-8.1.0)
	
## Installation

To install the package in R using `devtools`:

```R
library(devtools)
install_github("TilburgNetworkGroup/remulate")

#load the package
library(remulate)
```

## Usage
```R
effects <- ~ baseline(-4) + inertia(0.01) + reciprocity(-0.04) + itp(0.01,scaling="std")

remulateTie(effects, actors = 1:25, time = 20, events = 500, initial = 200)

```
## Support
```R
#To view all help files in the remulate package
help(package='remulate')

#To view available effects for remulateTie
help('remulateTieEffects')

#To view available effects for remulateActor
help('remulateActorEffects')

```
## Contributing
Pull requests and bug reports are welcome. For major changes, please open an issue first to discuss what you would like to change.
