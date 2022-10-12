# Custom

The **`Custom`** command group allows a program to implement their own sub commands.  
The purpose of this command group is to allow a program to implement editability in an optimal way for themselves, yes it means there might be competing methods for this, but since the command group takes in a unique identifier they can just use a shared identifier for said editability commands.  
A program should not execute the custom group if they don't support the unique identifier or the implemented version is below the required minimum version.  
This command group can appear multiple times within a component, which is useful to make programs mroe interchangeable, in the case of supporting multiple programs through adding more **`Custom`** command groups for them if needed.  
A program that wishes to edit a component through reading and writing a new one should retain all **`Custom`** command groups it doesn't recognize.  
For example if Component A was written for Program A with the unique identifier "**A**", then when imported into Program B the Custom group should be skipped quietly.

The syntax for the command is as follows
```
Custom [Name] [Version]
```

### **Name**

Something that can be uniquely identified for a program.

### **Version**

The minimum version required of the form `major` or `major.minor`, where `major` and `minor` are integers.