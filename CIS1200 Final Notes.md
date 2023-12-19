---
date: 2023-12-17
type: note
tags: 
---

OCaml only has static while Java has dynamic classes due to objects

All methods of classes are under class tables
- Classes have arrows to other classes to show subtyping/supertyping relationship

For private fields, if it's different objects but the same class, the different objects can all access the private fields.

this keyword cannot refer to static method
static field is a global variable

static methods can't use this pointer since static methods can only call other static methods or read/write static fields

For each loops:
```
for (type var : coll) {
	body
}

type - element type E
coll - Array of E or instance of Iterable<E>
```

switch statement, you need a break after each case
- Also need defaults

New Java code - switch expressions - no need to use break, uses -> syntax, must be exhaustive

1 byte = 8 bits - that is one input stream for I/O streams
BufferedInputStreams allows you to read a lot more at once - save time

---

OCaml abstract type is the interface (.mli) and Implementation (.ml) code. The interface provides all the type values and functions, and implementation actually defines it. The intended behavior of an abstract type is defined by the interface.

In OCaml, ; is the sequencing operator, and is used to execute expressions with side-effects like: `let () = printString...; printString...;`

Closures are stored as functions  with any external variables that are used in the function. It allows the function to access external variables that way, even if it is invoked outside of its scope. Closures encapsulates states and can create private variables and methods like objects in OO programming.
```
let g x = 
  let y = x * 2 in 
  let f z = y + z in 
  f
```
When g calls f, a closure is created in the heap which is f's code and the necessary variable it needs (which is variable y from g).

Java stores static variables in the heap. Since static variables are accessed by the class and not class instances, it has to go into the heap.

Try catch can have compile time errors if you don't write specific exceptions first.

A function is tail recursive if the last thing it does is call itself, with no further computation after that call. This means that the function doesn't need to maintain any state other than the arguments passed to the recursive call. If there's further computation or the result of the recursive call is combined with other values, the function is not tail recursive.

Simple inheritance is when a class inherits from 1 superclass

Subtype polymorphism: dynamic/runtime polymorphism, when subclass can be treated as an instance of superclass. Through inheritance and interface implementation usually.

Parametric polymorphism: allows classes and methods t o operate on different object types. Usually has a <> keyword like `Box<Integer> intergerBox = new Box<>();`

When combining subtyping and generics:
```
Even if String is subtype of Object
Queue<String> is not a subtype of Queue<Object>
Queue<String> can only be used with other Queue<String>

Thus Java generics are "invariants"
```

Exceptions must include in their interface using the throws keyword, or handled using try catch otherwise it will not compile.
![[CIS1200 Exceptions Tree.png]]


- Anonymous Inner Classes are used inside of AbstractClasses (abstract and concrete methods):
- Interfaces only have abstract methods (methods must be completed by the class itself)
```
AbstractClass ac = new AbstractClass() {
	@Override
	...
};
```
- star Look out for `new ... () {@Override}` or `() ->`, those are anonymous inner classes

dynamic class determined at runtime
```
Displaceable x;
x = new Point(2, 3)

x is the static type, Point is the dynamic type
Dynamic type needs to be subtype of the static type
```

Adapters implement all the defaults of an interface and allows you to fill in the implementation of a specific method without having to fill boilerplate for all the other methods

Inner class is a class defined within an outer class and has access to the outer class private members

A subclass is a class that inherits from another class, known as the superclass. Uses `extends`  keyword.

If a class extends another class, then it is a subclass. If a class implements another class, then it is a subtype.