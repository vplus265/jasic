# About

**Jasic** is an exercise in simplicity and pedagogy. It is a complete standalone interpreter for a dialect of the original BASIC language, all packed into a single `.java` file. Jasic handles:

- Tokenizing
- Parsing
- Interpreting
- Output
- Variables
- Expressions
- Flow control

Essentially, it operates like a full-scale compiler or interpreter but on a miniature scale. The code is designed to be simple and readable while maintaining a certain terseness.

If you've ever wanted a gentle introduction to how programming languages work under the hood, **Jasic** is a great place to start.

---

## Getting Started

You can build Jasic using your preferred IDE, but the simplest way is via the command line. Follow these steps:

1. Open a terminal or command prompt.
2. Navigate to the main Jasic directory (where this file is located).
3. Compile the code with:

```bash
  javac com/stuffwithstuff/Jasic.java
```

4. Run the interpreter with:

```bash
java com.stuffwithstuff.Jasic <script>
```

Replace <script> with the path to a .jas file containing Jasic code. For example:

```bash
  java com.stuffwithstuff.Jasic sample / mandel.jas ``
```

---

## Hello World! 
```BASIC
' It doesn't get much simpler than this!
print "Hello, world!"
```

---

## More Info

For more details about Jasic, including its syntax and how the interpreter works, explore the source code in Jasic.java. It's all there.

If you have questions, feel free to reach out. Cheers!