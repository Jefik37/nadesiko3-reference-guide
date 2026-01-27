## STRING OPERATIONS

### Basic Operations

```nadesiko
# Length (v3.7.2+ handles emoji correctly)
「Hello」の文字数  # Returns: 5
「Hello👋」の文字数  # Returns: 6 (v3.7.2+ counts emoji as 1 character)

# Substring extraction
「0123456789」の3から3  # "345" (index, length)

# Replace
「ABC」を「あいう」で「ABC DEF ABC」の置換  # "あいう DEF あいう"

# Split
「A,B,C」を「,」で区切る  # Returns: ["A", "B", "C"]

# Trim
textを空白除去
textを左トリム
textを右トリム

# Case conversion
「hello」を大文字変換  # "HELLO"
「HELLO」を小文字変換  # "hello"
```

**Important Note v3.7.2**: Unicode surrogate pair handling was significantly improved. Emoji and other multi-byte characters are now correctly counted as single characters.
