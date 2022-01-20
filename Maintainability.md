# Maintainability

[к оглавлению](./README.md)

## Содержание

- [Architecture](./Maintainability.md#architecture)
- [Code Style](./Maintainability.md#code-style)
- [Documentation](./Maintainability.md#documentation)
- [Release success indicators](./Maintainability.md#release-success-indicators)


## <a id="architecture"></a> Architecture

## Qualified:
### 1. Knows and understands SOLID principles
S: Single Responsibility Principle (Принцип единственной ответственности).
O: Open-Closed Principle (Принцип открытости-закрытости).
L: Liskov Substitution Principle (Принцип подстановки Барбары Лисков).
I: Interface Segregation Principle (Принцип разделения интерфейса).
D: Dependency Inversion Principle (Принцип инверсии зависимостей).

### 2. KISS, DRY, …
KISS говорит не усложнять интерфейс на столько, на сколько это допустимо
DRY продвигает идею неповторяющегося кода, в случае повторений, код следует вывести в функцию и обращаться к ней
YAGNI похож на KISS, говорит о том, что не нужно добавлять вещи, которые не понадобятся

### 3. Understand the concept of Optionals, knows when to use all kinds
Optional - enum который содержит nil, или же необходимое значение. Опциональность проверяется на этапе компиляции, что снижает количество ошибок в runtime. Опциональную переменную в Swift нельзя использовать точно так же, как неопциональную. Нужно либо принудительно преобразовывать к обычному значению, либо использовать специальные преобразующие идиомы, такие как if let, guard let и ??.
    
### 4. Knows what is protocol-oriented programming
Паттерн, ориентирующийся на протоколы, а конкретно: `protocol` `extension` `constraint`
Протокол описывает интерфейс и проверяет наличие этого интерфейса при написании компонентов программы с этим протоколом.
Расширения добавляет функционал к существующему типу или протоколу. 

```swift
protocol Ordered {
    func precedes(other: Self) -> Bool
}

extension Comparable {
// Если нежелательно, чтобы метод расширения был доступен для всех Comparable, можно добавить ограничение:
// extension Ordered where Self: Comparable
// либо 
// extension Comparable where Self: Ordered
    func precedes(other: Self) -> Bool { return self < other }
}

extension Int : Ordered {}
extension String : Ordered {}
```

Констрейнты (ограничения на тип) позволяют: соответствовать протоколу наследоваться от класса или иметь тип

```swift
func produce<F: Factory>(factory: F) where F.Product == Cola
```

```swift
func fly<T>(f: T) where T: Flying, T: Animal { ... } 
func fly<T: Flying & Animal>(f: T) { ... }
func fly<T: Animal>(f: T) where T: Flying { ... }
func fly<T>(f: T) where T: Flying & Animal { ... }
```

## Competent:
### 1. Keeps responsibilities according to selected architecture
    * ?
### 2. Knows and can explain Dependency Injection, Inversion of Control
    * ?
### 3. Knows and uses generics
    * ?
### 4. Knows how to share codebase and data with app extensions/tvOS/watchOS apps
    * ?

## Expert:
### 1. Makes appropriate architecture decisions according to the situation on a lower quality in non-critical app parts, advised technical debt - if time&budget requires it
    * ?
    
## <a id="code-style"></a> Code Style
 
## Qualified:
### 1. Uses iOS team Swift guidelines (checked via SwiftLint)
    * ?

## Competent:
### 1. Minimizes SwiftLint rules disabling
    * ?
 
## <a id="documentation"></a> Documentation
 
## Qualified:
### 1. Understands why does the project need documentation and comments
Документация и комментарии помогают при работе с командой, упрощают понимание кода
 
## Competent:
### 1. Important and non-obvious places in code are covered with comments
Уникальные части кода, с которыми, возможно, мало приходилось работать остальным, при обьявлении протоколов
 
## Expert:
### 1. readme.md file contains the definition of app architecture, all dependencies, and most important app services
    * ?
 
## <a id="release-success-indicators"></a> Release success indicators
 
## Qualified:
### 1. Knows some basics from HIG, can explain some topics
    * ?
### 2. Knows one-two term from Apple Review Guidelines
    * ?
### 3. Knows how to localize the application
    * ?
 
## Competent:
### 1. Knows most of Apple Review Guidelines
    * ?
### 2. Knows how to deal with DB changes in production apps
    * ? 
### 3. Knows types of in-app purchases and how to work with them
    * ? 
### 4. Knows what types of purchases may be implemented with 3rd party payment systems
    * ?
