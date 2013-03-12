RSofia-Sparse -- a fork of a port

This is a fork of the open source library RSofia: http://cran.r-project.org/web/packages/RSofia/
Which in turn is a port of the wonderful sophia-ml library: http://code.google.com/p/sofia-ml/

This version has limited sparse matrix support. The wonderful sophia-ml library utilizes the libsvm data format. RSofia only accepts dataframes to encode the explanitary variables. While great for smaller problems this approaches loses the main benefit of the libsvm format and limits the size of problems that can be tackled in-memory
 
After I get this code working I hope to merge with the RSophia package or Release a free standing version. Until then use devtools:

    install.packages("devtools")
    library(devtools)
    dev_mode(on=T)
    install_github("RSofia-Sparse", username = "jofusa")


John Dennison - March 2013



R Port by: Michael King and Fernando Cela Diaz. 
Original sofia-ml code by D. Sculley.

Supported learners include:

    * Pegasos SVM
    * Stochastic Gradient Descent (SGD) SVM
    * Passive-Aggressive Perceptron
    * Perceptron with Margins
    * ROMMA 

