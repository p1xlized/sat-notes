---
sticker: emoji//1f636-200d-1f32b-fe0f
---
### Abstract class
An abstract [[Classes]] in Dart is a class that cannot be instantiated directly and serves as a blueprint for other classes. It can contain abstract methods (without implementation) that must be implemented by subclasses, ensuring a consistent interface across different types.

```Shape.dart
abstract class Shape { 
	double area(); 
} 
class Circle extends Shape { 
	final double radius; 
	Circle(this.radius); 
	@override 
	double area() { 
		return 3.14 * radius * radius; 
	} 
}
```
##### Shape class
`Shape` cannot be instantiated and defines a contract for subclasses to implement the `area()` method.
##### Circle class
`Circle` extends `Shape`, provides a concrete implementation of `area()`, and initializes `radius` through its constructor.

---

### When do I use it?
**Common Behavior:** → enforce that all subclasses implement certain methods

**Code Organization:** -→related classes under a common type for better organization and code readability
