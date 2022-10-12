# Wire

The **`Wire`** command makes a wire from A to B, connected to a specific connections.  

The syntax for the command is as follows
```
Wire [ConnectionID] [StartX] [StartY] [EndX] [EndY]
```

### **ConnectionID**

The ID given from a previous **`Connections`** command.

### **StartX** & **StartY** & **EndX** & **EndY**

Integer coordinates for the start and end points of a wire.  
Optionally a program may support a `Grid:Offset` coordinate system for finer positioning within a grid cell, the offset should be from 0 to 1 can be represented however the program wishes, as a fractional integer I.e. a format like 1.15 or 1.31 where there's 1 bit for the whole number and 15 or 31 bits for the fractional part.