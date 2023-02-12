# Kotlin-Character-Count
 takes a list of names and a character as input, and returns the number of times that character appears in the names
``` kotlin
fun countCharacterInNames(names: List<String>, character: Char): Int {
    val lowercaseChar = character.toLowerCase()
    val uppercaseChar = character.toUpperCase()
    return names.map { it.count { it.toLowerCase() == lowercaseChar || it.toUpperCase() == uppercaseChar } }.sum()
}

// Test
val names = listOf("mk", "Mark", "moses", "jill")
val character = 'm'
println("Number of times '$character' appears in the names: ${countCharacterInNames(names, character)}")


```

## the output will be 

```
Number of times 'm' appears in the names: 3

```
