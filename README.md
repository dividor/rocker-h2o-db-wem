# rocker-h2o-db-wemmodels

# Introduction

This Docker image extends the excellent [rocker tidyverse image](https://hub.docker.com/r/rocker/tidyverse/), in summary ...

- R 3.3.3
- Rocker RStudio
- Java 8
- rJava
- RODBC, RJDBC         
- DPAR 101                  
- SQL Server ODBC 11 
- word2vector
- text2vec                    
- H2O.AI                      
- ReporteRs                 
- ggplot2, plotly

# Commands

To start things up ...

``` docker run -v /data01/R:/localdir -d -p 8787:8787 ny/rocker ```

In the above /data01/R is where the code lives. Once running, use a web browser to access R studio.

Full instructions can be found on the [rocker rstudio wiki](https://github.com/rocker-org/rocker/wiki/Using-the-RStudio-image)


# Caveats

The SQL Server ODBC 11 is a bit of a hack, but unfortunately the Microsoft latest releases don't seem to work
with the rocker version of Debian (somebody better than I can maybe fix this!)

