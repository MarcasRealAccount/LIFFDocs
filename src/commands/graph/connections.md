# Connections

The **`Connections`** command adds connections to a graph.  
Used to connect two or more nodes together.  
Each call to this command makes a new **ConnectionID** for it, by incrementing each time. So having 2, the first one has the ID of 0, the second one has the ID of 1.

The syntax for the command is as follows
```
Connections [[Name](:PortName) ...]
```
Space separated list of node names with an optional port name or number preceeded by `:`.  

### **Name**

A text field for a name, should follow normal C/C++ identifiers. In other words should only allow alphabetic or underscore followed by alphanumerics or underscores.  
The reason behind this is so that numbers and identifiers don't get mixed.  
In terms of Regex `[A-Za-z_][A-Za-z0-9_]*`.

### **(:PortName)**

An optional port name, specifies what port to connect.  
This can be either the name given in the header of the component or a number.  
The number represents an input if it is \\(\le\\) inputCount, otherwise it represents an output.