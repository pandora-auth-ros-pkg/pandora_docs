# Classes

A class is generally declared in a header file as follows:

```cpp
class MyClass : public OtherClass
{
  public:
    MyClass();
    explicit MyClass(int var);
    ~MyClass();
    void someFunction();
    void someFunctionThatDoesNothing();

    void setSomeVar(int var);
    int getSomeVar() const;

  private:
    bool someInternalFunction();

    int someVar_;
    int someOtherVar_;
};
```

1. A class should have a constructor and a destructor, even if they are empty.
In case the class is [pure abstract]
(https://en.wikibooks.org/wiki/C%2B%2B_Programming/Classes/Abstract_Classes/Pure_Abstract_Classes),
the constructor can be omitted.
2. If the constructor has **only one** argument, then the keyword **explicit** is
used before it is declared.
3. The declaration order of class members have a specific form. Typedefs, static
member functions and variables are first (if they exist). Then, public, protected
and private member functions are follow and, finally, protected and private
member variables are declared.
4. There should be **NO** public variables in a class. Instead, there are used
**get/set** functions to directly access private fields.
5. The **public**, **protected** and **private** keywords are separated with an
empty line from the code above them.
6. If the class inherites from another class or has virtual functions, the
constructor should be declared as **virtual**.
7. Classes with **only static** methods should not be created. It is better to
have **global** functions inside namespaces.
8. **Static** methods can be used, if a function **independent** from the
**state** of the object is needed.
9. **Structs** are only used to define data containers. So structs should not
include methods with functionality, only **get/set** functions.
10.
