## FUNCTIONS

### Defining Functions

```nadesiko
# Syntax: ●(params)function_nameとは
●(priceを)discountとは
    priceに0.8を掛けて切捨して戻す
ここまで

# Usage
100をdiscountして表示  # Output: 80

# Function without arguments
●greetingとは
    「Hello」を表示
ここまで

# Call
greeting

# Return value
●(valueを)doubleとは
    value*2で戻る
ここまで

# Can also call C-style
double(10)
```

### Special Variable それ

```nadesiko
# それ stores the result of the last operation
2に3を足して4を掛けて表示  # (2+3)*4 = 20
```

This allows method chaining in a natural Japanese style.
