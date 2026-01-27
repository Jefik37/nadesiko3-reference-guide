## FILE I/O

### Node.js File Operations

```nadesiko
# Read file
「file.txt」を開く
dataはそれ

# Write file
「content」を「output.txt」に保存

# Append to file
「more content」を「output.txt」に追記

# File existence
もし「file.txt」が存在するならば
    「File exists」を表示
ここまで

# File size
「file.txt」のファイルサイズ

# List files
「/path/to/dir」のファイル列挙

# File operations
「source.txt」を「dest.txt」にファイルコピー
「file.txt」をファイル削除
「newdir」をフォルダ作成
```

**Note**: File I/O commands only work in Node.js (cnako3), not in browser.

### Character Encoding

Node.js version supports multiple encodings:

```nadesiko
# Read with specific encoding
「file.txt」を「UTF-8」で開く
「eucjp.txt」を「EUC-JP」で開く  # v3.3.80+

# Save with encoding
dataを「UTF-8」で「output.txt」に保存
```
