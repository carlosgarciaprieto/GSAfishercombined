# GSAfisherCombined
## Definition 
Provides the p-value for a joint test of association between a phenotype and a set of genetic variants (SNPs) by combining marginal p-values using the Fisher method. See Fisher, R.A. (1925) Statistical Methods for Research Workers.
## Installation
### From GitHub
```R
library(devtools)
install_github("carlosgarciaprieto/GSAfisherCombined")
```
## GSAfisher.default
### Description
Default method of GSAfisher function that computes the p-value for a joint test of association between a phenotype and a set of genetic variants (SNPs) by combining marginal p-values using the Fisher method.
### Usage
```R
## Default S3 method:
GSAfisher(x,...)
```
### Arguments
```R
x = Numeric set of marginal p-values (one vector or a sinlge p-value).
... = Further arguments passed to or from other methods.
```
### Value
```R
p = Fisher method combined p-value.
```
## Example
```R
#Generate 1000 random values from an Uniform distribution U (0, 0.25). 
x<-runif(1000, 0, 0.25)
#Apply the GSAfisher.default function to this data vector.
GSAfisher(x)
```
