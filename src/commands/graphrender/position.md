# Position

The **`Position`** command sets the position of a node.  

The syntax for the command is as follows
```
Position [Name] [GridX] [GridY]
```

### **Name**

A text field for a name, should follow normal C/C++ identifiers. In other words should only allow alphabetic or underscore followed by alphanumerics or underscores.  
The reason behind this is so that numbers and identifiers don't get mixed.  
In terms of Regex `[A-Za-z_][A-Za-z0-9_]*`.

### **GridX** & **GridY**

Integer coordinates for the top left corner of the node.  
Optionally a program may support a `Grid:Offset` coordinate system for finer positioning within a grid cell, the offset should be from 0 to 1 can be represented however the program wishes, as a fractional integer I.e. a format like 1.15 or 1.31 where there's 1 bit for the whole number and 15 or 31 bits for the fractional part.