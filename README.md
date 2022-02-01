# Genetic_Algorithm

## Functions
- selbest
- selrand
- crossov
- muta
- mutx
- genpop

### selbest
The function copies from the old population into the new population
required a number of strings according to their fitness. The number of the
selected strings depends on the vector Nums as follows:
Nums=[number of copies of the best string, ... ,number of copies of the i-th best string, ...]
The best string is the string with the lowest value of its objective


### selrand
The function selects randomly from the old population a required number
of strings.


### crossov
The function creates a new population of strings, which rises after
1- to 4-point crossover operation of all (couples of) strings of the old
population. The selection of strings into couples is either random or
the neighbouring strings are selected, depending on the parameter sel.

### muta
The function mutates the population of strings with the intensity
proportional to the parameter rate from interval <0;1>. Only a few genes  
from a few strings are mutated in the population. The mutations are realized
by addition or substraction of random real-numbers to the mutated genes. The 
absolute values of the added constants are limited by the vector Amp. 
Next the mutated strings are limited using boundaries defined in 
a two-row matrix Space. The first row of the matrix represents the lower 
boundaries and the second row represents the upper boundaries of corresponding 
genes.

### mutx
The function mutates the population of strings with the intensity
proportional to the parameter rate from interval <0;1>. Only a few genes  
from a few strings are mutated in the population. The mutated values are
selected from the bounded real-number space, which is defined by the two-row 
matrix Space. The first row of the matrix represents the lower boundaries and the 
second row represents the upper boundaries of corresponding genes in the strings. 

### genpop
The function generates a population of random real-coded strings
which items (genes) are limited by a two-row matrix Space. The first
row of the matrix Space consists of the lower limits and the second row 
consists of the upper limits of the possible values of genes. 
%The length of the string is equal to the length of rows of the matrix Space.
