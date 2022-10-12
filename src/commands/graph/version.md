# Version

The **`Version`** command specifies what minimum version of LIFF the component was written for.  
This ensures the component doesn't crash older programs in the case of using a future builtin component.  
The program should tell the user the component is incompatible with the current version.

The syntax for the command is as follows
```
Version [VersionRequirement]
```

### **VersionRequirement**

A version number in one of the formats: `major`, `major.minor`, where `major` and `minor` are integers.