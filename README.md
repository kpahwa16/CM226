# CM226

Multiple methods have been developed to calculate heritability using single nucleotide polymorphisms (SNPs). We divide this project into two parts: in the first part, based on genotype-phenotype data for continuous phenotypes, we calculate heritability of simulated traits using linear regression, LASSO regression, ridge regression, and polygenic risk scores. Subsequently, we use simulated case-control data to directly asses disease risk using classification techniques: random forests, logistic regression and XGBoost. We perform a comparative analysis on these approaches to understand the which performs better. Phenotypic predictions in human datasets have been modeled using regression models with a few single nucleotide polymorphisms (SNPs) having strong association identified by GWAS.

We utilize genotype data from European individuals from the 1000 genomes project. The data is available at https:// drive.google.com/file/d/1IqRqXFbpQBxinmCcBOQVk_7tUCJbzp5B/view?usp=drive_web. The following is a description of the data used.

Genotype Data
The chromosome 22 imputed data was filtered for MAF > 0.05, HWE p-value > 0.000005, only keeping variation that had a PASS filter and for only containging SNPs. The bim file contains information about the SNPs in your data, the fam file about the individuals and the bed file the plink-readable genotype matrix.

Phenotype Data
The data provided was simulated using two models: the infinitesimal model (all causal) that assumes every SNP affects the trait, and Non-infinitesimal (OnePercCausal) where some SNPs have no effect on the trait; we assume that one percent of SNPs have a non-zero effect. ’hsq’ refers to the proportion of the variance in the simulated trait that is due to genetics. Simulations use hsq values of 0.2, 0.4, and 0.8. We consider two kinds of phenotypes: case-control and continuous. Height is an example of a continous trait while has diabetes vs doesn’t have diabetes is an example of a Case-Control trait.

Report Link : https://drive.google.com/file/d/1IGqHCz_TZ8b7mus9Uc_SWIrPCBkkcgkX/view?usp=sharing

Presentation : https://drive.google.com/file/d/1qT1CVfK6ksg4z35txgslS8JanfCC5Yem/view?usp=sharing

