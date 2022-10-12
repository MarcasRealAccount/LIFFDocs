# Body

The body is comprised of a `\r\n`/`\n` newline separated list of commands.  
The optimal layout of a body is
```
TruthTable

Graph
// Graph commands

GraphRender
// Graph render commands

Script

Custom
// Custom commands
```

As the above layout makes it quickly readable of what the component supports, whether it is a TruthTable only component or if it has a Graph associated with it for simulating the internals, or if it is a script component.