# GraphMerging
====

### Based on [multiMAGNA++](http://www3.nd.edu/~cone/multiMAGNA++/ "悬停显示")
----

### Input Format: 

[LEDA](http://www.algorithmic-solutions.info/leda_guide/graphs/leda_native_graph_fileformat.html)

LEDA.GRAPH
void
void
-2
3
|{A}|
|{B}|
|{C}|
3
1 2 0 |{}|
1 3 0 |{}|

### Shell Options:

> -G [file containing list of networks to align]
> -o [output file prefix]
> -m [optimizing measure]
> -d [file containing list of node similarity files]
> -a [alpha value]
> -p [population size]
> -e [elite percentage]
> -n [number of generations]
> -f [frequency of output]
> -t [number of threads]

Check README.txt for details.

### Sample Usage:

```sh
./magna -G test_graphs.txt -o test_run -m CIQ -p 10 -n 100 -f 2 -t 64
./magna -G test_graphs.txt -o test_run -m CIQ -d test_graphs_sim.txt -p 10 -n 100 -f 2 -a 0.6
```

> With some modifications on :

* `initialization`
* `crossover function`
* `fitness function`

### References:
[multiMAGNA++]:http://www3.nd.edu/~cone/multiMAGNA++/

