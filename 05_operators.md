## OPERATORS

### Arithmetic

```nadesiko
# Mathematical operators
+ - * / % ^

# Japanese style
足す (add)
引く (subtract)
掛ける (multiply)
割る (divide)
余り (modulo)
```

**Important Change in v3.7.3**: The 足す command now performs numeric addition. For string concatenation, use 連結.

```nadesiko
# v3.7.3+
5に10を足す  # Returns: 15 (numeric addition)
「A」に「B」を連結  # Returns: "AB" (string concatenation - REQUIRED)

# IMPORTANT: 足す no longer concatenates strings!
# 「A」に「B」を足す  # This will try numeric conversion and likely fail
```

### Comparison

```nadesiko
=  !=  <  >  <=  >=

# Japanese style
等しい (equal)
異なる (not equal)
```

### Logical

```nadesiko
かつ (AND)
または (OR)
でない (NOT)

# Also: &&  ||  !
```
