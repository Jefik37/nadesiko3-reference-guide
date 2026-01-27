## TIPS & BEST PRACTICES

### 1. Code Organization

```nadesiko
# Use descriptive variable names
userName = 「太郎」
userAge = 25

# Add comments for complex logic
# This calculates the discount
priceに0.8を掛けて切捨
```

### 2. Error Handling

Always wrap potentially failing operations in error handling:

```nadesiko
エラー監視
    「file.txt」を開く
    dataはそれ
エラーならば
    「File not found」を表示
ここまで
```

### 3. Emoji and Unicode (v3.7.2+)

v3.7.2 significantly improved emoji handling:

```nadesiko
text = 「Hello👋World🌍」
textの文字数を表示  # Correct: 12 (in v3.7.2+)
                       # Old versions: 14 (counted emoji as 2 chars)
```

### 4. String Operations (v3.7.3+)

Remember the 足す command changed:

```nadesiko
# Numeric addition
5に10を足す  # 15

# String concatenation - use 連結
「A」に「B」を連結  # "AB"
```

### 5. Boolean Values (v3.7.1+)

Use true/false instead of 1/0:

```nadesiko
# v3.7.1+
flagはtrue
もし、flagならば
    # code
ここまで
```

### 6. Check Environment

```nadesiko
もし、ブラウザならば
    「Running in browser」を表示
違えば
    「Running in Node.js」を表示
ここまで
```

### 7. Efficient Iteration

Use それ for chaining:

```nadesiko
10に20を足して30を掛けて100で割って表示
# Same as: ((10 + 20) * 30) / 100
```

### 8. Module System

Create reusable modules:

```nadesiko
# lib.nako3
●(aと、bを)addとは
    a+bで戻る
ここまで

# main.nako3
!「./lib.nako3」を取り込む
5と10をaddして表示  # 15
```
