---
sticker: emoji//1f973
tags:
  - dart
  - classes
  - dev
---
### Enum
`enum` is [[Classes]]] to represent a fixed number of values
`enum clors {black, white, grey}` → to define the enum
then we can use it here:
```
class Car {
  int hp;          // Horsepower
  String name;     // Car name
  Color color;     // Color of the car

  Car(this.hp, this.name, this.color); // Constructor

  void displayInfo() {
    print('Car: $name, HP: $hp, Color: $color');
  }
}

void main() {
  var myCar = Car(150, 'Toyota', Color.black);
  myCar.displayInfo(); // Outputs: Car: Toyota, HP: 150, Color: Color.black
}

```

`to use it just <name of the enum>.Value`
