## BUILT-IN COMMANDS

### System Commands

```nadesiko
# Time/Date
今                    # Current date/time
システム時間ミリ秒    # Timestamp in milliseconds
今年                  # Current year
今月                  # Current month
今日                  # Today

# Console output
表示(value)           # Print to console/screen
言う(message)         # Alert dialog (browser)
コンソール表示(value) # Console.log (browser)

# Type conversion
整数変換(value)
実数変換(value)
文字列変換(value)

# JSON
JSONエンコード(object)
JSONデコード(string)
```

### Math Functions

```nadesiko
# Random
乱数(1, 6)           # Random integer from 1 to 6

# Basic math
ABS(value)           # Absolute value
CEIL(value)          # Ceiling
FLOOR(value)         # Floor
ROUND(value)         # Round
切捨(value)          # Truncate
切上(value)          # Round up

# Trigonometry
SIN(angle)
COS(angle)
TAN(angle)

# Other
SQRT(value)          # Square root
POW(base, exp)       # Power

# Min/Max (v3.6.41+)
MAX(a, b)            # Maximum
MIN(a, b)            # Minimum
最大値(a, b)
最小値(a, b)
CLAMP(value, min, max)  # Clamp value between min and max
```

### String Functions

```nadesiko
文字数(string)
空白除去(string)
左トリム(string)
右トリム(string)
大文字変換(string)
小文字変換(string)
置換(find, replace, target)
区切る(string, delimiter)
文字抜出(string, index, length)
文字検索(string, substring)

# v3.7.7+
文字始まる(string, prefix)    # Check if starts with
文字終わる(string, suffix)    # Check if ends with
```

### Array Functions

```nadesiko
# Basic operations
配列要素数(array)
配列追加(array, element)
配列挿入(array, index, element)
配列削除(array, index)
配列検索(array, value)

# Sorting/manipulation
配列並替(array)               # Sort
配列逆順(array)               # Reverse
配列シャッフル(array)         # Shuffle

# Statistics
配列最大(array)
配列最小(array)
配列合計(array)
合計(array)                   # v3.7.3+

# Functional programming (v3.3.80+)
配列連番作成(start, end)
配列関数適用(array, func)
配列フィルタ(array, condition)
配列要素作成(count, initialValue)  # v3.7.4+ accepts arrays
配列プッシュ(array, element)
```
