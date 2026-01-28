## OPERATORS

### Arithmetic

| Japanese Style               | Operator | Example                  |
|-------------------------------|---------|-------------------------|
| A(に/と)Bを足す               | A+B     | 3 + 5を表示              |
| AからBを引く                  | A-B     | 10 - 5を表示             |
| A(に/と)Bを掛ける             | A*B     | 2 * 3を表示              |
| AをBで割る                   | A/B     | 10 / 5を表示             |
| 割った余る                    | A%B     | 10 % 3を表示             |
| AのBのべき乗                   | A^B     | (2 ^ 3)を表示 #→8       |
| A&Bで文字列を連結             | A&B     | (3 & 5)を表示 #→35      |

**Important Change in v3.7.3**: The 足す command now performs numeric addition. For string concatenation, use 連結.

```nadesiko
# v3.7.3+
5に10を足す  # Returns: 15 (numeric addition)
「A」に「B」を連結  # Returns: "AB" (string concatenation - REQUIRED)

# IMPORTANT: 足す no longer concatenates strings!
# 「A」に「B」を足す  # This will try numeric conversion and likely fail
```

### Comparison

| Japanese Style               | Operator | Example                  |
|-------------------------------|---------|-------------------------|
| AがBと等しい                 | A==B    | AがBと等しいを表示      |
| AがBと等しく無い             | A!=B    | AがBと等しく無いを表示  |
| AがB未満                     | A<B     | AがB未満を表示          |
| AがB超                       | A>B     | AがB超を表示            |
| AがB以下                     | A<=B    | AがB以下を表示          |
| AがB以上                     | A>=B    | AがB以上を表示          |

### Logical

| Japanese Style        | Operator | Example                  |
|----------------------|---------|-------------------------|
| 論理AND(A, B)         | A && B  | 論理AND(A, B)を表示      |
| 論理OR(A, B)          | A \|\| B  | 論理OR(A, B)を表示       |
| 論理NOT(V)            | !V      | 論理NOT(V)を表示         |

Also: && || !

## Useful links

* ttps://nadesi.com/v3/doc/index.php?plugin_system%2F四則演算
