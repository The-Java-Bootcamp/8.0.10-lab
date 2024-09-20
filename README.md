# Lab: 8.0.10

**Objective:**

- Understand the concept and importance of encapsulation and access control in Java development.
- Learn how to implement encapsulation using private fields, getter and setter methods, and appropriate access
  modifiers.
- Explore practical applications of encapsulation in real-world Java projects using a school management system example.
- Identify common pitfalls and best practices when working with encapsulation and access control.
- Gain hands-on experience with a complete Java example that demonstrates encapsulation and access control.

**Prerequisites:**

- Basic understanding of Java programming.
- Familiarity with creating classes and objects in Java.
- Understanding of inheritance in Java.

**What You'll Achieve:**

- Develop a solid understanding of encapsulation and access control in Java.
- Implement practical examples that can be applied in real-world scenarios such as a school management system.
- Enhance your skills in object-oriented programming, data hiding, and secure coding practices.

**Assignment Details**

In this assignment, you will create a simple school management system that demonstrates encapsulation and access
control. Follow these steps:

1. Create a base `Person` class:
    - Include private fields for `name`, `age`, and `id`.
    - Implement a constructor, getter methods, and setter methods with appropriate access control.
    - Add input validation in setter methods (e.g., age should be positive).
2. Create a `Student` class that extends `Person`:
    - Add a private field for `grade`.
    - Implement a constructor, getter, and setter for the new field.
    - Override the `toString()` method to provide a string representation of a Student.
3. Create a `Teacher` class that extends `Person`:
    - Add a private field for `subject`.
    - Implement a constructor, getter, and setter for the new field.
    - Override the `toString()` method to provide a string representation of a Teacher.
4. Create a `School` class:
    - Add private fields for school name and arrays to store students and teachers.
    - Implement methods to add students and teachers, ensuring proper encapsulation.
    - Create a method to display all students and teachers.
5. In the `main` method of a `SchoolManagementSystem` class:
    - Create a `School` object.
    - Add several `Student` and `Teacher` objects to the school.
    - Demonstrate the use of getter and setter methods.
    - Show how encapsulation prevents direct access to private fields.
    - Display all students and teachers in the school.

**Example Output**

```
Welcome to Springfield Elementary School

Adding students and teachers...

Student Details:
1. Lisa Simpson (ID: S001) - Age: 8, Grade: 3
2. Bart Simpson (ID: S002) - Age: 10, Grade: 5

Teacher Details:
1. Edna Krabappel (ID: T001) - Age: 38, Subject: General Education
2. Dewey Largo (ID: T002) - Age: 45, Subject: Music

Attempting to set invalid age for student...
Error: Age must be positive

Displaying updated student info:
Lisa Simpson (ID: S001) - Age: 9, Grade: 4

Attempting to access private field directly...
Error: age has private access in Person
```

**Starter Code**

The `TransformerBattle.java` file contains the following starter code:

```java
package academy.javapro.lab;

class Person {
    // Add your private fields here

    // Add your constructor here

    // Add your getter and setter methods here
}

class Student extends Person {
    // Add your private field here

    // Add your constructor here

    // Add your getter and setter methods here

    // Override toString() method
}

class Teacher extends Person {
    // Add your private field here

    // Add your constructor here

    // Add your getter and setter methods here

    // Override toString() method
}

class School {
    // Add your private fields here

    // Add your constructor here

    // Add methods to add students and teachers

    // Add method to display all students and teachers
}

public class SchoolManagementSystem {
    public static void main(String[] args) {
        // Create a School object
        // Add students and teachers
        // Demonstrate encapsulation and access control
    }
}

```

**Hints**

- Use the `private` keyword for fields to achieve encapsulation.
- Implement public getter and setter methods for controlled access to private fields.
- Use the `this` keyword in setter methods to distinguish between parameters and instance variables.
- In subclasses, use `super` to call the parent class constructor.
- Remember to handle potential exceptions when setting values (e.g., IllegalArgumentException for invalid input).
- When overriding `toString()`, consider using `super.toString()` to include information from the parent class.

**Submission Instructions**

1. Fork the repository
2. Clone your fork
3. Navigate into the repository
4. Implement the required classes and methods
5. Test your implementation with various inputs
6. Git add, commit, and push to your fork
7. Submit a pull request
    - Set the title of the pull request to your first name and last name
    - In the comment, briefly explain your implementation approach and any challenges you faced

Remember, the goal is to learn and have fun! Don't hesitate to ask for help if you get stuck.
