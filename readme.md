# Ways to define a variable in TS

| Define | Description |
|---|---|
| **var** | They have a function scope. They can be reassigned and redeclared in the same function. |
| **let** | They have a block scope. They can be reassigned, but not redeclared in the same block. |
| **const** | They also have a block scope. They cannot be reassigned or redeclared after their initialization. |

> **IMPORTANT**
> The use of **var** is not recommended

# Datatype 

## Primitive

- Boolean
- Number
- String

# Composite

- Array
- Tuple
- Enum
- Object
  
# Special

- Unknown
- Any
- Void
- Null and Undefined
- Never

# Examples - Boolean

> **IMPORTANT**
> It can only take 2 values **true** and **false**

```typescript
{
  (() => {
  
  let isDone: boolean = false;
  let isActive: boolean = false;
  let isValid: boolean = true;
  
  })();
}
```

