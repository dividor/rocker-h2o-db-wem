# rocker-h2o-db-wem

# Introduction

This Docker image extends rocker/tidyverse, in summary ...

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

# Caveats

The SQL Server ODBC 11 is a bit of a hack, but unfortunately the Microsoft latest releases don't seem to work
with the rocker version of Debian (somebody better than I can maybe fix this!)
