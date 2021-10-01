# CP4
## 9/27/21
*EXCEPTION
_Software will often be used in conditions that designer cannot precisely anticipate
Ex:
+A user might ender data that is incorrect
+A user programmer might create or manipulate objects in incorrect ways
+Programmatic operations might fail
+System errors might occur
_Technique for highlighting errors
+Sysout(ERROR_MESSAGE);
+System.err.println(ERROR_MESSAGE);
+Return a value that indicate an error
+System.exit();
_Syntax
try {
	// some code that could throw an exception
}
catch {
	// fix problem here
finally {
	//finish things up
}

## 9/29/21
_UML access
+public, -private, #protected, ~package (default visibility)
_Classes as contracts
+Superclass makes certain promises about available methods and instance variables. These promises must be kept by all child classes. But the implementation of these promises can be overridden.
+Sometimes a superclass needs to make a promise but not implementation => use abstract: abstract class can not be instantiated
_Abstract class
+A class that extends an abstract class must: implement all abstract methods or also be an abstract class.
+Properties: Must provide constructors: private and protected constructors, child classes can reference these with super
+Provide as many as method implementations as possible
_”Multiple inheritance”
+A clone of an object is equal in content but distinct in memory footprint
+Clone is not just a copy of object’s memory, but of all of its component objects (and their components, etc.)
*Java restriction:
+If a class inherits from Cloneable class, it can not inherit from other classes
The interface
+An interface defines no implementation – only a set of abstract methods
+A class can implement any number of interfaces
