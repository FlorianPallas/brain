# Java
---
## Basic Variables
- Variables can't be overshadowed. E.g. this yields an compile error
	String s = "Hello";
	if(true) { String s = "Bye"; }
## Lambda Expressions
- They are realised as anonymous classes / interfaces with one Function. Often they have the tag @FunctionalInterface to guarantee that they only contain one method.
	- The old way: 
		Predicate\<String\> is Empty = new Predicate\<String\>() {
		@Overrride public boolean test(String s) {
			return s.isEmpty();
		}
		}
	- The new way (the compiler knows which class and method to expect):
		Predicate\<String\> is Empty = (String s) -> { return s.isEmpty(); };
	- Even shorter ways 
		- Type inference: The compiler most often already knows the types of the parameter, so they can be omitted. E.g:
			Predicate\<String\> is Empty = (s) -> { return s.isEmpty(); };
		- If the lambda expression is only one return statement or one void statement the curly brackets and the return statement can be omitted. E.g:
			Predicate\<String\> is Empty = (s) -> s.isEmpty();
		- The parenthesises can be omitted if exactly one parameter is used. E.g:
			Predicate\<String\> is Empty = s -> s.isEmpty();
- Access Scope 
	- Visible variables can't be redeclared in lambda expressions just like in other code blocks. E.g.  this yields an compile error:
		String s = "Hello";
		Predicate\<String\> = s -> s.isEmpty();
	- Visible final variables can only be read not modified. Other variables can not be accessed.
	- The this reference in a lambda expression points to the this reference of the class the lambda expression is declared in.
	- Checked Exceptions inside lambda expressions have to be catched inside the lambda expression if the underlying method declaration in the functional interface has no throw annotation
- Method references
	- Class method (static method) ClassName::methodName
	- Object method (non static method) objectName::methodName
- Constructor references
	- ClassName::new