# Node

The **`Node`** command adds a node to the graph under a specific name.

The syntax for the command is as follows
```
Node [NamespaceID(;InputCount)] [Name]
```

### **(;InputCount)**

An optional input count, useful for having components with multiple input counts.  
If this field is omitted the program should try to figure out which component overload to use, based on the used ports. (*The program may skip over this, and instead scream at the user about this feature not being implemented under the message "NO_OVERLOAD_RESOLUTION"*)

### **Name**

A text field for a name, should follow normal C/C++ identifiers. In other words should only allow alphabetic or underscore followed by alphanumerics or underscores.  
The reason behind this is so that numbers and identifiers don't get mixed.  
In terms of Regex `[A-Za-z_][A-Za-z0-9_]*`.