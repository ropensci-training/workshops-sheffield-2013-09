## rvertnet use case - Plot species occurrence data

### Load libraries


```coffee
library(rvertnet)
library(ggplot2)
```


### Define a species list


```coffee
splist <- splist <- c("Accipiter erythronemius", "Junco hyemalis", "Aix sponsa", 
    "Haliaeetus leucocephalus", "Corvus corone", "Threskiornis molucca", "Merops malimbicus")
```


### Search for occurrences in VertNet


```coffee
out <- lapply(splist, function(x) vertoccurrence(t = x, grp = "bird", num = 500))
```


### Plot data


```coffee
vertmap(out)
```

```
## Rendering map...plotting 2265 points
```

```
## Warning: Removed 1790 rows containing missing values (geom_point).
```

![plot of chunk splist3](figure/splist3.png) 

