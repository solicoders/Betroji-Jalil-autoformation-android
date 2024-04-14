---
layout: default
chapitre: Présentation de Kotlin
order: 2
---

# Introduction to kotlin

Learn introductory programming concepts in Kotlin to prepare for building Android apps in Kotlin.

## Android Basics with Compose

- Course goals :
  - How to use Android Studio
  - Learning kotlin

1. First Program :

```Kotlin
 fun main(){
    println("Hello world")
 }
```
## Type inference

Type inference in Kotlin refers to the compiler's ability to automatically determine the type of a variable or expression without the developer needing to explicitly specify it in the code.

This means that when you initialize a variable with a value, the Kotlin compiler can infer the type of that variable based on the provided value. For example, if you initialize a variable with an integer, the compiler understands that this variable is of type Int. Similarly, if you initialize a variable with a string, the compiler infers that this variable is of type String.

Type inference allows for writing more concise and readable code because you don't need to explicitly specify the type of every variable you declare. However, it's still possible to explicitly specify the type of a variable if needed, especially in cases where the type inferred by the compiler is not clear or when you want to enhance code readability for other developers.

## pass by value

- Example

```Kotlin
fun main() {
    var nom = "Fouad"
    var bonjour_nom = Bonjour(nom)
    println (bonjour_nom)
    println (nom)
}

fun Bonjour(nom:String):String{
    nom =  "Bonjour" + nom
    return nom
}
```

- Error 

```Kotlin
Val cannot be reassigned
```

- Explaination

In pass by value, when a variable is passed as an argument to a function, a copy of the variable's value is created and passed to the function. In the example above, the variable `name` is passed to the `Bonjour` function. Inside the function, a new string is created by concatenating `Bonjour` with the original value of `name`. However, when attempting to assign this new value back to the parameter `name`, an error occurs because `name` is declared as a `val`, meaning it's immutable and cannot be reassigned. This demonstrates that changes made to the parameter inside the function do not affect the original variable outside the function.

  - Number of instructions: 4
  - Number of variables used: 2

## TP - Functions
Create a program that asks the user for two values. Then, it calculates the sum of these two values

- Solution

```kotlin
fun main() {
    println("Enter the first value:")
    val value1 = readLine()?.toDoubleOrNull()

    println("Enter the second value:")
    val value2 = readLine()?.toDoubleOrNull()

    if (value1 != null && value2 != null) {
        val sum = value1 + value2
        println("The sum of $value1 and $value2 is: $sum")
    } else {
        println("Please enter valid values.")
    }
}
```
## Références
[https://developer.android.com/courses/pathways/android-basics-compose-unit-1-pathway-1](https://developer.android.com/courses/pathways/android-basics-compose-unit-1-pathway-1)