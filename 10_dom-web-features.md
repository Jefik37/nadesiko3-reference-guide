## DOM/WEB FEATURES

### HTML Manipulation (Browser Only)

```nadesiko
# Get/Set HTML content
「#id」のDOM_HTML取得
「#id」へ「<p>text</p>」をDOM_HTML設定

# Get/Set text content
「#id」のDOM_テキスト取得
「#id」へ「text」をDOM_テキスト設定

# Attributes
「#id」の「class」をDOM_属性取得
「#id」の「class」に「active」をDOM_属性設定

# Styles
「#id」の「color」をDOM_スタイル取得
「#id」の「color」に「red」をDOM_スタイル設定

# Add/Remove elements (v3.6.22+)
「#parent」へ「<div>New</div>」をDOM部品追加
「#element」をDOM部品削除
```

### Event Handling

```nadesiko
# Click event
「#button」をクリックした時には
    「Button clicked」を表示
ここまで

# Other events
「#input」を変更した時には
    valueは「#input」のDOM_テキスト取得
    valueを表示
ここまで
```

### AJAX

```nadesiko
# GET request
「https://api.example.com/data」をAJAX取得した時には
    対象を表示
ここまで

# JSON request
「https://api.example.com/json」をAJAX_JSON取得した時には
    dataは対象
    dataの「field」を表示
ここまで

# Binary data (v3.3.61+)
「image.jpg」をAJAXバイナリ取得した時には
    # Process binary data
ここまで
```

### Canvas Drawing

```nadesiko
「#canvas」へ描画開始

# Set colors
線色設定(「black」)
塗色設定(「red」)
線太設定(2)

# Draw shapes
四角描画(x, y, width, height)
円描画(x, y, radius)
線描画(x1, y1, x2, y2)

# Draw text
文字描画(x, y, 「Text」)
```

### Timers

```nadesiko
# Execute after delay
1秒後には
    「1 second passed」を表示
ここまで

# Repeat at interval
1秒毎には
    「Tick」を表示
ここまで
```
