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
print "Hello, world!\n"
print "I am Jasic!" 
```

---

## Jasic Syntax 
```
 * Comments start with ' and proceed to the end of the line:
 * 
 *     print "hi there" ' this is a comment
 * 
 * Numbers and strings are supported. Strings should be in "double quotes", and
 * only positive integers can be parsed (though numbers are double internally).
 * 
 * Variables are identified by name which must start with a letter and can
 * contain letters or numbers. Case is significant for names and keywords.
 * 
 * Each statement is on its own line. Optionally, a line may have a label before
 * the statement. A label is a name that ends with a colon:
 * 
 *     foo:
 * 
 * 
 * The following statements are supported:
 * 
 * <name> = <expression>
 *     Evaluates the expression and assigns the result to the given named 
 *     variable. All variables are globally scoped.
 *     
 *     pi = (314159 / 10000)
 *     
 * print <expression>
 *     Evaluates the expression and prints the result.
 * 
 *     print "hello, " + "world"
 * 
 * input <name>
 *     Reads in a line of input from the user and stores it in the variable with
 *     the given name.
 *     
 *     input guess
 *     
 * goto <label>
 *     Jumps to the statement after the label with the given name.
 * 
 *     goto loop
 * 
 * if <expression> then <label>
 *     Evaluates the expression. If it evaluates to a non-zero number, then
 *     jumps to the statement after the given label.
 * 
 *     if a < b then dosomething
 * 
 * 
 * The following expressions are supported:
 * 
 * <expression> = <expression>
 *     Evaluates to 1 if the two expressions are equal, 0 otherwise.
 * 
 * <expression> + <expression>
 *     If the left-hand expression is a number, then adds the two expressions,
 *     otherwise concatenates the two strings.
 * 
 * <expression> - <expression>
 * <expression> * <expression>
 * <expression> / <expression>
 * <expression> < <expression>
 * <expression> > <expression>
 *     You can figure it out.
 * 
 * <name>
 *     A name in an expression simply returns the value of the variable with
 *     that name. If the variable was never set, it defaults to 0.
 * 
 * All binary operators have the same precedence. Sorry, I had to cut corners
 * somewhere.
 * 
```

---

## More Info

For more details about Jasic, including its syntax and how the interpreter works, explore the source code in Jasic.java. It's all there.

If you have questions, feel free to reach out. Cheers!

