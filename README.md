#D3.js FORCE DIRECTED GRAPH
#With a different way to format data

This is an experiment to find a different way to format the data used in a D3.js force directed graph. Instead of creating arrays of nodes and links, the parent nodes are created first and given a name. These names are used as the source for the child nodes. This means that you can create an array for the child nodes, where each entry in the array is an object containing the child data and the information about it parents.

```javascript
var nodeArray=[
    {"name":"And not for justice?",  "source":["APPLES", "GRAPES"]},
    {"name":"I know you all",  "source":["PLUMS"]},
    {"name":"Forever and a day",  "source":["PLUMS"]},
    {"name":"My library was dukedom <large enough",  "source":["APPLES"]},
    {"name":"Order gave each thing view",  "source":["ORANGES", "PLUMS"]},
    {"name":"Thou art the Mars of <malcontents",  "source":["ORANGES"]},
    {"name":"This blessed plot, this earth, <this realm, this England",  "source":["ORANGES"]},
    {"name":"Your wit’s too hot, it <speeds too fast",  "source":["PLUMS"]},
    {"name":"What a fool honesty is! ",  "source":["GRAPES", "PLUMS"]},
    {"name":"Harp not on that string",  "source":["GRAPES"]},
    {"name":"Boldness be my friend",  "source":["APPLES", "GRAPES"]},
    {"name":"To pluck bright honour from <the pale-faced moon",  "source":["ORANGES", "PLUMS"]},
];
```

```javascript
{"name":"And not for justice?",  "source":["APPLES", "GRAPES"]}
```

The child node And not for justice? is linked to two parent nodes, APPLES and GRAPES.