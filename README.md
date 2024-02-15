# LMEM-Sim Generator
This project aims to simplify the generation of simulations to test the sample size needed to achieve a desired statistical power using linear mixed models, as presented by DeBruine and Barr (2021). For a detailed explanation of the simulations, please read the [original article](https://journals.sagepub.com/doi/full/10.1177/2515245920965119). You can also access the examples provided by the authors at [https://osf.io/3cz2e/](https://osf.io/3cz2e/).

Using this project you will be able to generate the R code needed to do basic simulations without having to program yourself, just by inputting the desired parameters in the form or by uploading them in JSON format. Once you have written the parameters in the form, you can also download them in JSON format, to be able to reuse them later.

However, notice that this project only generates the code for the most basic designs (specifically, those similar to the example 1a and the 2ww2wb design of example 2 presented by DeBruine and Barr), but cannot generate the complete code for more complex designs (like the 2ww2ww design with counterbalancing of example 2). In these cases, you can use the generated code as a base and modify it according to your needs. In all cases, you should carefully read the code to ensure that it is working as you expect, so knowledge of R is highly recommended.

Another limitation of the project is that it uses the letter 'x' as the internal symbol for interactions, so you should not name any variable as only 'x' (names like 'x1' are OK, but not the character 'x' alone). You should not use special characters (such as tildes, asterisks, plus or minus signs, etc.) in variable names, since they will be used as R variable names. Valid characters for R variable names are numbers (as long as their not in the first position), letters a to z in lower or upper case, underscores and dots.

To use this project [click here](https://hernanqs.github.io/lmem-sim-gen/lmem-sim-gen.html).

## References
DeBruine, L. M., & Barr, D. J. (2021). Understanding mixed-effects models through data simulation. Advances in Methods and Practices in Psychological Science, 4(1), 2515245920965119.