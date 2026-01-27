## ADVANCED FEATURES

### Inline Indent (v3.1.5+)

Use `:` for single-line blocks:

```nadesiko
# Traditional
もし A>5 ならば
    Aを表示
ここまで

# Inline (v3.1.5+)
もし A>5 ならば: Aを表示

# Can even nest (v3.7.7 allows comments after :)
arrを反復:
    もし 対象>5 ならば: 対象を表示  # This is a comment
```

### Error Handling

```nadesiko
エラー監視
    # Code that might fail
    「nonexistent.txt」を開く
エラーならば
    「Error occurred」を表示
    エラー内容を表示
ここまで
```

### Async Functions (v3.2.1+)

Nadesiko3 supports async functions for file I/O and other async operations (v3.4.21+):

```nadesiko
# File operations are async
「data.txt」を開く
contentはそれ
contentを表示
```
