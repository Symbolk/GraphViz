Graph Viz
====

### A simple graph visualization tool in Javascript(http://www.liaoxuefeng.com/wiki/001434446689867b27157e896e74d51a89c25cc8b43bdb3000 "悬停显示")
----

### Graph Format(*.json): 
{
        "gid": 0,
        "gname": "society",
        "directed": true,
        "typed": false,
        "nodes": [{
            "nid": 0,
            "type": "Boy",
            "name": "John"
        }


### Shell Options:


> -t [number of threads]

Check README.txt for details.

### Sample Usage:

```Bash
./magna -G test_graphs.txt -o test_run -m CIQ -p 10 -n 100 -f 2 -t 64
./magna -G test_graphs.txt -o test_run -m CIQ -d test_graphs_sim.txt -p 10 -n 100 -f 2 -a 0.6
```

> With some modifications on :

* `initialization`
* `crossover function`
* `fitness function`

### References:
[1]multiMAGNA++:http://www3.nd.edu/~cone/multiMAGNA++/

[2]LEDA:http://www.algorithmic-solutions.info/leda_guide/graphs/leda_native_graph_fileformat.html
