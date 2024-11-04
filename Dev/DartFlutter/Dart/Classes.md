---
tags:
  - dart
  - classes
  - dev
sticker: emoji//1f436
---

### Simple Class 
```Person.dart
class Person { 
	String name; 
	int age; 
	Person(this.name, this.age); 
	void greet() { 
		print('Hello, my name is $name and I am $age years old.'); 
}
	} 
void main() { 
ar person = Person('Alice', 30); 
person.greet(); // Outputs: Hello, my name is Alice and I am 30 years old. 
}
```

The class **Person** has 2 propreties:
1. name→ a String
2. age → a Int
`Person(this.name, this.age); ` is the constructor that initializes these properties
`greet` function is a method of the class that shows a greeting

### Getters & Setters
**Getters** and **setters** are used to encapsulate data, control access, enforce validation, and enhance code maintainability while improving readability.
**getter** -> get the value
**setter** -> set/update the value

```Person.dart
class Person {
  String _name; // Private variable
  int _age;     // Private variable

  Person(this._name, this._age);

  // Getter for name
  String get name => _name;

  // Setter for name
  set name(String value) {
    if (value.isEmpty) {
      throw ArgumentError('Name cannot be empty');
    }
    _name = value;
  }

  // Getter for age
  int get age => _age;

  // Setter for age
  set age(int value) {
    if (value < 0) {
      throw ArgumentError('Age cannot be negative');
    }
    _age = value;
  }

  void greet() {
    print('Hello, my name is $name and I am $age years old.');
  }
}

```
