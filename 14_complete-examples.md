## COMPLETE EXAMPLES

### Example 1: FizzBuzz

```nadesiko
Nを1から100まで繰り返す
    もし、(N%3=0)かつ(N%5=0)ならば
        「FizzBuzz」を表示
    違えば、もし、N%3=0ならば
        「Fizz」を表示
    違えば、もし、N%5=0ならば
        「Buzz」を表示
    違えば
        Nを表示
    ここまで
ここまで
```

### Example 2: File Processing

```nadesiko
# Read and process CSV
「data.csv」を開く
csvはそれ

csvを「{~}」で区切る
rowsはそれ

rowsを反復
    rowは対象を「,」で区切る
    nameはrow[0]
    ageはrow[1]を整数変換

    もし、age>30ならば
        「{name} is over 30」を表示
    ここまで
ここまで
```

### Example 3: Web Scraping

```nadesiko
# Requires nadesiko3-htmlparser
!「nadesiko3-htmlparser」を取り込む

url = 「https://example.com」
urlからAJAX取得した時には
    htmlはそれ

    htmlをHTML解析
    domはそれ

    domから「h2」をDOM_SELECTORで抽出
    titlesはそれ

    titlesを反復
        それのテキストを表示
    ここまで
ここまで
```

### Example 4: Simple Web Server

```nadesiko
# Requires nadesiko3-server
!「nadesiko3-server」を取り込む

3000でWEBサーバ起動

「/」へアクセスした時には
    「<h1>Hello Nadesiko3!</h1>」をWEB送信
ここまで

「/api/time」へアクセスした時には
    timeは今
    dataは{「time」: time}
    dataをJSONエンコードしてWEB送信
ここまで

「Server running on http://localhost:3000」を表示
```

### Example 5: Interactive Calculator (Browser)

```nadesiko
「#app」へ「
<input type="text" id="num1" placeholder="Number 1">
<input type="text" id="num2" placeholder="Number 2">
<button id="add">Add</button>
<button id="subtract">Subtract</button>
<button id="multiply">Multiply</button>
<button id="divide">Divide</button>
<div id="result"></div>
」をDOM_HTML設定

●計算(演算子を)とは
    aは「#num1」のDOM_テキスト取得を整数変換
    bは「#num2」のDOM_テキスト取得を整数変換

    もし、演算子=「+」ならば
        answerはa+b
    違えば、もし、演算子=「-」ならば
        answerはa-b
    違えば、もし、演算子=「*」ならば
        answerはa*b
    違えば、もし、演算子=「/」ならば
        もし、b=0ならば
            answerは「Error: Division by zero」
        違えば
            answerはa/b
        ここまで
    ここまで

    「#result」へ「Result: {answer}」をDOM_HTML設定
ここまで

「#add」をクリックした時には: 「+」を計算
「#subtract」をクリックした時には: 「-」を計算
「#multiply」をクリックした時には: 「*」を計算
「#divide」をクリックした時には: 「/」を計算
```
