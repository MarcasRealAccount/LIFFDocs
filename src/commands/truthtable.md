# TruthTable

The **`TruthTable`** command expresses a truth table for the component.  
This command is only legal for components with \\(\le 16\\) inputs, as more would require substantually larger truth tables. (*Subject to be increased later*)  
The following sequence of bits `0`s and `1`s as ascii characters represents the outputs, the command should continue reading new lines until it either has read all the bits it needs (`(1 << input_count) * output_count`) or reaches another command, at which point it should error and explain to the user the truth table is written improperly, and telling them how many bits was found out of how many should be there.  
The bits can be indexed like `inputs * output_count` which specifies the bit index, where `inputs` is an integer with the input bits set correctly.  
So for a component with 3 inputs and 5 outputs the total bit count would be `(1 << 3) * 5 => 40` and could look like:
```
TruthTable
00000 // 000
01010 // 001
01001 // 010
11010 // 011
10110 // 100
11110 // 101
11101 // 110
11111 // 111
```

Or all on one line:
```
TruthTable 0000001010010011101010110111101110111111
```