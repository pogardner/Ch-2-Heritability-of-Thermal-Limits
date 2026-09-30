# Ch 2. Assessing the Heritability of Thermal Limits

The purpose of this repository is to share the code used to analyze the heritability of upper thermal limits of steelhead (*O. mykiss*). Here, we use genotypes derived from SNP and microhaplotype panels that are published in (insert publications) to build genetic relatedness matrices that are then used in an animal model.

We follow the below workflow:

1.  Assess relatedness of individuals in each population and ancestry using CKMRsim.
2.  Build genetic relatedness matrices:
    -   Apply a greedy algorithm to convert multi-allelic microhaplotype data into bi-allelic form
    -   Use AGHmatrix to build an A matrix and its inverse
3.  Apply the GRM to the animal model using brms and following the workflow specified by Wilson et al. 2010. (2012?)
    -   We test multiple model formats to select the best fit model.

This workflow corresponds to numbered Quarto notebooks.
