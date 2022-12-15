# S01T03 | Creating objects

> As you already know, every **instance** in programming have its **data type**. That means you must provide a type for every object in your code, otherwise the code will not compile
> 

## Here is test quiz

`quiz` select
Which is the **`second`**?
- [ ] _second_
- [x] **`second`**
- [ ] **second**
`quiz`

## Creating objects

Let’s take a look on how to create instances

```swift
var <name>: <Type> = <value>
// or create constant
let <name>: <Type> = <value>
```

It is not obligatory to put a value into the variable immediately after definition. You can do it later:

```swift
var someVariable: Int
// some code
someVariable = 5
```

## `var` and `let`

First of all, we need to define is the instance **constant** or not. Thus, will it be mutated or it will be the same for all the time

For example, your name is a constant value - `let`, but your height is variable - `var`

## Example

To create a new instance in Swift we use this construction:

```swift
let name: String = "Peter"
var height: Int = 175
```

In this example we defined 2 objects - string `name` and number `height`. After that we can use it as we want - for example print to the console or mutate:

```swift
print(name)
// prints Peter to the console
print(height)
// prints 175 to the console

name = "Tony"
// Code will fail to compile
height = 180
print(height)
// prints 180 to the console
```

If we try to change a constant value (e.g. `name`) the code will not compile. We can change only `var`, not `let`

## Type inference

Swift is smart

That means that the compiler will understand that `“Peter”` is a string and `175` is a number, so, we may skip it and just write

```swift
let name = "Peter"
// type of name is String
var height = 175
// type of height is Int
```

## Conclusion

Everything in Swift is an object and every object has its own type
