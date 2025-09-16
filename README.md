➕ Constructor and Operator Overloading in C++

🎯 Aim
To study and implement Constructor Overloading and Operator Overloading in C++.

📚 Theory

In C++, overloading is a fundamental feature of polymorphism that allows the same function, constructor, or operator to perform different tasks depending on the context. This improves flexibility, readability, and makes code closer to natural language.

🔹 Constructor Overloading
Constructor overloading allows a class to have multiple constructors with different parameter lists. Depending on the number and type of arguments provided at the time of object creation, the appropriate constructor is invoked.

Key Characteristics:

Constructors must differ in the number or type of parameters.

Return type is not specified for constructors.

Achieves compile-time polymorphism (static binding).

Provides flexibility in object initialization.

Advantages:

Simplifies object creation by allowing multiple ways to initialize.

Enhances readability and code reusability.

Provides default, parameterized, and copy constructors under one class.

🔹 Operator Overloading
Operator overloading allows redefining the behavior of operators (+, -, *, etc.) for user-defined types (classes). This enables objects to behave like built-in types, allowing natural expressions such as c1 + c2 for complex numbers.

Key Characteristics:

Declared using the keyword operator.

Can be implemented as a member function or friend function.

Some operators (::, ., .*, ?:) cannot be overloaded.

Makes user-defined types more intuitive.

Advantages:

Improves readability and abstraction.

Makes user-defined types behave like primitives.

Reduces verbosity and increases code clarity.

📋 Algorithms

🧾 Constructor Overloading (Addition Class)
Start

Define a class Addition.

Define multiple constructors:

Addition() → default constructor.

Addition(int a, int b) → initializes with sum of two integers.

Addition(double x, double y) → initializes with sum of two doubles.

Create a display() method to show results.

In main():

Create objects using different constructors.

Display results.
End

🧾 Constructor Overloading (UserInfo Class)
Start

Define a class UserInfo.

Overload constructors with different parameter lists:

UserInfo(string name) → initializes with only name.

UserInfo(string name, int age) → initializes with name and age.

UserInfo(string name, string city) → initializes with name and city.

UserInfo(string name, int age, string city) → initializes all details.

Add a show() function to display details.

In main():

Create objects with different constructors.

Display details.
End

🧾 Operator Overloading (Complex Numbers)
Start

Define a class Complex with members real, imag.

Create a constructor to initialize values.

Overload the + operator:

Add real parts.

Add imaginary parts.

Return a new Complex object.

Define a display() method to print the result.

In main():

Create two objects c1, c2.

Compute c3 = c1 + c2.

Display c3.
End

🧾 Operator Overloading (Book Class)
Start

Define a class Book with members title, pages.

Create constructors to initialize values.

Overload the - operator:

Concatenate titles with " & ".

Add page counts.

Return a new Book object.

Define a display() method to print details.

In main():

Create two objects b1, b2.

Compute b3 = b1 - b2.

Display all three books.
End

🧠 Conclusion
This experiment demonstrates the versatility of overloading in C++:

Constructor Overloading → Multiple constructors in the same class with different parameter lists, allowing objects to be initialized in various ways.

Operator Overloading → Redefines operators for user-defined types, enabling natural expressions on objects.

Both are examples of compile-time polymorphism, resolved at compile time. Overloading improves readability, reusability, and abstraction, making C++ programs more expressive and easier to maintain.
