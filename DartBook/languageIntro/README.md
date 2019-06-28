# Dart语言特性

## 基础概念

- num、Function、null都是对象，所有对象继承于Object，所有未初始化的对象初始值为null。
- 可以使用var、dynamic声明变量，var在编译期匹配变量类型，类型被锁定后无法改变，dynamic被编译后实际上是object类型。
- 没有public、protected、private关键字，以_标识符开头表示私有。

## [DartPad](https://dartpad.dartlang.org)

通过dartPad了解语言特性。

## Hello World

```
printNumber(num aNumber) {
  print('The number is $aNumber.'); // 在控制台打印内容。
}

// 支持顶级方法，程序入口
main() {
  var number = 42; // 定义并初始化一个变量。
  printNumber(number); // 调用一个方法。
}
```

## Test

```
printNumber(num aNumber) {
  aNumber = 21;
  print('The number is $aNumber.'); // 在控制台打印内容。
}

main() {
  var number = 42; // 定义并初始化一个变量。
  printNumber(number); // 调用一个方法。
  
  print('The number is $number after func.');
}
```

```
class TestObject {
  num number;
  TestObject(this.number);
} 

printNumber(TestObject testObject) {
  testObject.number = 21;
  print('The number is ${testObject.number}.'); // 在控制台打印内容。
}

main() {
  TestObject testObject = new TestObject(42);
  printNumber(testObject); // 调用一个方法。
  
  print('The number is ${testObject.number} after func.');
}
```

