# GraphViz

---

**A simple yet practical graph visualization tool.**


---

## Graph Format

Please format your graph data according to the following specifications before you throw it into the tool:

### Single Graph Format(For normal graph)
```json

{
    "gid": Graph_ID,
    "gname": Graph_Name,
    "directed": true|false,
    "typed": true|false,
    "nodes": [{
        "nid": Node_ID,
        "type": Node_Type,
        "name": Node_Name
    }],
    "edges": [{
        "eid": Edge_ID,
        "source": Source_Node_ID,
        "target": Target_Node,
        "type": Node_Type,
        "name": Node_Name
    }]
}

```
### Merged Graph Format(For merged graph)
```json
{
    "mid": Merged_Graph_ID,
    "clusters": [{
        "cid": Cluster_ID,
        "size": Cluster_Size,
        "nodes": [{
            "gid": Original_Graph_ID,
            "nid": Original_Node_ID,
            "size": Node_Size
     }],
    "links": [{
        "lid": Link_ID,
        "source": Source_Cluster_ID,
        "target": Target_Cluster_ID,
        "label": Link_Label
    }]
}

```


See examples in /data.


## Usage


Throw your json graph data into the html page in /release, your graph should be visualized like this:


### Single Graph Format(For normal graph)

![single_graph](https://github.com/Symbolk/GraphViz/blob/master/screenshots/single_graph.jpg)

### Merged Graph Format(For merged graph)
![merged_graph](https://github.com/Symbolk/GraphViz/blob/master/screenshots/merged_graph.jpg)

