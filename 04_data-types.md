## DATA TYPES

### Strings

```nadesiko
text = 「こんにちは」
text = "hello"

# String interpolation (v3.x+)
name = 「太郎」
「こんにちは、{name}さん」を表示  # Output: こんにちは、太郎さん
```

### Numbers

```nadesiko
integer = 123
decimal = 3.14

# BigInt (v3.4.19+)
huge = 12345678901234567890n
```

### Arrays

```nadesiko
# Declaration
arr = [1, 2, 3, 4, 5]
arr = [「a」, 「b」, 「c」]

# Access (0-indexed)
arr[0]       # First element
arrの0       # Same thing
arrの2       # Third element

# Array literals can use mixed types
mixed = [1, 「text」, true, [1,2,3]]
```

**Important**: Arrays are 0-indexed, not 1-indexed.

### Dictionaries/Objects

```nadesiko
dict = {「name」: 「太郎」, 「age」: 25}

# Access
dictの「name」
dict[「age」]
```

### Booleans

**Important Change in v3.7.1**: Boolean values changed from 0/1 to true/false.

```nadesiko
# v3.7.1+
flag = true
flag = false

# Older versions used 1/0
# flag = 1  # true
# flag = 0  # false
```
