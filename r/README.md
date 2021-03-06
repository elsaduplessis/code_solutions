R packages
---

Recommended lists:
* https://support.rstudio.com/hc/en-us/articles/201057987-Quick-list-of-useful-R-packages


Cheatsheets:
* https://github.com/rstudio/cheatsheets

---


**DATA CONNECTIONS**

RCurl
- https://crantastic.org/packages/RCurl
- download data from secure URL
    * https://www.earthdatascience.org/courses/earth-analytics/get-data-using-apis/access-gapminder-data-rcurl-r/


---



**READING**  

xlsx

sas7bdat
- SAS data

foreign  
- SAS data (.bdat)
- SPSS data (.sav)
    * SPSS date: as.Date(x/86400, origin = "1582-10-14")

memisc
- https://github.com/melff/memisc
- survey data
- import SPSS data
- as.data.set() 
    * e.g. *as.data.set(spss.system.file("..."))*

readr
- https://readr.tidyverse.org/
- tidyverse rectangular data import
    * https://rawgit.com/rstudio/cheatsheets/master/data-import.pdf

reticulate
- https://rstudio.github.io/reticulate/
- R interface to Python


---




**WRANGLING**  

**Tidyverse**  
* https://www.tidyverse.org/  
* https://github.com/tidymodels/tidymodels

dplyr
- https://dplyr.tidyverse.org/
- data transformation
    * https://github.com/rstudio/cheatsheets/blob/master/data-transformation.pdf

stringr 
- https://stringr.tidyverse.org/reference/index.html
- string handling
    * http://edrub.in/CheatSheets/cheatSheetStringr.pdf

tidyr
- https://tidyr.tidyverse.org/
- create tidy data (var = col, obs = row, val = cell)
    * gather(), spread()
    * separate(), separate_rows(), unite()
    * complete(), expand()
    * drop_na(), fill(), replace_na()
    * https://github.com/rstudio/cheatsheets/blob/master/data-import.pdf

broom
- https://broom.tidyverse.org/
- stat summaries of tidy data
    * interact with stat model objects
    * tidy(), glance(), augment()
    * https://github.com/tidymodels/broom

magrittr
- https://magrittr.tidyverse.org/
- le pipe %>%

purr
- https://purrr.tidyverse.org/
- functional programming
    * map(), pmap() [can use to apply row-wise funs]
    * https://github.com/rstudio/cheatsheets/blob/master/purrr.pdf

forcats
- https://forcats.tidyverse.org/
- factor handling


**Other**

data.table
- https://github.com/Rdatatable/data.table/wiki
- alternative to tidyverse
    * dependencies: base R


**Sensitive data**

encryptr
- https://github.com/SurgicalInformatics/encryptr
    * "Encrypt and decrypt data frame or tibble columns using the strong RSA public/private keys"
    * https://surgicalinformatics.org/ 

---



**METHODS**

**Data QC**  

janitor
- https://github.com/sfirke/janitor
- data cleaning
- examples
    * https://medium.com/@verajosemanuel/janitor-a-good-r-package-for-data-cleaning-f3c733632ad9


naniar  
- http://naniar.njtierney.com/articles/naniar-visualisation.html
- very useful missing data analysis / visualisation

**Extreme value analysis**

extReme
 - http://www.crm.umontreal.ca/2017/Extreme17/pdf/Gilleland_slides.pdf

**Multivariable analyis**

Nullabor

GGally
- ggpairs()

igraph
- create network objects

ggnet2
- use igraph network object as base layer for a ggplot

ggnetwork
- similar to ggnet2

ppcor  
- partial correlations

factoeextra
- https://www.rpackages.io/package/factoextra
- multivariate analysis
    * PCA, clustering

FactoMineR 


---




**VISUALISATION**  

ggplot2
- https://ggplot2.tidyverse.org/
- tidyverse plotting
    * https://github.com/rstudio/cheatsheets/blob/master/data-visualization-2.1.pdf

esquisse
- https://github.com/dreamRs/esquisse
- easy interactive GUI plotting for ggplot2

ggplotly
- https://plot.ly/ggplot2/
- Plotly for ggplot


grid

gridExtra
- plot to grids  
- grid.arrange()
- arrangeGrob()

cowplot
- also plotting to grids

Cairo
- Cairo graphics
- use with ggsave() to enable alpha transparency levels in .eps output


---



**PALETTES**
- https://github.com/EmilHvitfeldt/r-color-palettes
    * giant readme of palettes in R

viridis

wesanderson
- https://github.com/karthik/wesanderson
    * https://blog.revolutionanalytics.com/2014/03/give-your-r-charts-that-wes-anderson-style.html

gameofthrones
- https://github.com/aljrico/gameofthrones
    * "Lady Margaery"


---




**REPORTING**  

rmarkdown
- https://rmarkdown.rstudio.com/
- R Markdown reproducible reporting
    * https://www.rstudio.com/wp-content/uploads/2015/02/rmarkdown-cheatsheet.pdf

knitr
- inter-converts: Rmw - html - tex - pdf
- via R Markdown:
    * R block start: ```{R} 
    * end: ```
- via LaTeX: 
    * save LaTeX doc as .Rnw ("R no web")
    * R block start: << options >>= 
    * end: @ 

xtable
- includes LaTeX longtables  
- some issues with caption at top when not using longtable


---