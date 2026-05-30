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


Installation steps 
https://www.oracle.com/java/technologies/downloads/#jdk26-mac

download the stable JDK version depending on the system you are using. I am using Mac M3 chip laptop, so i downloaded it from 
https://download.oracle.com/java/26/latest/jdk-26_macos-aarch64_bin.dmg

Once installed, check the java version and javac (java compiler) version by using below command

java --version
javac --version 

As a React developer, you might be wondering: "Wait, why are there two different commands? java -version and javac --version?"

This is actually a fundamental concept in how Java works, and it's quite different from how JavaScript runs in the browser or Node.js.

The Two-Step Dance: javac vs java
In JavaScript, your code is read and executed line-by-line at runtime by an engine (like V8 in Chrome or Node). Java doesn't do that. It uses a two-step compilation and execution process.

1. javac (The Java Compiler)
What it is: This is the tool you just tested. It takes your human-readable source code (your .java files) and compiles it into something called Bytecode (which creates .class files).

The React Analogy: Think of javac like Babel or the TypeScript compiler (tsc). It checks your code for syntax and type errors and builds it into a format that the computer can actually use. If you make a typo or mismatch a type, javac will scream at you right here and refuse to build the app.

2. java (The Java Virtual Machine / JVM)
What it is: This is the execution engine. It takes that compiled Bytecode (.class file) and translates it into machine code that your M3 Mac's processor understands, running your application.

The React Analogy: Think of the java command like running node dist/index.js or loading your bundled code into a browser engine.

<img width="731" height="465" alt="Screenshot 2026-05-29 at 7 49 44 AM" src="https://github.com/user-attachments/assets/e595db6e-5429-48d9-9eee-c078d806caf9" />


🛠️ Understanding What You Just Checked
In JavaScript, Node just runs your code. Java uses a two-step process, which is why you checked two different commands:

javac (The Compiler): This takes your human-readable .java file and compiles it into .class files containing "Bytecode".

java (The JVM): This is the execution engine. It takes that Bytecode and runs it on your Mac.

