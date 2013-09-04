
# Rstudio server

The RStudio you used for the workshop today is available as a public Amazon Machine Image (AMI). This means that you can use your own [personal Amazon account](https://console.aws.amazon.com/console/home) to launch a copy at any time of your choosing. We'll keep all the packages and tools updated. However, you might also want a local copy for your use.

In that case, you'll need the latest version of R (currently `3.0.1`) and [RStudio](http://www.rstudio.com/) for your platform. Then install the following packages:

```coffee
# First install the devtools package since it will allow you to install packges directly from GitHub that are currently not available on CRAN.

install.packages("devtools")
library(devtools)
```

Next install:

```coffee
install.packages("rgbif")
install.packages("rplos")
install.packages("rfisheries")
install.packages("rfigshare")

# from GitHub
install_github("rWBclimate",  "ropensci")
```
