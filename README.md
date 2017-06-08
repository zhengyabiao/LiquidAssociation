# LiquidAssociation

 the source code of 'Genome-wide trait-trait dynamics interaction study dissects the gene regulation pattern in maize kernels'

## liquid association

The LA theory is presented in terms of continuous random variables (Li et al, 2002, PNAS). Li proposed the concept of LA to describe how the coexpression pattern of two genes, X and Y, changes according to the level of a third gene, Z.

 - LA(X,Y|Z)=E(XYZ)

for large matrix gene expression data X, we can use matrix cross-product to accelerate, which much faster than sum(x*y*z)/N.
the detail code is in 02_genome-LA.R.

## exp_qqnorm.7z
the qqnormed gene expression data. 

## 01_permutation.R
generate a reference distribution of LA scores using a simulation scheme

## 02_genome-LA.R
compute a genome wide LA scores. every triplet gene expression combinations. 

## write_LA.cpp
the Rcpp function to accelerate output LA result.






