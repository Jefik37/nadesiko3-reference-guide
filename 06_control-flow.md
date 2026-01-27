## CONTROL FLOW

### Conditionals

```nadesiko
もし (condition) ならば
    # code
違えば
    # code
ここまで

# Multiple conditions
もし A=1 ならば
    「One」を表示
違えば、もし A=2 ならば
    「Two」を表示
違えば
    「Other」を表示
ここまで
```

### Loops

#### Counter Loop

```nadesiko
# Repeat N times
3回
    「Hello」を表示
ここまで
# The variable 回数 is automatically available (1, 2, 3...)

# Loop from N to M
Nを1から100まで繰り返す
    Nを表示
ここまで

# Loop with step
1から10まで2ずつ増やし繰り返す
    対象を表示  # 1, 3, 5, 7, 9
ここまで
```

#### While Loop

```nadesiko
(condition)の間
    # code
ここまで

# Example
count = 0
(count < 5)の間
    countを表示
    countに1を足す
ここまで
```

#### Array Iteration

```nadesiko
arr = [1,2,3,4,5]
arrを反復
    対象を表示  # 対象 contains current element
ここまで

# 回数 is also available (iteration index starting from 1)
arrを反復
    「Index: {回数}, Value: {対象}」を表示
ここまで
```

#### Break and Continue

```nadesiko
# Break out of loop
抜ける

# Continue to next iteration
続ける
```
