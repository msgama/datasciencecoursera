# Open ".csv" files R
File is :  "hw1_data_2.csv"

> x <- read.csv (file = "hw1_data_2.csv", header = TRUE, sep = ",") 

##*file = the name of the file
##*header = if there is a name in each column you should "say" TRUE
##*sep = as "csv" file which are separated by a comman (,). if were space put " "

x[1]    # é para pedir a primeira linha toda ( do ínicio ao fim), um subgrupo
    Ozone
1      41
2      36
3      12

> ncol(x)
[1] 6
> nrow (x)
[1] 153

 x [1, ] # é para pedir a primeira linha e todas as colunas
  Ozone Solar.R Wind Temp Month Day
1    41     190  7.4   67     5   1

>  x [1:2, ] # é para pedir a primeira e a segunda linha e todas as colunas
  Ozone Solar.R Wind Temp Month Day
1    41     190  7.4   67     5   1
2    36     118  8.0   72     5   2

>  x [c(1,2), ]  # é para pedir a primeira e a segunda linha e todas as colunas
  Ozone Solar.R Wind Temp Month Day
1    41     190  7.4   67     5   1
2    36     118  8.0   72     5   2

>  x [c(152,153), ]  # é para pedir a última e a penultima linha e todas as colunas
    Ozone Solar.R Wind Temp Month Day
152    18     131  8.0   76     9  29
153    20     223 11.5   68     9  30

>  x [152:153, ]  # é para pedir a última e a penultima linha e todas as colunas
    Ozone Solar.R Wind Temp Month Day
152    18     131  8.0   76     9  29
153    20     223 11.5   68     9  30

> tail(x) # é para pedir as últimas linhas e todas as colunas
    Ozone Solar.R Wind Temp Month Day
148    14      20 16.6   63     9  25
149    30     193  6.9   70     9  26
150    NA     145 13.2   77     9  27
151    14     191 14.3   75     9  28
152    18     131  8.0   76     9  29
153    20     223 11.5   68     9  30

> head (x) # é para pedir as primeiras linhas e todas as colunas
  Ozone Solar.R Wind Temp Month Day
1    41     190  7.4   67     5   1
2    36     118  8.0   72     5   2
3    12     149 12.6   74     5   3
4    18     313 11.5   62     5   4
5    NA      NA 14.3   56     5   5
6    28      NA 14.9   66     5   6
