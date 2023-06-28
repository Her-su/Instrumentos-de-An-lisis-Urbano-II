# Instrumentos-de-An-lisis-Urbano-II
Clases escrito desde R _local_ 

# ctrl + shift + m = atajo de pipe %>% 

# alt + shift + K = shortcut menu 

# ctrl + enter = para correr los script (Run)

curso <- data.frame(nombre     = c("Juan", "Pedro", "María", "José","Enzo", "Ariel", "Eva"),
                    edad       = c(25, 32, 21,40, 30, 28, 37),
                    nacimiento = c(1993, 1986, 1997, 1978, 1988, 1990, 1981),
                    programa   = c("spss", "stata", "stata", "excel", "R", "stata", "spss"),
                    nivel      = c(3, 5,7, 6, 2, 6, 8))

# COn el comando de abajo veo en la consola donde esta el ancla               
getwd()

round(prop.table(table(curso$programa)) * 100, digits = 1)

#R base

mean(curso$edad)

library(tidyverse)

class(2)

class("2")



# Formato tidyverse

curso$edad %>% 
  mean() %>%
  round(digits = 1)

