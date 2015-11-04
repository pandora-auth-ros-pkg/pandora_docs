
# Class declaration

Η σειρά δήλωσης των members μιας κλάσης έχει συγκεκριμένη μορφή. Προηγούνται οι
**public**, **protected**, **private** μέθοδοι και ακολουθούν τα **protected** και **private** πεδία   ­
με αυτή τη σειρά.

```cpp
class MyClass: public OtherClass {
    public:
        MyClass();
        explicit MyClass(int var);
        ~MyClass();

        void someFunction();
        void someFunctionThatDoesSomething();

        void setSomeVar(int var);
        int someVar() const;

    private:
        bool someInternalFunction();

        int someVar_;
        int someOhterVar_;
};
```
