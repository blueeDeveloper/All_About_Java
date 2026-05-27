Java forces everything inside a class, we have to look at the core philosophy of how Java was designed

When Java was created in the 1990s, the software industry was facing a massive crisis: codebases were becoming too large, messy, and incredibly difficult to maintain. The solution at the time was Object-Oriented Programming (OOP), and Java’s creators decided to go "all in" on it.

Here is the breakdown of why Java forces this structure, and how it compares to what you know in React.

1. The Core Philosophy: The World is Made of "Things"
In JavaScript and React, the core philosophy is often functional: "Give me data, and I will transform it using functions." In Java, the philosophy is structural: "The world is made of objects (nouns), and those objects have characteristics (fields) and behaviors (methods)." Because Java insists that you model the real world this way, a function cannot just float around in space. It must belong to an object or a concept.

In JavaScript: You can just write function calculateTax(price) { ... } anywhere.

In Java: You have to ask, "Who is responsible for calculating tax?" The answer is a TaxCalculator class.

2. Predictability and Memory Management
Java was designed to be highly secure and predictable. By forcing everything into a class, the Java Virtual Machine (JVM) knows exactly how to compile, load, and manage the memory of your application from the moment it starts.

When everything is wrapped in a class, the compiler can strictly enforce rules about who is allowed to see or change certain data (using keywords like public, private, and protected). In JavaScript, keeping variables truly private used to require complex closures; in Java, it’s built into the very nature of the class.

3. How to Do "Just Functions" in Java (The React Mental Model)
As a React developer, you might wonder: "What if I just want a simple utility function, like formatting a date? Do I really need to instantiate a whole object just to use it?"

No, you don't! Java handles this using the static keyword.

When you make a method static, it means it belongs to the class itself, not to an instance of the class. This is the closest Java gets to a standalone JavaScript function.


we have a technology called JVM (Java Virtual Machine)
