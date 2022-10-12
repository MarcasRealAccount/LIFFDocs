# Header

The header is the only fully required part of a LIFF file.

```
[NamespaceID]
[InputNames]
[OutputNames]
```

### **NamespaceID**

An identifier of the form `Namespace:Name` where `Namespace` and `Name` are text.
The allowed characters in the sequences are as follows:
- `0123456789` numbers
- `abcdefghijklmnopqrstuvxyz` lowercase letters
- `_`
- `-`
- `.`

### **InputNames** & **OutputNames**

A semicolon separated list of input and output names, these define how many inputs and outputs a component has.