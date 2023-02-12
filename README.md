# Kotlin-Character-Count
 takes a list of names and a character as input, and returns the number of times that character appears in the names
``` kotlin
fun countCharacterInNames(names: List<String>, character: Char): Int {
    return names.map { it.count { it == character } }.sum()
}

// Test
val names = listOf("John", "Jane", "Jim", "Jill")
val character = 'j'
println("Number of times '$character' appears in the names: ${countCharacterInNames(names, character)}")

```

## the output will be 

```

```
