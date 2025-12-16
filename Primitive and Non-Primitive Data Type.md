                                                                                Primitive and Non-Primitive Data Types in Java

## 1. Introduction
In Java, a **data type** specifies:
- The type of data a variable can hold
- The amount of memory allocated
- The operations that can be performed on the data

↬Java data types are classified into:
- Primitive Data Types
- Non-Primitive (Reference) Data Types

## 2. Primitive Data Types
‣Primitive data types store **simple values** and are **predefined** by Java.  
‣They are not objects and do not have methods.

↬List of Primitive Data Types
| Data Type | Size |  Default Value | 
Ⓐ byte     ⇨ 1 byte    ⇨0 
Ⓑ short    ⇨ 2 bytes   ⇨ 0  
Ⓒ int      ⇨ 4 bytes   ⇨ 0  
Ⓓ long     ⇨ 8 bytes   ⇨ 0L  
Ⓔ float    ⇨ 4 bytes   ⇨ 0.0f 
Ⓕ double   ⇨ 8 bytes   ⇨ 0.0  
Ⓖ char     ⇨ 2 bytes   ⇨ '\\u0000' 
Ⓗ boolean  ⇨ 1 bit     ⇨ false 

### Example: Primitive Data Types

```java
public class PrimitiveExample {
    public static void main(String[] args) {
        int age = 21;
        double salary = 35000.50;
        char grade = 'A';
        boolean isEmployee = true;

        System.out.println(age);
        System.out.println(salary);
        System.out.println(grade);
        System.out.println(isEmployee);
    }
}

⦿ Characteristics of Primitive Data Types
➣Store actual values
➣Fixed memory size
➣Faster execution
➣Cannot store null
➣No methods available



## 3. Non-Primitive Data Types
‣Non-primitive data types store references (memory addresses) of objects.
‣They are also called reference types.

↬Examples of Non-Primitive Data Types
•String
•Array
•Class
•Object
•Interface
•Wrapper Classes

### Example: Non-Primitive Data Types
```java
public class NonPrimitiveExample {
    public static void main(String[] args) {
        String name = "Rajdip";
        int[] marks = {85, 90, 88};

        System.out.println(name);
        System.out.println(marks[1]);
    }
}

⦿ Characteristics of Non-Primitive Data Types
➣Store memory address of data
➣Size is not fixed
➣Can store multiple values
➣Can be null
➣Have built-in methods

## 4. Primitive vs Non-Primitive (Comparison)
| Feature      | Primitive | Non-Primitive |
| ------------ | --------- | ------------- |
| Stores       | Value     | Address       |
| Predefined   | Yes       | No            |
| Size         | Fixed     | Variable      |
| Methods      | No        | Yes           |
| Null allowed | No        | Yes           |
| Examples     | int, char | String, Array |

## 5. Wrapper Classes
‣In Java, wrapper classes are predefined classes that convert primitive data types into objects.
‣Each primitive data type has a corresponding wrapper class in the java.lang package.

↬Wrapper classes are mainly used when objects are required instead of primitives, such as in:
•Collections Framework
•Generics
•Frameworks (Spring, Hibernate, etc.)

◉ Primitive Types and Their Wrapper Classes
| Primitive Data Type | Wrapper Class |
| ------------------- | ------------- |
| byte                | Byte          |
| short               | Short         |
| int                 | Integer       |
| long                | Long          |
| float               | Float         |
| double              | Double        |
| char                | Character     |
| boolean             | Boolean       |

↬Example: Autoboxing
int a = 10;
Integer b = a; // Autoboxing

