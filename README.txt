To recreate the examples from the tutorial,
open R and run the following commands at the R prompt.

==============================================
====   Tutorial Part I
==============================================

Load the functions for Example 1:
> source("ex1_beta.R")

Draw a random distribution using a beta random variable
with parameters (1,1).
Keep pressing enter to get more iid beta random variables.
Press "x" and then enter when you're done.
> ex1_draw_betas(1)
Choose a very small parameter tuple
> ex1_draw_betas(0.001)
Choose a very large parameter tuple
> ex1_draw_betas(1000)

Note: though we didn't cover it in the tutorial,
you can use the function "ex1_draw_betas_diffa"
to draw random distributions using both beta parameters.
e.g. > ex1_draw_betas_diffa(0.1,10)

Load the functions for Example 2.
Note: you may need to install the MCMCpack package first: > install.packages("MCMCpack")
> source("ex2_diri.R")

Draw a random distribution using a Dirichlet random variable
with all parameters 1.
Keep pressing enter to get more iid Dirichlet random variables.
Press "x" and then enter when you're done.
> ex2_draw_diris(K=4,a_scalar=1)
Choose a very small shared parameter
> ex2_draw_diris(K=4,a_scalar=0.001)
Choose a very large shared parameter
> ex2_draw_diris(K=4,a_scalar=1000)

Note: though we didn't cover it in the tutorial,
you can use the function "ex2_draw_diris_diffa"
to draw random distributions using different Dirichlet parameters.
e.g. > ex2_draw_diris_diffa(c(1,3,5,2))

Load Example 3
Draw a Dirichlet distribution with large K.
> source("ex3_largeK_distr.R")
Press enter to keep making draws from the random distribution.
Press "x" and then enter when you're done.

Note: in the tutorial we tried out different values
of a. (For K=1000, we tried a=0.001,0.01,1,10.)
Although we didn't cover it in the tutorial,
you can use the function "ex3_gen_largeK_diri"
to also try out different values of K.
E.g. > ex3_gen_largeK_diri(K=1000,a=0.01)

Load Example 4
Look at the cluster assignments according to a Dirichlet distribution with large K.
> source("ex4_largeK_count.R")
Press enter to keep making draws from the random distribution.
Press "x" and then enter when you're done.

Note: though we didn't cover it in the tutorial,
you can use the function "ex4_gen_largeK_count"
to draw cluster assignments with different values of K and a.
E.g. > ex4_gen_largeK_count(K=1000,a=0.01)
