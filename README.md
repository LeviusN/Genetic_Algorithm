# Genetic_Algorithm

## Function
- selbest
- selrand
- crossov
- muta

### selbest
The function copies from the old population into the new population
required a number of strings according to their fitness. The number of the
selected strings depends on the vector Nums as follows:
Nums=[number of copies of the best string, ... ,
            number of copies of the i-th best string, ...]
The best string is the string with the lowest value of its objective


## selrand
The function selects randomly from the old population a required number
of strings.


### crossov
The function creates a new population of strings, which rises after
1- to 4-point crossover operation of all (couples of) strings of the old
population. The selection of strings into couples is either random or
the neighbouring strings are selected, depending on the parameter sel.
