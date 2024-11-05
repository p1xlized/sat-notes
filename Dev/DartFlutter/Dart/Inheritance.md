---
sticker: emoji//1f9d3
tags: dart, dev, classes
---

### Inheritance

```
class Animal {
  String name;

  Animal(this.name);

  void speak() {
    print('$name makes a sound.');
  }
}

class Dog extends Animal {
  Dog(String name) : super(name); // Calling the superclass constructor

  @override
  void speak() {
    print('$name barks.');
  }
}

void main() {
  var dog = Dog('Buddy');
  dog.speak(); // Outputs: Buddy barks.
}

```

- `Animal` [[Classes]] is a base class & initializes the `name` property and a method `speak`.
- `Dog` Is a subclass and it inherits from `Animal` and uses `super(name)` in its constructor to call the constructor of `Animal`, passing the `name` argument.
- The `speak` method is overridden to provide a specific implementation for `Dog`.

### super()

Use `super()` in a subclass constructor to invoke the superclass constructor.
Use `super()` in a subclass constructor to invoke the superclass constructor.
- `super.methodName()`  → methods from the superclass.
- `super.propretyName`  → to access properties from the superclass.