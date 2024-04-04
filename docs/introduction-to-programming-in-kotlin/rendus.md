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
**How does this work?**
 A Kotlin program is required to have a main function, which is the specific place in your code where the program starts running. The main function is the entry point, or starting point, of the program.

2. Modify your program

Try it
Now look back at the original code in the program. Can you modify the code in the Kotlin Playground so that the output shows this message instead?

`Hello, Android!`


- test 

Now look back at the original code in the program. Can you modify the code in the Kotlin Playground so that the output shows this message instead? `Hello, Android!`

```kotlin
fun main(){
    println("Hello, Android!")
}
```
3. Conclusion

**Throughout this codelab, you've:**

Worked with simple Kotlin programs, observing how changes affect the output.
Learned about troubleshooting and correcting errors in your code.
Discovered the importance of the main function as the entry point of a Kotlin program.
Defined functions using the fun keyword, specifying inputs and the function body.
Printed text to the output using the println() function.
Keep practicing and exploring! In the next codelab, you'll delve into using variables in Kotlin to create more dynamic programs.

## Create and use variables in Kotlin

1. Create and use variables in Kotlin:

```kotlin
fun main() {
    // Define variables
    val numberOfUnreadMessages: Int = 2
    val userName: String = "John"

    // Using variables with string templates
    println("$userName has $numberOfUnreadMessages unread messages.")
}
```
