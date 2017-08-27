Rprofile > set the Cran mirror

Renviron : http_proxy=http://proxy.mycompany.com

R STartup
https://www.r-bloggers.com/r-for-enterprise-understanding-rs-startup/

Rstudio
updated versions of the following
evaluate, digest, formatR, highr, markdown, stringr, yaml, Rcpp, htmltools, caTools, bitops, knitr, jsonlite, base64enc, rprojroot, rmarkdown


https://www.r-bloggers.com/installing-r-packages/

https://www.r-bloggers.com/list-of-user-installed-r-packages-and-their-versions/
ip <- as.data.frame(installed.packages()[,c(1,3:4)])
rownames(ip) <- NULL
ip <- ip[is.na(ip$Priority),1:2,drop=FALSE]
print(ip, row.names=FALSE)

https://stats.idre.ucla.edu/r/faq/how-can-i-manage-r-packages/


https://rstudio.github.io/packrat/walkthrough.html
https://www.r-bloggers.com/r-package-dependencies/

http://mazamascience.com/WorkingWithData/?p=728
R CMD Install

# this will prompt for a CRAN mirror
pack <- available.packages()
pack["ggplot2","Depends"]

https://stackoverflow.com/questions/14645363/listing-r-package-dependencies-without-installing-packages
https://www.r-bloggers.com/upgrading-r-and-packages/s

https://www.r-bloggers.com/install-all-required-r-packages-on-your-shiny-server/

https://www.r-bloggers.com/function-to-simplify-loading-and-installing-packages/



https://www.r-bloggers.com/permanently-setting-the-cran-repository/
local({
  r <- getOption("repos")
  r["CRAN"] <- "http://cran.cnr.berkeley.edu/"
  options(repos = r)
})



# Getting Help ! Section
R Online Documentation


--------------
R 3.2.5
--------------
base
boot
class
cluster
codetools
compiler
datasets
foreign
graphics
grDevices
grid
KernSmooth
lattice
MASS
Matrix
methods
mgcv
nlme
nnet
parallel
rpart
spatial
splines
stats
stats4
survival
tcltk
tools
translations
utils

