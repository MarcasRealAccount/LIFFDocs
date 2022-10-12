# GraphRender

The **`GraphRender`** command group expresses the rendering of a graph for a component.  
This command requires a previous **`Graph`** command group.  
This command and its sub commands can be skipped if the program only simulates without visuals, the program shall quietly skip them as if they never existed.  
This command doesn't help implement editability for a program, covered [here](./custom.md).

The sub commands you can use within a **`GraphRender`** is:
- [Position](./graphrender/position.md)
- [Wire](./graphrender/wire.md)