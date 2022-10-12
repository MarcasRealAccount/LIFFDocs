# Depend

The **`Depend`** command specifies what other components must exist before using this one.  
This ensures the component doesn't crash programs where it requires a missing component.  
The program should tell the user the component is missing the components.

The syntax for the command is as follows
```
Depend [NamespaceID(;InputCount) ...]
```
Space separated list of component ids comprised of the namespace id and an optional input count preceeded by `;`.

### **(;InputCount)**

An optional input count, useful for having components with multiple input counts.  
If this field is omitted the program should try to figure out which component overload to use, based on the used ports. (*The program may skip over this, and instead scream at the user about this feature not being implemented under the message "NO_OVERLOAD_RESOLUTION"*)