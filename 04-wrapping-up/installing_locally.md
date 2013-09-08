
# Rstudio server

The RStudio you used for the workshop today is available as a public Amazon Machine Image (AMI). The machine ID is:

```coffee
xxxxxxx
```

This means that you can use your own [personal Amazon account](https://console.aws.amazon.com/console/home) to launch an instance of this machine image at your convenience. We'll keep all the stable versions of rOpenSci packages and tools updated at all times. 

You will most likely just want to work locally on your copy of RStudio. In that case, you'll need the latest version of R (currently `3.0.1`) and [RStudio](http://www.rstudio.com/) for your platform. Then install the following packages:

```coffee
# First install the devtools package since it will allow you to install packges directly from GitHub that are currently not available on CRAN.

install.packages("devtools")
library(devtools)
```

Next install:

```coffee
install.packages("ggplot2", dependencies = TRUE)
install.packages("plyr")
install.packages("reshape2")
install.packages("knitr") # for reproducible documents
install.packages("gdata") # for reading excel files + other misc functions
install.packages("rgbif")
install.packages("rplos")
install.packages("rfisheries")
install.packages("rfigshare")

# from GitHub
install_github("rWBclimate",  "ropensci")
install_github("reml",  "ropensci")
```

*Note: REML currently has dependencies that are not on CRAN. See [this page]() for instructions on how to install them from source. Once a stable version is ready, all dependencies will also be available and setup will be a lot simpler.*


