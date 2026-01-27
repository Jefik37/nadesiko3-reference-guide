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
AがB以上 (greater than or equal to)
AがB以下 (less than or equal to)
AがB超 (greater than)
AがB未満 (less than)
AがBと等しい (equal)
AがBと等しく無い (not equal)
```

### Logical

```nadesiko
 &&  ||  !

# Japanese style
論理AND(A, B) (AND)
論理OR(A, B) (OR)
論理NOT(V) (NOT)
```
