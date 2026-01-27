## COMMON PITFALLS

### 1. Array Indexing

Arrays are 0-indexed:

```nadesiko
arr = [10, 20, 30]
arrの0  # 10 (first element)
arrの2  # 30 (third element)
```

### 2. Missing ここまで

Always close blocks:

```nadesiko
# WRONG
もし A>5 ならば
    Aを表示
# Missing ここまで!

# RIGHT
もし A>5 ならば
    Aを表示
ここまで
```

### 3. Reserved Words

Cannot use particles as variable names:

```nadesiko
# WRONG
を = 10  # Error!

# RIGHT
value = 10
```

### 4. File I/O in Browser

File commands don't work in browser - only in Node.js.

### 5. Particle Confusion

```nadesiko
# WRONG
valueを変数代入  # Missing particle

# RIGHT
valueを変数に代入
# or
value = 変数
```
