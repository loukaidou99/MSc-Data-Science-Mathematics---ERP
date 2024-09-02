This file lists the required R packages along with their versions and provides instructions on how to install them using RStudio.

## **Required R Packages**

**Package      Version**
- **readxl**        1.4.3
- **dplyr**         1.1.4
- **ggplot2**       3.5.1
- **lubridate**     1.9.3
- **tidyr**         1.3.1
- **imputeTS**      3.3
- **readr**         2.1.5
- **tidyverse**     2.0.0
- **reshape2**      1.4.4
- **sf**            1.0.16
- **leaflet**       2.2.2
- **RColorBrewer**  1.1.3
- **scales**        1.3.0
- **lattice**       0.22.6
- **rgl**           1.3.1
- **car**           3.1.2
- **broom**         1.0.6
- **caret**         6.0.94
- **MASS**          7.3.61
- **leaps**         3.2
- **gridExtra**     2.3
- **grid**          4.4.1
- **lme4**          1.1.35.5
- **Epi**           2.53
- **performance**   0.12.2
- **lmerTest**      3.1.3
- **buildmer**      2.11
- **nlme**          3.1.164
- **MuMIn**         1.48.4
- **merTools**      0.6.2
- **sp**            2.1.4
- **spacetime**     1.3.1
- **xts**           0.14.0
- **spatstat**      3.1.1
- **mgcv**          1.9.1
- **plotly**        4.10.4
- **akima**         0.6.3.4
- **reticulate**    1.38.0
- **gganimate**     1.0.9
- **animation**     2.7
- **viridis**       0.6.5

## **Instructions for Installing the Required Libraries**

To install the required R packages listed above while using RStudio, follow these steps:

1. **Open RStudio**.
2. **Copy and paste the following command into the R console to install all required packages**:

```{r}
# Function to install or update a package to a specific version
install_or_update <- function(package, version) {
  if (!requireNamespace(package, quietly = TRUE)) {
    # Install if not installed
    devtools::install_version(package, version = version)
  } else {
    # Check installed version
    installed_version <- packageVersion(package)
    if (installed_version != version) {
      # Update to the required version
      devtools::install_version(package, version = version)
    }
  }
}

# Install devtools if not already installed
if (!requireNamespace("devtools", quietly = TRUE)) {
  install.packages("devtools")
}

# List of packages and their required versions
packages <- c(
  "readxl" = "1.4.3",
  "dplyr" = "1.1.4",
  "ggplot2" = "3.5.1",
  "lubridate" = "1.9.3",
  "tidyr" = "1.3.1",
  "imputeTS" = "3.3",
  "readr" = "2.1.5",
  "tidyverse" = "2.0.0",
  "reshape2" = "1.4.4",
  "sf" = "1.0.16",
  "leaflet" = "2.2.2",
  "RColorBrewer" = "1.1.3",
  "scales" = "1.3.0",
  "lattice" = "0.22.6",
  "rgl" = "1.3.1",
  "car" = "3.1.2",
  "broom" = "1.0.6",
  "caret" = "6.0.94",
  "MASS" = "7.3.61",
  "leaps" = "3.2",
  "gridExtra" = "2.3",
  "grid" = "4.4.1",
  "lme4" = "1.1.35.5",
  "Epi" = "2.53",
  "performance" = "0.12.2",
  "lmerTest" = "3.1.3",
  "buildmer" = "2.11",
  "nlme" = "3.1.164",
  "MuMIn" = "1.48.4",
  "merTools" = "0.6.2",
  "sp" = "2.1.4",
  "spacetime" = "1.3.1",
  "xts" = "0.14.0",
  "spatstat" = "3.1.1",
  "mgcv" = "1.9.1",
  "plotly" = "4.10.4",
  "akima" = "0.6.3.4",
  "reticulate" = "1.38.0",
  "gganimate" = "1.0.9",
  "animation" = "2.7",
  "viridis" = "0.6.5"
)

# Install or update each package
lapply(names(packages), function(pkg) install_or_update(pkg, packages[pkg]))
```

3. **You can use the following R code to check the versions of the installed packages on your system**:
4. 
```{r}
# List of packages to check
packages <- c(
  "readxl", "dplyr", "ggplot2", "lubridate", "tidyr", "imputeTS", "readr", 
  "tidyverse", "reshape2", "sf", "leaflet", "RColorBrewer", "scales", 
  "lattice", "rgl", "car", "broom", "caret", "MASS", "leaps", "gridExtra", 
  "grid", "lme4", "Epi", "performance", "lmerTest", "buildmer", "nlme", 
  "MuMIn", "merTools", "sp", "spacetime", "xts", "spatstat", "mgcv", 
  "plotly", "akima", "reticulate", "gganimate", "animation", "viridis"
)

# Function to get the version of a package
get_package_version <- function(pkg) {
  if (requireNamespace(pkg, quietly = TRUE)) {
    return(as.character(packageVersion(pkg)))
  } else {
    return("Not Installed")
  }
}

# Get versions of all packages
package_versions <- sapply(packages, get_package_version)

# Combine package names and versions into a data frame
package_info <- data.frame(Package = packages, Version = package_versions, stringsAsFactors = FALSE)

# Print the package information
print(package_info)
```


