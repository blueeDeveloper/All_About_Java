🧠 5. Memory Architecture: The Stack vs. The Heap
To understand variables in Java, you must understand how the JVM splits its runtime memory allocation:

1. Stack Memory (Primitives Live Here)
The Stack is a fast, immediate-access memory structure managed directly by the CPU. When you declare a primitive type variable, 
the actual raw value is stored directly inside that variable's allocated slot on the Stack.

2. Heap Memory (Objects Live Here)
The Heap is a large pool of memory used for dynamic allocations. When you declare a Non-Primitive/Reference type (like a String, 
an Array, or a Custom Class), the variable on the Stack does not contain the actual data. Instead, it contains a memory address 
pointer pointing to the object's physical location on the Heap.


🛡️ 6. The 8 Primitive Data TypesPrimitive types are the most basic data types built directly into the Java language. 
They are identified by reserved keywords (all lowercase) and represent raw binary values stored directly on the Stack.


<img width="727" height="544" alt="Screenshot 2026-05-29 at 3 44 00 PM" src="https://github.com/user-attachments/assets/fe2ec118-e538-4469-b88b-1b657d132302" />

<img width="806" height="671" alt="Screenshot 2026-05-29 at 3 44 08 PM" src="https://github.com/user-attachments/assets/3bc230a9-c622-4a1a-9a49-0261cf2b6a2f" />


<img width="748" height="354" alt="Screenshot 2026-05-29 at 3 44 15 PM" src="https://github.com/user-attachments/assets/1f752a17-5b24-469f-b34a-c80aa090a9c8" />

🔄 Core Syntactic Adjustments: JavaScript vs. Java
As a developer transitioning from JavaScript/TypeScript, keep these vital behavioral adjustments in mind:

1. No Loose Type Coercion
JavaScript dynamically evaluates expressions across types (e.g., 4 + "4" = "44"). Java throws compilation errors for invalid type combinations
before bytecode can ever be generated.

2. Variable Scope Keywords
Java does not feature let or const. Instead, type safety handles standard parameters. To lock a primitive variable down as an immutable constant, 
prepend the final keyword:

```
// JavaScript constant
const MAX_CONNECTIONS = 100;

// Java constant
final int MAX_CONNECTIONS = 100;
```

3. Numeric Literals and Readability
For highly granular numeric assignments, Java allows you to place underscores (_) inside numeric literals to act as visual separators. 
The compiler entirely strips these out during parsing:

```
int creditCardNumber = 4111_2222_3333_4444;
```



