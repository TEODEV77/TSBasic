# Ways to define a variable in TS

| Define    | Description                                                                                       |
| --------- | ------------------------------------------------------------------------------------------------- |
| **var**   | They have a function scope. They can be reassigned and redeclared in the same function.           |
| **let**   | They have a block scope. They can be reassigned, but not redeclared in the same block.            |
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

  (() => {
  
  let isDone: boolean = false;
  let isActive: boolean = false;
  let isValid: boolean = true;
  
  })();

```
# Examples - Number

```typescript

  (() => {
  
  let price: number = 300;
  let stock: number = 50;
  let discount: number = 0.1;
  
  })();

```

# Examples - String

> **IMPORTANT**
> You can use **double quotes (")** or **single quotes (')**
> You can also use template strings **`My name is ${firstName}`**

```typescript

  (() => {
  
  let firstName: string;
  let lastName: string;
  let fulltName: string;
  let template: string = `My name is ${firstName}`;
  })();

```

# Examples - Array

```typescript

  (() => {
  
  let numbers: number[] = [1, 2, 3];
  let fruits: string [] = ["Apple", "Lemon", "Carrot"];
  let languages: string [] = ["Java","Python","C#"]
  
  })();

```

# Examples - Tuple

```typescript

  (() => {
  
  let tuple: [string, number];
  let tuple2: [string, boolean];
  let tuple3: [string, number, boolean];
  
  })();

```

# Examples - Enum

```typescript

(() => {
  
enum UserRole {
 Admin = "ADMIN",
 Editor = "EDITOR",
 Viewer = "VIEWER",

}
  
enum OrderStatus {
 Pending,
 Processing,
 Shipped,
 Delivered,
 Cancelled,  

}

  })();

```
> **IMPORTANT**
> OrderStatus.Pending **returns =>** 0
> OrderStatus.Cancelled **returns =>** 4

# Examples - Object

```typescript

  (() => {
  
  const currentUser: User = {
    id: 1,
    username: "usuario123",
    email: "usuario@example.com",
    isAdmin: false
  };
  
  })();

```


# Examples - Unknown

```typescript

  (() => {
  
  let userInput: unknown;
  let userData: unknown;
  
  })();

```

# Examples - Any

```typescript

  (() => {
  
  const mixedArray: any[] = [1, "Hi, There", true, { title: "Hello TypeScript" }];
  
  })();

```

# Examples - Void

> **IMPORTANT**
> **void** is a little like the opposite of **any:** the absence of having any type at all.
>  You may commonly see this as the return type of functions that do not return a value

```typescript

  (() => {
  
  function sayHi(name: string): void {

  console.log(`Hi, ${name}`);
  
  }
  
  })();

```

# Examples - Null and Undefined

> **IMPORTANT**
> **null** Used to indicate that a variable or property is present but does not have a meaningful value or is uninitialized
> **undefined** When a variable is declared but not given an initial value

# Examples - Never

> **IMPORTANT**
> The never type represents the type of values that never occur. 

```typescript

  (() => {
  
  // Function returning never must not have a reachable end point
  function error(message: string): never {
    throw new Error(message);
  }

  // Inferred return type is never
  function fail() {
    return error("Something failed");
  }

  // Function returning never must not have a reachable end point
  function infiniteLoop(): never {
    while (true) {}
  }
  
  })();

```






