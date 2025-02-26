# C++ Notes

## 1. **Macros**  
**Definition**: A macro in C++ is a preprocessor directive used to define constants or functions that are replaced by the preprocessor before the compilation.  


**Types of Macros**:
- **Object-like Macros**: Used for defining constants.  
  Example:
  ```cpp
  #define PI 3.14159
  ```
- **Function-like Macros:** Used for defining functions that take arguments.   
    Example:
  ```cpp
  #define SQUARE(x) ((x) * (x))  
    ```

**Usage**: 
- Macros are commonly used to simplify repeated code, conditional compilation, and to define constants.
- Be careful with the parentheses in function-like macros to avoid unexpected behavior.

## 2. **Scope Resolution Operator ( :: )**
**Definition**: The :: operator is used to specify the scope of a variable, function, or class, allowing you to refer to global variables, class members, or elements in namespaces.    

**Common Uses** 
- **Access Global Variables:**  
  If a local variable has the same name as a global one, :: can be used to specify the global variable. 
  Example:
  ```cpp
  int x = 10;
    void func() {
        int x = 20;
        std::cout << "Global x: " << ::x << std::endl; // Refers to global x
    }
    ```
- **Class member access:**  
  Used to define or call static members of a class outside the class definition.    
  Example:
  ```cpp
  class MyClass {
    public:
     static int value;
  };

  MyClass::value = 100;
  ```
  



 
