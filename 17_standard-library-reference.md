## Standard Library Reference

**Legend:**

- 🔸 Function (関数) - Callable command
- 🔹 Constant (定数) - Predefined value
- **Parameters** shown in parentheses use Japanese particles

**Usage Note**: Parameters are shown in format like "AをBで" where を、で、に、へ、と、から、まで are Japanese particles that indicate parameter roles.

### Core Language

- [System Constants](#system-constants) (46 items)
- [Standard Output](#standard-output) (8 items)
- [Special Commands](#special-commands) (11 items)
- [Honorifics](#honorifics) (6 items)

### Mathematics

- [Four Arithmetic Operations](#four-arithmetic-operations) (27 items)
- [Arithmetic Functions](#arithmetic-functions) (17 items)
- [Trigonometric Functions](#trigonometric-functions) (12 items)
- [Numeric Rounding](#numeric-rounding) (9 items)
- [Logical Operations](#logical-operations) (3 items)
- [Bit Operations](#bit-operations) (7 items)

### Type System

- [Type Conversion](#type-conversion) (17 items)

### Strings

- [String Processing](#string-processing) (24 items)
- [Replacement and Trim](#replacement-and-trim) (7 items)
- [Character Conversion](#character-conversion) (16 items)
- [Character Types](#character-types) (4 items)
- [Character Code](#character-code) (5 items)

### Date/Time

- [Date Time Processing](#date-time-processing) (28 items)
- [Date Time Processing (Simple)](#date-time-processing-simple)](#%E6%97%A5%E6%99%82%E5%87%A6%E7%90%86%E7%B0%A1%E6%98%93) (31 items)

### Collections

- [Array Operations](#array-operations) (34 items)
- [Two Dimensional Array Processing](#two-dimensional-array-processing) (16 items)
- [Dictionary Variable Operations](#dictionary-variable-operations) (3 items)

### Patterns

- [Regular Expressions](#regular-expressions) (4 items)
- [Specified Format](#specified-format) (3 items)

### I/O

- [File Input Output](#file-input-output) (25 items)
- [Folder Acquisition](#folder-acquisition) (11 items)
- [CSV Operations](#csv-operations) (5 items)
- [JSON](#json) (6 items)
- [BASE64](#base64) (2 items)
- [TOML](#toml) (2 items)

### Command Line

- [Command Line and Standard Input Output](#command-line-and-standard-input-output) (7 items)

### Web/Browser

- [DOM Operations](#dom-operations) (47 items)
- [DOM Operations and Events](#dom-operations-and-events) (35 items)
- [DOM Component Operations](#dom-component-operations) (32 items)
- [Drawing](#drawing) (33 items)
- [HTTP and AJAX](#http-and-ajax) (12 items)
- [New AJAX](#new-ajax) (3 items)
- [Ajax](#ajax) (18 items)
- [Local Storage](#local-storage) (12 items)
- [Blob](#blob) (1 items)
- [Clipboard Operations](#clipboard-operations) (2 items)
- [Audio](#audio) (10 items)

### Server/Network

- [HTTP Server (Express)](#http-server-express)](#http%E3%82%B5%E3%83%BC%E3%83%90express) (16 items)
- [WebSocket](#websocket) (6 items)
- [WebSocket Server](#websocket-server) (10 items)
- [SMTP](#smtp) (2 items)
- [LINE](#line) (2 items)

### Data

- [Hash Functions](#hash-functions) (8 items)
- [URL Encoding and Parameters](#url-encoding-and-parameters) (3 items)
- [Compression and Decompression](#compression-and-decompression) (6 items)

### Database

- [SQLite3](#sqlite3) (10 items)
- [MySQL](#mysql) (3 items)
- [PostgreSQL](#postgresql) (4 items)
- [SQLServer](#sqlserver) (3 items)
- [ODBC](#odbc) (8 items)
- [KUDB](#kudb) (10 items)

### Office

- [Excel](#excel)](#%E3%82%A8%E3%82%AF%E3%82%BB%E3%83%ABexcel) (18 items)

### Graphics

- [Turtle Graphics](#turtle-graphics) (31 items)
- [3D Turtle Graphics Basic Functions](#3d-turtle-graphics-basic-functions) (16 items)
- [3D Turtle Graphics Turtle Operations](#3d-turtle-graphics-turtle-operations) (34 items)
- [Graph Drawing CHARTJS](#graph-drawing-chartjs) (13 items)

### System

- [Environment Variables](#environment-variables) (2 items)
- [Timer](#timer) (8 items)
- [Node Process](#node-process) (5 items)
- [Debug Support](#debug-support) (16 items)
- [Dialog](#dialog) (5 items)
- [Plugin Management](#plugin-management) (5 items)

### Advanced

- [Asynchronous Processing Guarantee](#asynchronous-processing-guarantee) (6 items)
- [NAKO Worker](#nako-worker) (14 items)
- [Machine Learning](#machine-learning) (10 items)
- [Morphological Analysis (MECAB)](#morphological-analysis-mecab)](#%E5%BD%A2%E6%85%8B%E7%B4%A0%E8%A7%A3%E6%9E%90mecab) (2 items)
- [Speech Synthesis](#speech-synthesis) (10 items)
- [Music](#music) (5 items)

---

## Core Language

### System Constants

**Constants:**

```nadesiko
# 🔹 ナデシコバージョン - '?'
# 🔹 ナデシコ言語バージョン - '?'
# 🔹 ナデシコエンジン - 'nadesi.com/v3'
# 🔹 ナデシコ種類 - '?'
# 🔹 はい - true
# 🔹 いいえ - false
# 🔹 真 - true
# 🔹 偽 - false
# 🔹 永遠 - true
# 🔹 オン - true
# 🔹 オフ - false
# 🔹 改行 - '\n'
# 🔹 タブ - '\t'
# 🔹 カッコ - '「'
# 🔹 カッコ閉 - '」'
# 🔹 波カッコ - '{'
# 🔹 波カッコ閉 - '}'
# 🔹 OK - true
# 🔹 NG - false
# 🔹 キャンセル - 0
# 🔹 TRUE - true
# 🔹 FALSE - false
# 🔹 true - true
# 🔹 false - false
# 🔹 PI - Math.PI
# 🔹 空 - ''
# 🔹 NULL - null
# 🔹 undefined - undefined
# 🔹 未定義 - undefined
# 🔹 エラーメッセージ - ''
# 🔹 対象 - ''
# 🔹 対象キー - ''
# 🔹 回数 - ''
# 🔹 CR - '\r'
# 🔹 LF - '\n'
# 🔹 非数 - NaN
# 🔹 無限大 - Infinity
# 🔹 戻値無 - 0
# 🔹 戻値有 - 1
# 🔹 Eアプリ - app
# 🔹 IPCメイン - ipcMain
```

**Functions:**

```nadesiko
# 🔸 空配列
#    空の配列を返す。『[]』と同義。

# 🔸 空辞書
#    空の辞書型を返す。『{}』と同義。

# 🔸 空ハッシュ
#    空のハッシュを返す(v3.2以降非推奨)

# 🔸 空オブジェクト
#    空のオブジェクトを返す(v3.2以降非推奨)

# 🔸 真偽判定 (Bの/Bを)
#    引数bが真(true)ならば「真」を偽(false)ならば「偽」を返す
```

### Standard Output

**Constants:**

```nadesiko
# 🔹 表示ログ - ''
```

**Functions:**

```nadesiko
# 🔸 表示 (Sを/Sと)
#    Sを表示

# 🔸 継続表示 (Sを/Sと)
#    Sを改行なしで表示(ただし「表示」命令を使うことで画面出力される)

# 🔸 連続表示 (...Aと/...Aを)
#    引数に指定した引数を全て表示する(可変引数)

# 🔸 連続無改行表示 (...Aと/...Aを)
#    引数に指定した引数を全て表示する（改行しない)(可変引数)

# 🔸 表示ログクリア
#    表示ログを空にする

# 🔸 言 (Sを/Sと)
#    Sを表示

# 🔸 コンソール表示 (Sを/Sと)
#    Sをコンソール表示する(console.log)
```

### Special Commands

**Functions:**

```nadesiko
# 🔸 JS実行 (SRCを/SRCで)
#    JavaScriptのコードSRCを実行する(変数sysでなでしこシステムを参照できる)

# 🔸 JSオブジェクト取得 (NAMEの)
#    なでしこで定義した関数や変数nameのJavaScriptオブジェクトを取得する

# 🔸 JS関数実行 (NAMEをARGSで)
#    JavaScriptの関数NAMEを引数ARGS(配列)で実行する

# 🔸 ASYNC
#    なでしこのユーザー関数定義でASYNC(非同期関数である)ことを宣言する(非同期関数)

# 🔸 AWAIT実行 (FをARGSで)
#    JavaScriptの非同期関数(Promise/async関数)のFを引数ARGSでawait実行する(非同期関数)

# 🔸 JSメソッド実行 (OBJのMをARGSで)
#    JavaScriptのオブジェクトOBJのメソッドMを引数ARGS(配列)で実行する

# 🔸 ナデシコ (CODEを/CODEで)
#    なでしこのコードCODEを実行する

# 🔸 ナデシコ続 (CODEを/CODEで)
#    なでしこのコードCODEを実行する

# 🔸 実行 (Fを/Fに/Fで)
#    無名関数（あるいは、文字列で関数名を指定）Fを実行する(Fが関数でなければ無視する)

# 🔸 実行時間計測 (Fの)
#    関数Fを実行して要した時間をミリ秒で返す

# 🔸 終
#    終わる
```

### Honorifics

**Functions:**

```nadesiko
# 🔸 ください
#    敬語対応のため

# 🔸 お願い
#    ソースコードを読む人を気持ちよくする

# 🔸 です
#    ソースコードを読む人を気持ちよくする

# 🔸 拝啓
#    ソースコードを読む人を気持ちよくする

# 🔸 敬具
#    ソースコードを読む人を気持ちよくする

# 🔸 礼節レベル取得
#    (お遊び)敬語を何度使ったか返す
```

Links:
* https://nadesi.com/v3/doc/index.php?文法%2F敬語

## Mathematics

### Four Arithmetic Operations

**Functions:**

```nadesiko
# 🔸 足 (AにBを/Aと)
#    AとBを足す(算術演算を行う)

# 🔸 合計 (...Aと/...Aを/...Aの)
#    引数(可変)に指定した値を全て合計して返す(可変引数)

# 🔸 引 (AからBを)
#    AからBを引く

# 🔸 掛 (AにBを/Aと)
#    AにBを掛ける

# 🔸 倍 (AのB/Aを)
#    AのB倍を求める

# 🔸 割 (AをBで)
#    AをBで割る

# 🔸 割余 (AをBで)
#    AをBで割った余りを求める

# 🔸 偶数 (Aが)
#    Aが偶数なら真を返す

# 🔸 奇数 (Aが)
#    Aが奇数なら真を返す

# 🔸 二乗 (Aの/Aを)
#    Aを二乗する

# 🔸 べき乗 (AのBの)
#    AのB乗を求める

# 🔸 以上 (AがB)
#    AがB以上か

# 🔸 以下 (AがB)
#    AがB以下か

# 🔸 未満 (AがB)
#    AがB未満か

# 🔸 超 (AがB)
#    AがB超か

# 🔸 等 (AがBと)
#    AがBと等しいか

# 🔸 等無 (AがBと)
#    AがBと等しくないか

# 🔸 一致 (AがBと)
#    AがBと一致するか(配列や辞書も比較可能)

# 🔸 不一致 (AがBと)
#    AがBと不一致か(配列や辞書も比較可能)

# 🔸 範囲内 (VがAからBの/Bまでの)
#    VがAからBの範囲内か

# 🔸 範囲 (AからBの/Bまでの)
#    AからBの範囲を表現する範囲オブジェクトを返す

# 🔸 連続加算 (Bを...Aに/...Aと)
#    A1+A2+A3...にBを足す(可変引数)

# 🔸 MAX (Bの...Aと)
#    2個以上の数値のうち最大値を返す。(可変引数)

# 🔸 最大値 (Bの...Aと)
#    2個以上の数値のうち最大値を返す。(可変引数)

# 🔸 MIN (Bの...Aと)
#    2個以上の数値のうち最小値を返す。(可変引数)

# 🔸 最小値 (Bの...Aと)
#    2個以上の数値のうち最小値を返す。(可変引数)

# 🔸 CLAMP (XのAからBまでの/XをBで)
#    数値を下限から上限の範囲内に収めた値を返す。
```

### Arithmetic Functions

**Functions:**

```nadesiko
# 🔸 SIGN (Vの)
#    Vが0なら0を、0超なら1を、0未満なら-1を返す

# 🔸 符号 (Vの)
#    Vが0なら0を、0超なら1を、0未満なら-1を返す

# 🔸 ABS (Aの)
#    Vの絶対値を返す

# 🔸 絶対値 (Aの)
#    Vの絶対値を返す

# 🔸 EXP (Aの)
#    e（自然対数の底）の A 乗の値を返す

# 🔸 HYPOT (AとBの)
#    直角三角形の二辺の長さA,Bから斜辺を求めて返す。

# 🔸 斜辺 (AとBの)
#    直角三角形の二辺の長さA,Bから斜辺を求めて返す。

# 🔸 LN (Aの)
#    実数式 A の自然対数（Ln(e) = 1）を返す

# 🔸 LOG (Aの)
#    Aの自然対数（底はE）を返す

# 🔸 LOGN (AでBの)
#    指定された底AでBの対数を計算して返す

# 🔸 FRAC (Aの)
#    実数Aの小数部分を返す

# 🔸 小数部分 (Aの)
#    実数Aの小数部分を返す

# 🔸 整数部分 (Aの)
#    実数Aの整数部分を返す

# 🔸 乱数 (Aの)
#    0から(A-1)までの乱数を返す。引数Aには範囲オブジェクトや配列[最小,最大]も指定可能

# 🔸 乱数範囲 (AからBまでの/Bの)
#    AからBまでの範囲の乱数を返す

# 🔸 SQRT (Aの)
#    Aの平方根を返す

# 🔸 平方根 (Aの)
#    Aの平方根を返す
```

Links:
* https://nadesi.com/v3/doc/index.php?plugin_system%2F四則演算

### Trigonometric Functions

**Functions:**

```nadesiko
# 🔸 SIN (Vの)
#    ラジアン単位VのSINを求める

# 🔸 COS (Vの)
#    ラジアン単位VのCOSを求める

# 🔸 TAN (Vの)
#    ラジアン単位VのTANを求める

# 🔸 ARCSIN (Vの)
#    ラジアン単位VのARCSINを求める

# 🔸 ARCCOS (Vの)
#    ラジアン単位VのARCCOSを求める

# 🔸 ARCTAN (Vの)
#    ラジアン単位VのARCTANを求める

# 🔸 ATAN2 (YとXの)
#    ARCTAN(Y/X)をラジアン単位で返す

# 🔸 座標角度計算 (XYの)
#    点[0,0]から[x,y]の直線とX軸の角度(度)を返す

# 🔸 RAD2DEG (Vを)
#    ラジアンから度に変換

# 🔸 DEG2RAD (Vを)
#    度からラジアンに変換

# 🔸 度変換 (Vを)
#    ラジアンから度に変換

# 🔸 ラジアン変換 (Vを)
#    度からラジアンに変換
```

### Numeric Rounding

**Functions:**

```nadesiko
# 🔸 ROUND (Vを)
#    実数型の値Vを丸めてもっとも近い整数値を返す

# 🔸 四捨五入 (Vを/Vの)
#    実数型の値Vを丸めてもっとも近い整数値を返す

# 🔸 小数点切上 (AをBで)
#    整数Aを小数点第B桁で切り上げして返す

# 🔸 小数点切下 (AをBで)
#    整数Aを小数点第B桁で切り下げして返す

# 🔸 小数点四捨五入 (AをBで)
#    実数Aを小数点第B桁で四捨五入して返す

# 🔸 CEIL (Vを)
#    数値を正の無限大方向へ切り上げて返す。

# 🔸 切上 (Vを)
#    数値を正の無限大方向へ切り上げて返す。

# 🔸 FLOOR (Vを)
#    数値を負の無限大方向へ切り下げて返す。

# 🔸 切捨 (Vを)
#    数値を負の無限大方向へ切り下げて返す。
```

### Logical Operations

**Functions:**

```nadesiko
# 🔸 論理OR (AとBの)
#    AとBの論理和を返す(v1非互換)。

# 🔸 論理AND (AとBの)
#    AとBの論理積を返す(v1非互換)。日本語の「AかつB」に相当する

# 🔸 論理NOT (Vの)
#    値Vが0や空ならばtrue、それ以外ならばfalseを返す(v1非互換)
```

### Bit Operations

**Functions:**

```nadesiko
# 🔸 OR (AとBの)
#    (ビット演算で)AとBの論理和を返す。

# 🔸 AND (AとBの)
#    (ビット演算で)AとBの論理積を返す。日本語の「AかつB」に相当する

# 🔸 XOR (AとBの)
#    (ビット演算で)AとBの排他的論理和を返す。

# 🔸 NOT (Vの)
#    (ビット演算で)Vの各ビットを反転して返す。

# 🔸 SHIFT_L (VをAで)
#    VをAビット左へシフトして返す

# 🔸 SHIFT_R (VをAで)
#    VをAビット右へシフトして返す(符号を維持する)

# 🔸 SHIFT_UR (VをAで)
#    VをAビット右へシフトして返す(符号を維持しない、0で埋める)
```

## Type System

### Type Conversion

**Functions:**

```nadesiko
# 🔸 変数型確認 (Vの)
#    変数Vの型を返す

# 🔸 TYPEOF (Vの)
#    変数Vの型を返す

# 🔸 文字列変換 (Vを)
#    値Vを文字列に変換

# 🔸 TOSTR (Vを)
#    値Vを文字列に変換

# 🔸 整数変換 (Vを)
#    値Vを整数に変換

# 🔸 TOINT (Vを)
#    値Vを整数に変換

# 🔸 実数変換 (Vを)
#    値Vを実数に変換

# 🔸 TOFLOAT (Vを)
#    値Vを実数に変換

# 🔸 INT (Vの)
#    値Vを整数に変換

# 🔸 FLOAT (Vの)
#    値Vを実数に変換

# 🔸 NAN判定 (Vを)
#    値VがNaNかどうかを判定(命令『非数判定』を使う事を推奨)

# 🔸 非数判定 (Vを)
#    値Vが非数かどうかを判定(NAN判定より堅牢)

# 🔸 HEX (Aの)
#    値Vを16進数に変換

# 🔸 進数変換 (VをN/Vの)
#    値VをN進数に変換

# 🔸 二進 (Vを/Vの/Vから)
#    値Vを2進数に変換

# 🔸 二進表示 (Vを/Vの/Vから)
#    値Vを2進数に変換して表示

# 🔸 RGB (RとGのBで)
#    HTML用のカラーコードを返すRGB(R,G,B)で各値は0-255
```

## Strings

### String Processing

**Functions:**

```nadesiko
# 🔸 文字数 (Vの)
#    文字列Vの文字数を返す

# 🔸 何文字目 (SでAが/Sの)
#    文字列SでAが何文字目にあるか調べて返す。見つからなければ0を返す。

# 🔸 CHR (Vの)
#    文字コードV(あるいは文字列配列)から文字を返す

# 🔸 ASC (Vの)
#    文字列V(あるいは文字列配列)の最初の文字の文字コードを返す

# 🔸 文字挿入 (SでIにAを/SのIへ)
#    文字列SのI文字目に文字列Aを挿入する

# 🔸 文字検索 (SでAからBを/Sの)
#    文字列SでA文字目から文字列Bを検索。見つからなければ0を返す。(類似命令に『何文字目』がある)(v1非互換)

# 🔸 追加 (SでAを/Sに/Sへ)
#    文字列または配列SにAを追加して返す(v1非互換)

# 🔸 一行追加 (SでAを/Sに/Sへ)
#    文字列または配列SにAと改行を追加して返す(v1非互換)

# 🔸 連結 (...Aと/...Aを)
#    引数(可変)に指定した文字列を連結して文字列を返す(可変引数)

# 🔸 文字列連結 (...Aと/...Aを)
#    引数(可変)に指定した文字列を連結して文字列を返す(可変引数)

# 🔸 文字列分解 (Vを/Vの/Vで)
#    文字列Vを一文字ずつに分解して返す

# 🔸 リフレイン (VをCNTで/Vの)
#    文字列VをCNT回繰り返す(v1非互換)

# 🔸 出現回数 (SでAの)
#    文字列SにAが何回出現するか数える

# 🔸 MID (SでAからCNTを/Sの)
#    文字列SのA文字目からCNT文字を抽出する(『文字抜出』と同じ)

# 🔸 文字抜出 (SでAからCNTを/SのCNT)
#    文字列SのA文字目からCNT文字を抽出する

# 🔸 LEFT (SのCNTだけ/Sで)
#    文字列Sの左端からCNT文字を抽出する

# 🔸 文字左部分 (SのCNTだけ/SでCNT)
#    文字列Sの左端からCNT文字を抽出する

# 🔸 RIGHT (SのCNTだけ/Sで)
#    文字列Sの右端からCNT文字を抽出する(『文字右部分』と同じ)

# 🔸 文字右部分 (SのCNTだけ/SでCNT)
#    文字列Sの右端からCNT文字を抽出する

# 🔸 区切 (SのAで/Sを)
#    文字列Sを区切り文字Aで区切って配列で返す

# 🔸 文字列分割 (SをAで)
#    文字列Sを区切り文字Aで分割して配列で返す

# 🔸 切取 (SからAまで/SのAを)
#    文字列Sから文字列Aまでの部分を抽出する。切り取った残りは特殊変数『対象』に代入される。(v1非互換)

# 🔸 範囲切取 (SでAからBまで/SのBを)
#    文字列Sで文字列AからBまでの部分を抽出して返す。切り取った残りは特殊変数『対象』に代入される。(v1非互換)

# 🔸 文字削除 (SのAからBだけ/Bを/B)
#    文字列SのA文字目からB文字分を削除して返す
```

### Replacement and Trim

**Functions:**

```nadesiko
# 🔸 置換 (SのAをBに/SでAからBへ)
#    文字列Sのうち文字列AをBに全部置換して返す

# 🔸 単置換 (SのAをBに/SでBへ)
#    文字列Sのうち、最初に出現するAだけをBに置換して返す

# 🔸 トリム (Sの/Sを)
#    文字列Sの前後にある空白を削除する

# 🔸 空白除去 (Sの/Sを)
#    文字列Sの前後にある空白を削除する

# 🔸 右トリム (Sの/Sを)
#    文字列Sの末尾にある空白を削除する

# 🔸 左トリム (Sの/Sを)
#    文字列Sの先頭にある空白を削除する

# 🔸 末尾空白除去 (Sの/Sを)
#    文字列Sの末尾にある空白を削除する
```

### Character Conversion

**Constants:**

```nadesiko
# 🔹 全角カナ一覧 - 'アイウエオカキクケコサシスセソタチツテトナニヌネノハヒフヘホマミムメモヤユヨラリルレロワヲンァィゥェォャュョッ、。ー「」'
# 🔹 全角カナ濁音一覧 - 'ガギグゲゴザジズゼゾダヂヅデドバビブベボパピプペポ'
# 🔹 半角カナ一覧 - 'ｱｲｳｴｵｶｷｸｹｺｻｼｽｾｿﾀﾁﾂﾃﾄﾅﾆﾇﾈﾉﾊﾋﾌﾍﾎﾏﾐﾑﾒﾓﾔﾕﾖﾗﾘﾙﾚﾛﾜｦﾝｧｨｩｪｫｬｭｮｯ､｡ｰ｢｣ﾞﾟ'
# 🔹 半角カナ濁音一覧 - 'ｶﾞｷﾞｸﾞｹﾞｺﾞｻﾞｼﾞｽﾞｾﾞｿﾞﾀﾞﾁﾞﾂﾞﾃﾞﾄﾞﾊﾞﾋﾞﾌﾞﾍﾞﾎﾞﾊﾟﾋﾟﾌﾟﾍﾟﾎﾟ'
```

**Functions:**

```nadesiko
# 🔸 大文字変換 (Sの/Sを)
#    アルファベットの文字列Sを大文字に変換

# 🔸 小文字変換 (Sの/Sを)
#    アルファベットの文字列Sを小文字に変換

# 🔸 平仮名変換 (Sの/Sを)
#    文字列Sのカタカナをひらがなに変換

# 🔸 カタカナ変換 (Sの/Sを)
#    文字列Sのひらがなをカタカナに変換

# 🔸 英数全角変換 (Sの/Sを)
#    文字列Sの半角英数文字を全角に変換

# 🔸 英数半角変換 (Sの/Sを)
#    文字列Sの全角英数文字を半角に変換

# 🔸 英数記号全角変換 (Sの/Sを)
#    文字列Sの半角英数記号文字を全角に変換

# 🔸 英数記号半角変換 (Sの/Sを)
#    文字列Sの記号文字を半角に変換

# 🔸 カタカナ全角変換 (Sの/Sを)
#    文字列Sの半角カタカナを全角に変換

# 🔸 カタカナ半角変換 (Sの/Sを)
#    文字列Sの全角カタカナを半角に変換

# 🔸 全角変換 (Sの/Sを)
#    文字列Sの半角文字を全角に変換

# 🔸 半角変換 (Sの/Sを)
#    文字列Sの全角文字を半角に変換
```

### Character Types

**Functions:**

```nadesiko
# 🔸 かなか判定 (Sを/Sの/Sが)
#    文字列Sの1文字目がひらがなか判定

# 🔸 カタカナ判定 (Sを/Sの/Sが)
#    文字列Sの1文字目がカタカナか判定

# 🔸 数字判定 (Sを/Sが)
#    文字列Sの1文字目が数字か判定

# 🔸 数列判定 (Sを/Sが)
#    文字列S全部が数字か判定
```

### Character Code

**Functions:**

```nadesiko
# 🔸 文字コード変換サポート判定 (CODEの/CODEを)
#    文字コードCODEをサポートしているか確認

# 🔸 SJIS変換 (STRに/STRへ/STRを)
#    (v1非互換)文字列をShift_JISのバイナリバッファに変換

# 🔸 SJIS取得 (BUFから/BUFを/BUFで)
#    Shift_JISのバイナリバッファを文字列に変換

# 🔸 エンコーディング変換 (SをCODEへ/CODEで)
#    文字列SをCODEへ変換してバイナリバッファを返す

# 🔸 エンコーディング取得 (BUFをCODEから/CODEで)
#    バイナリバッファBUFをCODEから変換して返す
```

## Date/Time

### Date Time Processing

**Constants:**

```nadesiko
# 🔹 元号データ - era
```

**Functions:**

```nadesiko
# 🔸 今
#    現在時刻を「HH:mm:ss」の形式で返す

# 🔸 システム時間
#    現在のUNIX時間 (UTC(1970/1/1)からの経過秒数) を返す

# 🔸 今日
#    今日の日付を「YYYY/MM/DD」の形式で返す

# 🔸 明日
#    明日の日付を「YYYY/MM/DD」の形式で返す (v1非互換)

# 🔸 昨日
#    昨日の日付を「YYYY/MM/DD」の形式で返す (v1非互換)

# 🔸 今年
#    今年が何年かを西暦で返す

# 🔸 来年
#    来年が何年かを西暦で返す

# 🔸 去年
#    去年が何年かを西暦で返す

# 🔸 今月
#    今月が何月かを返す

# 🔸 来月
#    来月が何月かを返す

# 🔸 先月
#    先月が何月かを返す

# 🔸 曜日 (Sの)
#    日付Sの曜日を返す

# 🔸 曜日番号取得 (Sの)
#    Sに指定した日付の曜日番号をで返す。不正な日付の場合は今日の曜日番号を返す。(0=日/1=月/2=火/3=水/4=木/5=金/6=土)

# 🔸 UNIX時間変換 (Sの/Sを/Sから)
#    日時SをUNIX時間 (UTC(1970/1/1)からの経過秒数) に変換して返す(v1非互換)

# 🔸 UNIXTIME変換 (Sの/Sを/Sから)
#    日時SをUNIX時間 (UTC(1970/1/1)からの経過秒数) に変換して返す

# 🔸 日時変換 (TMを/TMから)
#    UNIX時間 (UTC(1970/1/1)からの経過秒数) を「YYYY/MM/DD HH:mm:ss」の形式に変換

# 🔸 和暦変換 (Sを)
#    Sを和暦に変換する。Sは明治以降の日付が有効。

# 🔸 年数差 (AとBの/AからBまでの)
#    日付AとBの差を年数で求めて返す。A<Bなら正の数、そうでないなら負の数を返す (v1非互換)。

# 🔸 月数差 (AとBの/AからBまでの)
#    日付AとBの差を月数で求めて返す。A<Bなら正の数、そうでないなら負の数を返す (v1非互換)。

# 🔸 日数差 (AとBの/AからBまでの)
#    日付AとBの差を日数で求めて返す。A<Bなら正の数、そうでないなら負の数を返す。

# 🔸 日時差 (AとBのUNITによる/AからBまでの)
#    日時AとBの差を種類unitで返す。A<Bなら正の数、そうでないなら負の数を返す (v1非互換)。

# 🔸 時間差 (AとBの/AからBまでの)
#    時間AとBの時間の差を求めて返す。A<Bなら正の数、そうでないなら負の数を返す。

# 🔸 分差 (AとBの/AからBまでの)
#    時間AとBの分数の差を求めて返す。A<Bなら正の数、そうでないなら負の数を返す。

# 🔸 秒差 (AとBの/AからBまでの)
#    時間AとBの差を秒差で求めて返す。A<Bなら正の数、そうでないなら負の数を返す。

# 🔸 時間加算 (SにAを)
#    時間SにAを加えて返す。Aには「(+｜-)hh:nn:dd」で指定する。

# 🔸 日付加算 (SにAを)
#    日付SにAを加えて返す。Aには「(+｜-)yyyy/mm/dd」で指定する。

# 🔸 日時加算 (SにAを)
#    日時SにAを加えて返す。Aは「(+｜-)1(年/ヶ月/日/時間/分/秒)」のように指定する (v1非互換)。
```

### Date Time Processing (Simple)

**Constants:**

```nadesiko
# 🔹 元号データ - [{ '元号': '令和', '改元日': '2019/05/01' }, { '元号': '平成', '改元日': '1989/01/08' }, { '元号': '昭和', '改元日': '1926/12/25' }, { '元号': '大正', '改元日': '1912/07/30' }, { '元号': '明治', '改元日': '1868/10/23' }]
```

**Functions:**

```nadesiko
# 🔸 今
#    現在時刻を「HH:mm:ss」の形式で返す

# 🔸 システム時間
#    現在のUNIX時間 (UTC(1970/1/1)からの経過秒数) を返す

# 🔸 システム時間ミリ秒
#    現在のUNIX時間 (UTC(1970/1/1)からの経過秒数) をミリ秒で返す

# 🔸 今日
#    今日の日付を「YYYY/MM/DD」の形式で返す

# 🔸 明日
#    明日の日付を「YYYY/MM/DD」の形式で返す

# 🔸 昨日
#    昨日の日付を「YYYY/MM/DD」の形式で返す

# 🔸 今年
#    今年が何年かを西暦で返す

# 🔸 来年
#    来年が何年かを西暦で返す

# 🔸 去年
#    去年が何年かを西暦で返す

# 🔸 今月
#    今月が何月かを返す

# 🔸 来月
#    来月が何月かを返す

# 🔸 先月
#    先月が何月かを返す

# 🔸 曜日 (Sの)
#    Sに指定した日付の曜日を返す。不正な日付の場合は今日の曜日を返す。

# 🔸 曜日番号取得 (Sの)
#    Sに指定した日付の曜日番号を番号で返す。不正な日付の場合は今日の曜日番号を返す。(0=日/1=月/2=火/3=水/4=木/5=金/6=土)

# 🔸 UNIXTIME変換 (Sの/Sを/Sから)
#    日時SをUNIX時間 (UTC(1970/1/1)からの経過秒数) に変換して返す(v1非互換)

# 🔸 UNIX時間変換 (Sの/Sを/Sから)
#    日時SをUNIX時間 (UTC(1970/1/1)からの経過秒数) に変換して返す(v1非互換)

# 🔸 日時変換 (TMを/TMから)
#    UNIX時間 (UTC(1970/1/1)からの経過秒数) を「YYYY/MM/DD HH:mm:ss」の形式に変換

# 🔸 日時書式変換 (TMをFMTで)
#    UNIX時間TM(または日付文字列)を「YYYY/MM/DD HH:mm:ss」または「YY-M-D H:m:s」その他、W:曜日、WWW:曜日英、MMM:月英、ccc:ミリ秒の書式に変換

# 🔸 和暦変換 (Sを)
#    Sを和暦に変換する。Sは明治以降の日付が有効。

# 🔸 年数差 (AとBの/AからBまでの)
#    日付AとBの差を年数で求めて返す。A<Bなら正の数、そうでないなら負の数を返す (v1非互換)。

# 🔸 月数差 (AとBの/AからBまでの)
#    日付AとBの差を月数で求めて返す。A<Bなら正の数、そうでないなら負の数を返す (v1非互換)。

# 🔸 日数差 (AとBの/AからBまでの)
#    日付AとBの差を日数で求めて返す。A<Bなら正の数、そうでないなら負の数を返す。

# 🔸 時間差 (AとBの/AからBまでの)
#    時間AとBの時間の差を求めて返す。A<Bなら正の数、そうでないなら負の数を返す。

# 🔸 分差 (AとBの/AからBまでの)
#    時間AとBの分数の差を求めて返す。A<Bなら正の数、そうでないなら負の数を返す。

# 🔸 秒差 (AとBの/AからBまでの)
#    時間AとBの差を秒差で求めて返す。A<Bなら正の数、そうでないなら負の数を返す。

# 🔸 日時差 (AとBのUNITによる/AからBまでの)
#    日時AとBの差を種類unitで返す。A<Bなら正の数、そうでないなら負の数を返す (v1非互換)。

# 🔸 時間加算 (SにAを)
#    時間SにAを加えて返す。Aには「(+｜-)hh:nn:dd」で指定する。

# 🔸 日付加算 (SにAを)
#    日付SにAを加えて返す。Aには「(+｜-)yyyy/mm/dd」で指定する。

# 🔸 日時加算 (SにAを)
#    日時SにAを加えて返す。Aは「(+｜-)1(年/ヶ月/日/週/時間/分/秒)」のように指定する (v1非互換)。

# 🔸 時間ミリ秒取得
#    ミリ秒単位の時間を数値で返す。結果は実装に依存する。
```

## Collections

### Array Operations

**Functions:**

```nadesiko
# 🔸 配列結合 (AをSで)
#    配列Aを文字列Sでつなげて文字列で返す

# 🔸 配列只結合 (Aを)
#    配列Aの要素をただ結合して文字列で返す。(「」で配列結合と同じ)

# 🔸 配列検索 (AのSを/Aから)
#    配列Aから文字列Sを探してインデックス番号(0起点)を返す。見つからなければ-1を返す。

# 🔸 配列要素数 (Aの)
#    配列Aの要素数を返す

# 🔸 要素数 (Aの)
#    Aの要素数を返す。Aには配列/辞書型/文字列を指定する。

# 🔸 LEN (Aの)
#    Aの要素数を返す。Aには配列/辞書型/文字列を指定する。

# 🔸 配列挿入 (AのIにSを/Iへ)
#    配列AのI番目(0起点)に要素Sを追加して返す(v1非互換)

# 🔸 配列一括挿入 (AのIにBを/Iへ)
#    配列AのI番目(0起点)に配列bを追加して返す(v1非互換)

# 🔸 配列ソート (Aの/Aを)
#    配列Aをソートして返す(A自体を変更)

# 🔸 配列数値変換 (Aの/Aを)
#    配列Aの各要素を数値に変換して返す(変数A自体を変更)

# 🔸 配列数値ソート (Aの/Aを)
#    配列Aをソートして返す(A自体を変更)

# 🔸 配列カスタムソート (FでAの/Aを)
#    関数Fで配列Aをソートして返す(引数A自体を変更)

# 🔸 配列逆順 (Aの/Aを)
#    配列Aを逆にして返す。Aを書き換える(A自体を変更)。

# 🔸 配列シャッフル (Aの/Aを)
#    配列Aをシャッフルして返す。Aを書き換える

# 🔸 配列削除 (AのIを/Aから)
#    配列AのI番目(0起点)の要素を削除して返す。Aの内容を書き換える。辞書型変数ならキーIを削除する。

# 🔸 配列切取 (AのIを/Aから)
#    配列AのI番目(0起点)の要素を切り取って返す。Aの内容を書き換える。引数Iには範囲オブジェクトを指定できる。その場合戻り値は配列型となる。辞書型変数ならキーIを削除する。

# 🔸 配列取出 (AのIからCNTを)
#    配列AのI番目(0起点)からCNT個の要素を取り出して返す。Aの内容を書き換える

# 🔸 配列ポップ (Aの/Aから)
#    配列Aの末尾を取り出して返す。Aの内容を書き換える。

# 🔸 配列プッシュ (AにBを/Aへ)
#    配列Aの末尾にNを追加。Aの内容を書き換える。(『配列追加』と同じ)

# 🔸 配列追加 (AにBを/Aへ)
#    配列Aの末尾にBを追加して返す。Aの内容を書き換える。

# 🔸 配列複製 (Aを)
#    配列Aを複製して返す。

# 🔸 配列範囲コピー (AのIを/Aから)
#    配列Aの範囲I(数値化範囲オブジェクト)を複製して返す。

# 🔸 参照 (AからIを/Aの)
#    値A(配列/文字列/辞書型)の範囲I(キーまたは範囲オブジェクト)を参照して(コピーせず)返す

# 🔸 配列参照 (AのIを/Aから)
#    値A(配列/文字列/辞書型)の範囲I(キーまたは範囲オブジェクト)を参照して(コピーせず)返す(『参照』と同じ)

# 🔸 配列足 (AにBを/Aへ/Aと)
#    配列Aに配列Bを足し合わせて返す。

# 🔸 配列最大値 (Aの)
#    配列Aの値の最大値を調べて返す。

# 🔸 配列最小値 (Aの)
#    配列Aの値の最小値を調べて返す。

# 🔸 配列合計 (Aの)
#    配列Aの値を全て足して返す。配列の各要素を数値に変換して計算する。数値に変換できない文字列は0になる。

# 🔸 配列入替 (AのIとJを)
#    配列Aの(0から数えて)I番目とJ番目の要素を入れ替えて返す。Aの内容を書き換える。

# 🔸 配列連番作成 (AからBまでの/Bまで/Bの)
#    AからBまでの連番配列を生成して返す。

# 🔸 配列要素作成 (AをBだけ)
#    値AをB個持つ配列を生成して返す。

# 🔸 配列関数適用 (FをAへ/Aに)
#    引数を1つ持つ関数Fを、配列Aの全要素に適用した、新しい配列を返す。

# 🔸 配列マップ (FをAへ/Aに)
#    引数を1つ持つ関数Fを、配列Aの全要素に適用した、新しい配列を返す。(『配列関数適用』と同じ)

# 🔸 配列フィルタ (FでAを/FのAについて)
#    引数を1つ持ち真偽を返す関数Fを利用して、配列Aの要素をフィルタして、新しい配列として返す。
```

### Two Dimensional Array Processing

**Functions:**

```nadesiko
# 🔸 表ソート (AのNOを)
#    二次元配列AでB列目(0起点)(あるいはキー名)をキーに文字列順にソートする。Aの内容を書き換える。

# 🔸 表数値ソート (AのNOを)
#    二次元配列AでB列目(0起点)(あるいはキー名)をキーに数値順にソートする。Aの内容を書き換える。

# 🔸 表ピックアップ (AのNOからSを/Sで)
#    配列Aの列番号B(0起点)(あるいはキー名)で検索文字列Sを含む行を返す

# 🔸 表完全一致ピックアップ (AのNOからSを/Sで)
#    配列Aの列番号B(0起点)(あるいはキー名)で検索文字列Sと一致する行を返す

# 🔸 表検索 (AのCOLでROWからSを/COLに)
#    二次元配列AでCOL列目(0起点)からキーSを含む行をROW行目から検索して何行目にあるか返す。見つからなければ-1を返す。

# 🔸 表列数 (Aの)
#    二次元配列Aの列数を調べて返す。

# 🔸 表行数 (Aの)
#    二次元配列Aの行数を調べて返す。

# 🔸 表行列交換 (Aの/Aを)
#    二次元配列Aの行と列を交換して返す。

# 🔸 表右回転 (Aの/Aを)
#    二次元配列Aを90度回転して返す。

# 🔸 表重複削除 (AのIを/Iで)
#    二次元配列AのI列目にある重複項目を削除して返す。

# 🔸 表列取得 (AのIを)
#    二次元配列AのI列目を返す。

# 🔸 表列挿入 (AのIにSを/Iへ)
#    二次元配列Aの(0から数えて)I列目に配列Sを挿入して返す

# 🔸 表列削除 (AのIを)
#    二次元配列Aの(0から数えて)I列目削除して返す

# 🔸 表列合計 (AのIを/Iで)
#    二次元配列Aの(0から数えて)I列目を合計して返す。

# 🔸 表曖昧検索 (AのROWからCOLでSを)
#    二次元配列AのROW行目からCOL列目(0起点)で正規表現Sにマッチする行を検索して何行目にあるか返す。見つからなければ-1を返す。(v1非互換)

# 🔸 表正規表現ピックアップ (AのCOLからSを/Aで)
#    二次元配列AでI列目(0起点)から正規表現パターンSにマッチする行をピックアップして返す。
```

### Dictionary Variable Operations

**Functions:**

```nadesiko
# 🔸 辞書キー列挙 (Aの)
#    辞書型変数Aのキーの一覧を配列で返す。

# 🔸 辞書キー削除 (AからKEYを/Aの)
#    辞書型変数AからキーKEYを削除して返す（A自体を変更する）。

# 🔸 辞書キー存在 (AのKEYが/Aに)
#    辞書型変数AのキーKEYが存在するか確認
```

## Patterns

### Regular Expressions

**Constants:**

```nadesiko
# 🔹 抽出文字列 - []
```

**Functions:**

```nadesiko
# 🔸 正規表現マッチ (AをBで/AがBに)
#    文字列Aを正規表現パターンBでマッチして結果を返す(パターンBは「/pat/opt」の形式で指定。optにgの指定がなければ部分マッチが『抽出文字列』に入る)

# 🔸 正規表現置換 (SのAをBで/AからBに/Bへ)
#    文字列Sの正規表現パターンAをBに置換して結果を返す(パターンAは/pat/optで指定)

# 🔸 正規表現区切 (SをAで)
#    文字列Sを正規表現パターンAで区切って配列で返す(パターンAは/pat/optで指定)
```

### Specified Format

**Functions:**

```nadesiko
# 🔸 通貨形式 (Vを/Vの)
#    数値Vを三桁ごとにカンマで区切る

# 🔸 ゼロ埋 (VをAで)
#    数値VをA桁の0で埋める

# 🔸 空白埋 (VをAで)
#    文字列VをA桁の空白で埋める
```

## I/O

### File Input Output

**Functions:**

```nadesiko
# 🔸 開 (Fを/Fから)
#    ファイルFを開く

# 🔸 読 (Fを/Fから)
#    ファイFSを開く

# 🔸 バイナリ読 (Sを/Sから)
#    ファイルSをバイナリ(Buffer)として開く

# 🔸 保存 (SをFへ/Fに)
#    データSをファイルFヘ書き込む(文字コードはUTF-8)(非同期関数)

# 🔸 SJISファイル読 (Sを/Sから)
#    SJIS形式のファイルSを読み込む

# 🔸 SJISファイル保存 (SをFへ/Fに)
#    SをSJIS形式でファイルFへ書き込む

# 🔸 EUCファイル読 (Sを/Sから)
#    euc-jp形式のファイルSを読み込む

# 🔸 EUCファイル保存 (SをFへ/Fに)
#    Sをeuc-jp形式でファイルFへ書き込む

# 🔸 起動待機 (Sを)
#    シェルコマンドSを起動し実行終了まで待機する

# 🔸 起動 (Sを)
#    シェルコマンドSを起動

# 🔸 起動時 (CALLBACKでSを)
#    シェルコマンドSを起動

# 🔸 ブラウザ起動 (URLを)
#    ブラウザでURLを起動

# 🔸 ファイル列挙 (Sの/Sを/Sで)
#    パスSのファイル名（フォルダ名）一覧を取得する。ワイルドカード可能。「*.jpg;*.png」など複数の拡張子を指定可能。

# 🔸 全ファイル列挙 (Sの/Sを/Sで)
#    パスS以下の全ファイル名を取得する。ワイルドカード可能。「*.jpg;*.png」のように複数の拡張子を指定可能。

# 🔸 存在 (PATHが/PATHの)
#    ファイルPATHが存在するか確認して返す

# 🔸 フォルダ存在 (PATHが/PATHの)
#    ディレクトリPATHが存在するか確認して返す

# 🔸 フォルダ作成 (PATHの/PATHを/PATHに/PATHへ)
#    ディレクトリPATHを作成して返す(再帰的に作成)

# 🔸 ファイルコピー (AからBに/AをBへ)
#    パスAをパスBへファイルコピーする

# 🔸 ファイルコピー時 (CALLBACKでAからBに/AをBへ)
#    パスAをパスBへファイルコピーしてcallbackを実行

# 🔸 ファイル移動 (AからBに/AをBへ)
#    パスAをパスBへ移動する

# 🔸 ファイル移動時 (CALLBACKでAからBに/AをBへ)
#    パスAをパスBへ移動してcallbackを実行

# 🔸 ファイル削除 (PATHの/PATHを)
#    パスPATHを削除する

# 🔸 ファイル削除時 (CALLBACKでPATHの/PATHを)
#    パスPATHを削除してcallbackを実行

# 🔸 ファイル情報取得 (PATHの/PATHから)
#    パスPATHの情報を調べてオブジェクトで返す

# 🔸 ファイルサイズ取得 (PATHの/PATHから)
#    パスPATHのファイルサイズを調べて返す
```

### Folder Acquisition

**Constants:**

```nadesiko
# 🔹 母艦パス - ''
```

**Functions:**

```nadesiko
# 🔸 カレントディレクトリ取得
#    カレントディレクトリを返す

# 🔸 カレントディレクトリ変更 (DIRに/DIRへ)
#    カレントディレクトリをDIRに変更する

# 🔸 作業フォルダ取得
#    カレントディレクトリを返す

# 🔸 作業フォルダ変更 (DIRに/DIRへ)
#    カレントディレクトリをDIRに変更する

# 🔸 ホームディレクトリ取得
#    ホームディレクトリを取得して返す

# 🔸 デスクトップ
#    デスクトップパスを取得して返す

# 🔸 マイドキュメント
#    マイドキュメントのパスを取得して返す

# 🔸 母艦パス取得
#    スクリプトのあるディレクトリを返す

# 🔸 テンポラリフォルダ
#    テンポラリフォルダのパスを取得して返す

# 🔸 一時フォルダ作成 (DIRに/DIRへ)
#    指定のフォルダに作業用の一時フォルダを作成して取得して返す
```

### CSV Operations

**Functions:**

```nadesiko
# 🔸 CSV取得 (STRを/STRの/STRで)
#    CSV形式のデータstrを強制的に二次元配列に変換して返す

# 🔸 TSV取得 (STRを/STRの/STRで)
#    TSV形式のデータstrを強制的に二次元配列に変換して返す

# 🔸 表CSV変換 (Aを)
#    二次元配列AをCSV形式に変換して返す

# 🔸 表TSV変換 (Aを)
#    二次元配列AをTSV形式に変換して返す

# 🔸 CSVオプション設定 (OBJ{ [KEY}を/OBJ{ [KEY}で)
#    「CSV取得」「表CSV変換」命令のオプションOBJ{delimiter,eol,auto_convert_number}をオブジェクトで指定
```

### JSON

**Functions:**

```nadesiko
# 🔸 JSONエンコード (Vを/Vの)
#    オブジェクトVをJSON形式にエンコードして返す

# 🔸 JSONエンコード整形 (Vを/Vの)
#    オブジェクトVをJSON形式にエンコードして整形して返す

# 🔸 JSONデコード (Sを/Sの/Sから)
#    JSON文字列Sをオブジェクトにデコードして返す

# 🔸 JSON_E (Vを/Vの)
#    オブジェクトVをJSON形式にエンコードして返す(JSONエンコードと同じ)

# 🔸 JSON_ES (Vを/Vの)
#    オブジェクトVをJSON形式にエンコードして整形して返す(JSONエンコード整形と同じ)

# 🔸 JSON_D (Sを/Sの/Sから)
#    JSON文字列Sをオブジェクトにデコードして返す(JSONデコードと同じ)
```

### BASE64

**Functions:**

```nadesiko
# 🔸 BASE64エンコード (TEXTを/TEXTから)
#    BASE64エンコードして返す

# 🔸 BASE64デコード (TEXTを/TEXTへ/TEXTに)
#    BASE64デコードして返す
```

### TOML

**Functions:**

```nadesiko
# 🔸 TOMLデコード (Sを/Sの/Sから)
#    TOML文字列をオブジェクトにデコードして返す

# 🔸 TOMLエンコード (Sを/Sから/Sの)
#    オブジェクトをTOML文字列にエンコードする
```

## Command Line

### Command Line and Standard Input Output

**Constants:**

```nadesiko
# 🔹 コマンドライン - ''
# 🔹 ナデシコランタイム - ''
# 🔹 ナデシコランタイムパス - ''
```

**Functions:**

```nadesiko
# 🔸 標準入力取得時 (CALLBACK(Fを)
#    標準入力を一行取得した時に、変数『対象』に取得した文字列を代入し、無名関数（あるいは、文字列で関数名を指定）F(s: string)を実行する

# 🔸 尋 (MSGと/MSGを)
#    標準入力を一行取得する(非同期関数)

# 🔸 文字尋 (MSGと/MSGを)
#    標準入力を一行取得する。ただし自動で数値に変換しない(非同期関数)

# 🔸 標準入力全取得
#    標準入力を全部取得して返す(非同期関数)
```

## Web/Browser

### DOM Operations

**Constants:**

```nadesiko
# 🔹 DOCUMENT - ''
# 🔹 WINDOW - ''
# 🔹 NAVIGATOR - ''
# 🔹 DOM和属性 - undefined
# 🔹 DOM和スタイル - undefined
# 🔹 DOMプロパティ情報 - undefined
```

**Functions:**

```nadesiko
# 🔸 DOM要素ID取得 (IDの/IDを)
#    DOMの要素をIDを指定して取得

# 🔸 DOM要素取得 (Qの/Qを)
#    DOMの要素をクエリqで取得して返す

# 🔸 DOM要素全取得 (Qの/Qを)
#    DOMの要素をクエリqで全部取得して返す

# 🔸 タグ一覧取得 (TAGの/TAGを)
#    任意のタグの一覧を取得して返す

# 🔸 DOM子要素取得 (PAのQを)
#    DOMの要素PAの子要素をクエリqを指定して結果を一つ取得して返す

# 🔸 DOM子要素全取得 (PAのQを)
#    DOMの要素PAの子要素をクエリqを指定して結果を複数取得して返す

# 🔸 DOMイベント設定 (DOMのEVENTにFUNCSTRを/EVENTへ)
#    DOMのEVENTになでしこ関数名funcStrのイベントを設定

# 🔸 DOMテキスト設定 (DOMにTEXTを/DOMの/DOMへ)
#    DOMにテキストを設定

# 🔸 DOMテキスト取得 (DOMの/DOMから)
#    DOMのテキストを取得

# 🔸 DOM_HTML設定 (DOMにTEXTを/DOMの/DOMへ)
#    DOMにHTML文字列を設定

# 🔸 DOM_HTML取得 (DOMの/DOMから)
#    DOMのHTML文字列を取得

# 🔸 テキスト設定 (DOMにVを/DOMの/DOMへ)
#    DOMのテキストにVを設定

# 🔸 テキスト取得 (DOMの/DOMから)
#    DOMのテキストを取得

# 🔸 HTML設定 (DOMにVを/DOMの/DOMへ)
#    DOMのHTMLにVを設定

# 🔸 HTML取得 (DOMの/DOMから)
#    DOMのテキストを取得

# 🔸 DOM属性設定 (DOMのSにVを/Sへ)
#    DOMの属性Sに値Vを設定(属性Sには『DOM和属性』も適用される)

# 🔸 DOM属性取得 (DOMのSを/DOMから)
#    DOMの属性Sを取得(属性Sには『DOM和属性』も適用される)

# 🔸 DOMスタイル設定 (DOMのSにVを/Sへ)
#    DOMのスタイルAに値Bを設定

# 🔸 DOMスタイル一括設定 (DOMにVALUESを/DOMへ)
#    DOMに(オブジェクト型で)スタイル情報を一括設定

# 🔸 DOMスタイル取得 (DOMのSTYLEを)
#    DOMのSTYLEの値を取得

# 🔸 DOMスタイル一括取得 (DOMのSTYLEを)
#    DOMのSTYLE(配列で複数指定)の値を取得

# 🔸 データ属性取得 (DOMのPROPを/DOMから)
#    DOMのdata-PROPの値を取得

# 🔸 データ属性設定 (DOMのPROPにVALを/PROPへ)
#    DOMのdata-PROPに値Vを設定

# 🔸 DOM設定変更 (DOMのPROPにVALUEを/PROPへ)
#    DOMの属性とスタイルPROP(配列で指定可能)を適当にVALUEに設定

# 🔸 DOM設定取得 (DOMのPROPを/DOMから)
#    DOMの属性とスタイルPROP(配列で指定可能)の値を適当に取得

# 🔸 DOM有効設定 (DOMにVALUEを/DOMへ)
#    DOMのdata-有効の値を設定

# 🔸 DOM有効取得 (DOMの/DOMから)
#    DOMのdata-有効の値を取得

# 🔸 DOM可視設定 (DOMにVALUEを/DOMへ)
#    DOMのdata-可視の値を設定

# 🔸 DOM可視取得 (DOMの/DOMから)
#    DOMのdata-可視の値を取得

# 🔸 ポケット取得 (DOMの/DOMから)
#    DOMのポケット(data-pocket属性)の値を取得(エンコードされるので辞書型や配列も取得できる)

# 🔸 DOMポケット取得 (DOMの/DOMから)
#    DOMのポケット(data-pocket属性)の値を取得(エンコードされるので辞書型や配列も取得できる)

# 🔸 ポケット設定 (DOMにVALを/DOMへ)
#    DOMのポケット(data-pocket属性)に値Vを設定(エンコードされるので辞書型や配列も設定できる)

# 🔸 DOMポケット設定 (DOMにVALを/DOMへ)
#    DOMのポケット(data-pocket属性)に値Vを設定(エンコードされるので辞書型や配列も設定できる)

# 🔸 ヒント取得 (DOMの/DOMから)
#    DOMのヒント(title属性)の値を取得

# 🔸 DOMヒント取得 (DOMの/DOMから)
#    DOMのヒント(title属性)の値を取得

# 🔸 ヒント設定 (DOMにVALを/DOMへ)
#    DOMのヒント(title属性)に値Vを設定

# 🔸 DOMヒント設定 (DOMにVALを/DOMへ)
#    DOMのヒント(title属性)に値Vを設定

# 🔸 DOM要素作成 (TAGの/TAGを)
#    DOMにTAGの新規要素を作成

# 🔸 DOM子要素追加 (PAにELを/PAへ)
#    DOMの要素PAの子へ要素ELを追加してPAを返す

# 🔸 DOM子要素削除 (PAからELを)
#    DOMの要素PAの子から要素ELを削除してPAを返す

# 🔸 注目 (DOMを/DOMへ/DOMに)
#    要素DOMにフォーカスする(カーソルを移動する)
```

### DOM Operations and Events

**Constants:**

```nadesiko
# 🔹 対象イベント - ''
# 🔹 押キー - ''
# 🔹 マウスX - 0
# 🔹 マウスY - 0
# 🔹 押ボタン - 0
# 🔹 マウスホイール値 - 0
# 🔹 タッチX - 0
# 🔹 タッチY - 0
# 🔹 タッチ配列 - []
```

**Functions:**

```nadesiko
# 🔸 DOMイベント追加 (DOMのEVENTにFUNCSTRを/EVENTへ)
#    DOMのEVENTになでしこ関数名funcStrのイベントを追加

# 🔸 DOMイベント削除 (DOMのEVENTからFUNCSTRを)
#    DOMのEVENTからなでしこ関数名funcStrのイベントを削除

# 🔸 DOMイベント発火時 (CALLBACKでDOMのEVENTが)
#    DOMのEVENTが発火した時にCALLBACKを実行するように設定

# 🔸 DOMイベント処理停止 (EVENTを/EVENTの)
#    キーイベントやマウスイベントで、元々ブラウザが行う処理を中止する

# 🔸 クリック時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMをクリックした時に実行するイベントを設定

# 🔸 ダブルクリック時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMをダブルクリックした時に実行するイベントを設定

# 🔸 右クリック時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMを右クリックした時に実行するイベント(contextmenu)を設定

# 🔸 変更時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMを変更した時に実行するイベントを設定

# 🔸 読込時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMを読み込んだ時に実行するイベントを設定

# 🔸 フォーム送信時 (FUNCでDOMを/DOMの)
#    無名関数Fでフォームを送信した時に実行するイベントを設定

# 🔸 キー押時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMに対してキーを押した時に実行するイベントを設定。『押されたキー』が設定される。

# 🔸 キー離時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMに対してキーを離した時に実行するイベントを設定。『押されたキー』が設定される。

# 🔸 キータイピング時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMに対してキーをプレスした時に実行するイベントを設定。『押されたキー』が設定される。

# 🔸 マウス押時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMに対してマウスボタンを押した時に実行するイベントを設定。『マウスX』『マウスY』に座標が、『押したボタン』に押したボタン(左,中央,右)が設定される。『対象』にイベントDOM。『対象イベント』にイベント引数。

# 🔸 マウス移動時 (FUNCでDOMを/DOMの/DOMへ/DOMに)
#    無名関数FでDOMに対してマウスカーソルが移動した時に実行するイベントを設定。『マウスX』『マウスY』に座標が設定される。『対象』にイベントDOM。『対象イベント』にイベント引数。

# 🔸 マウス離時 (FUNCでDOMを/DOMの/DOMから)
#    無名関数FでDOMに対してマウスボタンを離した時に実行するイベントを設定。『マウスX』『マウスY』に座標が、『押したボタン』に押したボタン(左,中央,右)が設定される。『対象』にイベントDOM。『対象イベント』にイベント引数。

# 🔸 マウス入時 (FUNCでDOMを/DOMの/DOMに/DOMへ)
#    無名関数FでDOMに対してマウスカーソルが入った時のイベントを設定。『マウスX』『マウスY』に座標が設定される。『対象』にイベントDOM。『対象イベント』にイベント引数。

# 🔸 マウス出時 (FUNCでDOMを/DOMの/DOMから)
#    無名関数FでDOMに対してマウスカーソルが出た時のイベントを設定。『マウスX』『マウスY』に座標が設定される。『対象』にイベントDOM。『対象イベント』にイベント引数。

# 🔸 マウスホイール時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMに対してマウスホイールを回した時のイベントを設定。『マウスホイール値』に値が設定される。『対象』にイベントDOM。『対象イベント』にイベント引数。

# 🔸 タッチイベント計算 (Eの)
#    タッチイベントで座標計算を行う。『タッチX』『タッチY』『タッチ配列』『対象』『対象イベント』が設定される。『タッチ配列』の内容が返る

# 🔸 タッチ開始時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMに対してタッチを開始した時に実行するイベントを設定。

# 🔸 タッチ時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMに対してタッチして指を動かした時に実行するイベントを設定。

# 🔸 タッチ終了時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMに対してタッチして指を離した時のイベントを設定。

# 🔸 タッチキャンセル時 (FUNCでDOMを/DOMの)
#    無名関数FでDOMに対してタッチイベントをキャンセルした時の動作を設定。

# 🔸 画面更新時実行 (FUNCを)
#    画面描画タイミングで関数F(文字列指定も可)を実行する。識別IDを返す。

# 🔸 画面更新処理取消 (IDの/IDを)
#    識別IDを指定して『画面更新時実行』を取り消す
```

### DOM Component Operations

**Constants:**

```nadesiko
# 🔹 DOM親要素 - ''
# 🔹 DOM部品個数 - 0
# 🔹 DOM部品オプション - { '自動改行': false, 'テーブルヘッダ': true, 'テーブル背景色': ['#AA4040', '#ffffff', '#fff0f0'], 'テーブル数値右寄せ': true }
# 🔹 DOMスキン - ''
# 🔹 DOMスキン辞書 - {}
```

**Functions:**

```nadesiko
# 🔸 DOM親要素設定 (ELに/ELへ)
#    「ボタン作成」「エディタ作成」など『DOM部品作成』で追加する要素の親要素を指定(デフォルトはdocument)して要素を返す。

# 🔸 DOM親部品設定 (ELに/ELへ)
#    DOM部品作成でDOM要素を追加する親の対象を指定。『DOM親要素設定』と同じ。

# 🔸 DOMスキン設定 (SKINを/SKINに/SKINの)
#    「ボタン作成」「エディタ作成」などで適用するスキンを指定する(#1033)

# 🔸 DOM部品作成 (ELMの)
#    elmの要素を作成して『DOM親要素設定』で指定した要素に追加して、DOMオブジェクトを返す。(elmがDOM要素なら追加する)

# 🔸 DOM部品削除 (ELMの/ELMを)
#    elmの要素を削除する

# 🔸 ボタン作成 (LABELの)
#    ラベルlabelを持つbutton要素を追加しDOMオブジェクトを返す

# 🔸 エディタ作成 (TEXTの)
#    textの値を持つテキストボックス(input[type='text'])の要素を追加しDOMオブジェクトを返す

# 🔸 テキストエリア作成 (TEXTの)
#    textの値を持つtextarea要素を追加しDOMオブジェクトを返す

# 🔸 ラベル作成 (TEXTの)
#    textの値を持つラベル(span要素)を追加しDOMオブジェクトを返す

# 🔸 キャンバス作成 (SIZEの)
#    大きさ[幅, 高]のcanvas要素を追加しDOMオブジェクトを返す

# 🔸 画像作成 (URLの/URLから)
#    URLを指定してimg要素を追加しDOMオブジェクトを返す

# 🔸 改行作成
#    改行(br要素)を追加しDOMオブジェクトを返す

# 🔸 チェックボックス作成 (TEXTの)
#    textのラベルを持つチェックボックス(input[type='checkbox'])要素を追加しDOMオブジェクトを返す

# 🔸 セレクトボックス作成 (OPTIONSの)
#    配列optionsの選択肢を持つselect要素を追加しDOMオブジェクトを返す

# 🔸 セレクトボックスアイテム設定 (OPTIONSをDOMへ/DOMに)
#    配列データをセレクトボックスdomのアイテムに差し替える

# 🔸 色選択ボックス作成
#    色選択ボックス(input[type='color'])を作成しDOMオブジェクトを返す

# 🔸 日付選択ボックス作成
#    日付選択ボックス(input[type='date'])を作成しDOMオブジェクトを返す

# 🔸 パスワード入力エディタ作成 (Sの/Sで)
#    パスワード入力エディタ(input[type='password'])を作成し初期値Sを設定し、DOMオブジェクトを返す

# 🔸 値指定バー作成 (RANGEの/RANGEで)
#    範囲RANGE(配列で[最小,最大[,値]])を指定するバー(input[type='range'])を作成しDOMオブジェクトを返す

# 🔸 送信ボタン作成 (LABELの)
#    ラベルSの送信ボタン(input[type='submit'])を作成しDOMオブジェクトを返す

# 🔸 フォーム作成 (OBJでSを/OBJの)
#    属性OBJ{method:"GET",action:"..."}で項目一覧S「項目1=初期値1{改行}項目2=初期値2{改行}…」を送信フォームを作成しDOMオブジェクトを返す。「=?」でオプションの指定が可能

# 🔸 フォーム入力一括取得 (DOMの/DOMから)
#    DOMのフォームを取得し、そのフォーム以下にある入力項目のnameとvalueを辞書形式で返す

# 🔸 テーブル作成 (AAの/AAから)
#    二次元配列AA(あるいは文字列の簡易CSVデータ)からTABLE要素を作成し、DOMオブジェクトを返す

# 🔸 ヘッダ無テーブル作成 (AAの/AAから)
#    二次元配列AA(あるいは文字列の簡易CSVデータ)からヘッダ無しのTABLE要素を作成し、DOMオブジェクトを返す

# 🔸 テーブル更新 (TBLをAAに/AAへ)
#    既に作成したテーブルTBLを二次元配列AA(あるいは文字列の簡易CSVデータ)で更新する

# 🔸 テーブルセル変更 (TのCELLをVに/Vへ)
#    TABLE要素のセル[行,列]をVへ変更する。Vが二次元配列変数であれば複数のセルを一括変更する

# 🔸 マーメイド作成 (SRCの)
#    Mermaid記法を使ってSRCのチャートを作成する(非同期関数)
```

### Drawing

**Constants:**

```nadesiko
# 🔹 描画中キャンバス - null
# 🔹 描画中コンテキスト - null
```

**Functions:**

```nadesiko
# 🔸 描画開始 (CVの/CVへ/CVで)
#    描画先にCanvas(文字列でクエリの指定も可)を指定して描画API(2D)の利用準備する

# 🔸 キャンバス状態保存
#    Canvasの状態を保存(save)

# 🔸 キャンバス状態復元
#    Canvasの状態を復元(restore)

# 🔸 線色設定 (Vに/Vへ)
#    Canvasの線の描画色(lineStyle)を指定する

# 🔸 塗色設定 (Vに/Vへ)
#    Canvasへの描画色(fillStyle)を指定する

# 🔸 線描画 (AからBへ/Bまで)
#    [x1, y1]から[x2, y2]まで線を描画する

# 🔸 線太設定 (Vに/Vへ)
#    vに線の太さ設定

# 🔸 四角描画 (Bの/Bへ/Bに)
#    [x, y, w, h]で矩形を描画する

# 🔸 全描画クリア
#    描画中のキャンバスをクリアする。

# 🔸 描画クリア (Bの/Bへ/Bに)
#    [x, y, w, h]の範囲を描画クリア。空配列を指定すると『全描画クリア』と同じ。2要素の配列だと[0,0]を省略したのと同じ。

# 🔸 円描画 (XYへRの/XYに)
#    [x, y]へrの円を描画する

# 🔸 楕円描画 (ARGSへ/ARGSに/ARGSの)
#    [x, y, x幅, y幅, 回転, 開始角, 終了角, 左回転か]に楕円を描画する

# 🔸 多角形描画 (Aで/Aの/Aを)
#    座標配列vを指定して多角形を描画する

# 🔸 画像読 (URLの/URLを)
#    画像のURLを読み込んでImageオブジェクトを返す。(URLにdataスキームも指定可能)

# 🔸 画像読待 (URLの/URLを)
#    画像のURLを読み込んでImageオブジェクトを返す。その際、画像の読み込みが終わるまで待つ。(非同期関数)

# 🔸 画像逐次読 (URLの/URLを)
#    (非推奨) 画像のURLを読み込んでImageオブジェクトを返す。また完了時『対象』にも代入する。『逐次実行』構文で使う。

# 🔸 画像読時 (FでURLの/URLを)
#    画像のURLを読み込んでコールバック関数Fを読み込み、変数『対象』にImageオブジェクトを代入する

# 🔸 画像描画 (IMGのXYへ/IMGをXYに)
#    画像IMG(またはURL)を描画先座標[x,y]へ描画し、Imageオブジェクトを返す。座標には2,4,8個の引数を指定可能。

# 🔸 画像部分描画 (IMGのSXYをDXYへ/SXYからDXYに)
#    画像IMG(またはURL)の座標[sx, sy, sw, sh]を描画先座標[dx, dy, dw, dh]へ描画し、Imageオブジェクトを返す

# 🔸 描画フォント設定 (Nを/Nの/Nで/Nに)
#    描画フォントを指定する(CSSのフォント設定と同じ 例「36px Aria」)。フォントサイズのみの指定も可。

# 🔸 文字描画 (XYへSの/XYにSを)
#    [x, y]へテキストSを描画する(描画フォント設定でサイズなど指定)

# 🔸 文字描画幅取得 (Sの)
#    テキストSを指定して文字の描画幅を取得する

# 🔸 描画起点設定 (XYへ/XYに)
#    描画位置の起点を[x,y]へ設定する(translate)

# 🔸 描画回転 (Aだけ/Aに/Aへ)
#    描画内容をA度だけ回転する(rotate)

# 🔸 描画拡大 (XYだけ/XYに/XYへ)
#    描画内容を[x方向,y方向]だけ拡大する(scale)

# 🔸 描画変換マトリクス設定 (Aだけ/Aに/Aへ)
#    描画内容を[a,b,c,d,e,f]の変換マトリクスに設定。既存内容を破棄して設定(setTransform)

# 🔸 描画変換マトリクス追加 (Aだけ/Aに/Aへ)
#    描画内容を[a,b,c,d,e,f]のマトリクスで変換。既存のマトリクスに掛け合わせる(transform)

# 🔸 描画データURL変換
#    描画内容をPNG形式のデータURLに変換して得る。

# 🔸 描画データBLOB変換
#    描画内容をPNG形式のBLOBオブジェクトに変換して戻す。(非同期関数)

# 🔸 描画ダウンロードリンク作成 (DOMへ/DOMに)
#    描画内容をPNG形式のデータURLに変換してDOMに設定する。

# 🔸 描画ダウンロード
#    描画内容をPNG形式のデータURLに変換してダウンロードする。(「クリックした時」などと組み合わせて使う)
```

### HTTP and AJAX

**Constants:**

```nadesiko
# 🔹 AJAXオプション - ''
```

**Functions:**

```nadesiko
# 🔸 HTTP取得 (URLの/URLから/URLを)
#    「AJAXテキスト取得」と同じ。非同期通信(AJAX)でURLからテキストデータを取得する。(非同期関数)

# 🔸 AJAX受信 (URLから/URLを)
#    「AJAXテキスト取得」と同じ。非同期通信(AJAX)でURLからテキストデータを取得する。(非同期関数)

# 🔸 AJAX受信時 (CALLBACKでURLから/URLを)
#    「AJAX送信時」と同じ。非同期通信(AJAX)を利用してURLからデータを受信した時callbackが実行される。その際『対象』にデータが代入される。『AJAXオプション』を指定できる。

# 🔸 AJAX送信 (URLまで/URLへ/URLに)
#    「AJAXテキスト取得」と同じ。非同期通信(AJAX)でURLからテキストデータを取得する。(非同期関数)

# 🔸 AJAX送信時 (CALLBACKのURLまで/URLへ/URLに)
#    非同期通信(AJAX)でURLにアクセスし成功するとCALLBACKを実行。『対象』にデータを代入。『AJAXオプション』が指定可能。エラーなら『AJAX失敗時』を実行。

# 🔸 AJAXオプション設定 (OPTIONに/OPTIONへ/OPTIONと)
#    AJAX命令でオプションを設定

# 🔸 AJAXオプションPOST設定 (PARAMSを/PARAMSで)
#    AJAXオプションにPOSTメソッドとパラメータPARAMSを設定

# 🔸 AJAX失敗時 (CALLBACKの)
#    AJAX命令でエラーが起きたとき

# 🔸 AJAXテキスト取得 (URLから/URLを)
#    AJAXでURLにアクセスしテキスト形式で結果を得る。送信時『AJAXオプション』の値を参照。(非同期関数)

# 🔸 AJAX_JSON取得 (URLから)
#    AJAXでURLにアクセスしJSONの結果を得て、送信時『AJAXオプション』の値を参照。(非同期関数)

# 🔸 AJAXバイナリ取得 (URLから)
#    AJAXでURLにアクセスしバイナリ(blob)形式で結果を得る。送信時『AJAXオプション』の値を参照。(非同期関数)
```

### New AJAX

**Functions:**

```nadesiko
# 🔸 AJAXテキスト取得 (URLから)
#    AJAXでURLにアクセスしテキスト形式で結果を得る。送信時AJAXオプションの値を参照。(非同期関数)

# 🔸 AJAX_JSON取得 (URLから)
#    AJAXでURLにアクセスしJSONの結果を得て、送信時AJAXオプションの値を参照。(非同期関数)

# 🔸 AJAXバイナリ取得 (URLから)
#    AJAXでURLにアクセスしバイナリ(arrayBuffer)形式で結果を得る。送信時AJAXオプションの値を参照。(非同期関数)
```

### Ajax

**Constants:**

```nadesiko
# 🔹 AJAXオプション - ''
```

**Functions:**

```nadesiko
# 🔸 AJAX送信時 (CALLBACKのURLまで/URLへ/URLに)
#    非同期通信(Ajax)でURLにデータを送信し、成功するとcallbackが実行される。その際『対象』にデータが代入される。

# 🔸 AJAX受信時 (CALLBACKでURLから/URLを)
#    非同期通信(Ajax)でURLにデータを送信し、成功するとcallbackが実行される。その際『対象』にデータが代入される。

# 🔸 GET送信時 (CALLBACKのURLまで/URLへ/URLに)
#    非同期通信(Ajax)でURLにデータを送信し、成功するとcallbackが実行される。その際『対象』にデータが代入される。

# 🔸 POST送信時 (CALLBACKのURLまでPARAMSを/URLへ/URLに)
#    AjaxでURLにPARAMSをPOST送信し『対象』にデータを設定

# 🔸 POSTフォーム送信時 (CALLBACKのURLまでPARAMSを/URLへ/URLに)
#    AjaxでURLにPARAMSをフォームとしてPOST送信し『対象』にデータを設定

# 🔸 AJAX失敗時 (CALLBACKの)
#    Ajax命令でエラーが起きたとき

# 🔸 AJAXオプション設定 (OPTIONに/OPTIONへ/OPTIONと)
#    Ajax命令でオプションを設定

# 🔸 AJAX保障送信 (URLまで/URLへ/URLに)
#    非同期通信(Ajax)でURLにデータの送信を開始する非同期処理オブジェクト(Promise)を作成する。

# 🔸 HTTP保障取得 (URLの/URLから/URLを)
#    非同期通信(Ajax)でURLにデータの送信を開始する非同期処理オブジェクト(Promise)を作成する。

# 🔸 GET保障送信 (URLまで/URLへ/URLに)
#    非同期通信(Ajax)でURLにデータの送信を開始する非同期処理オブジェクト(Promise)を作成する。

# 🔸 POST保障送信 (URLまでPARAMSを/URLへ/URLに)
#    非同期通信(Ajax)でURLにPARAMSをPOST送信を開始する非同期処理オブジェクト(Promise)を作成する。

# 🔸 POSTフォーム保障送信 (URLまでPARAMSを/URLへ/URLに)
#    非同期通信(Ajax)でURLにPARAMSをフォームとしてPOST送信を開始する非同期処理オブジェクト(Promise)を作成する。

# 🔸 AJAX内容取得 (RESからTYPEで)
#    非同期通信(Ajax)の応答から内容を指定した形式で取り出すための非同期処理オブジェクト(Promise)を返す。

# 🔸 AJAX受信 (URLから/URLを)
#    「!非同期モード」で非同期通信(Ajax)でURLからデータを受信する。『AJAXオプション』を指定できる。結果は変数『対象』に入る

# 🔸 POSTデータ生成 (PARAMSの/PARAMSを)
#    辞書形式のデータPARAMSをkey=value&key=value...の形式に変換する

# 🔸 POST送信 (URLまでPARAMSを/URLへ/URLに)
#    非同期通信(AJAX)でPOSTメソッドにてURLへPARAMS(辞書型)を送信して応答を戻す。(非同期関数)

# 🔸 POSTフォーム送信 (URLまでPARAMSを/URLへ/URLに)
#    非同期通信(AJAX)でURLにPARAMS(辞書型)をフォームとしてPOSTメソッドにてURLへ送信し応答を返す。(非同期関数)
```

### Local Storage

**Constants:**

```nadesiko
# 🔹 保存オプション - 'json'
```

**Functions:**

```nadesiko
# 🔸 保存 (VをKEYに/KEYへ)
#    ブラウザのlocalStorageのキーKに文字列Vを保存

# 🔸 開 (KEYを/KEYから/KEYの)
#    ブラウザのlocalStorageからVを読む

# 🔸 読 (KEYを/KEYから/KEYの)
#    ブラウザのlocalStorageからVを読む

# 🔸 存在 (KEYが)
#    ブラウザのlocalStorageにKEYが存在しているか調べる

# 🔸 ローカルストレージ保存 (VをKEYに/KEYへ)
#    ブラウザのlocalStorageのKにVを保存

# 🔸 ローカルストレージ読 (KEYを/KEYから/KEYの)
#    ブラウザのlocalStorageからVを読む

# 🔸 ローカルストレージキー列挙
#    ブラウザのlocalStorageのキー一覧を返す

# 🔸 ローカルストレージキー削除 (KEYを/KEYの)
#    ブラウザのlocalStorageのkeyを削除

# 🔸 ローカルストレージ全削除
#    ブラウザのlocalStorageのデータを全部削除する

# 🔸 ローカルストレージ有効確認
#    ブラウザのlocalStorageが使えるか確認

# 🔸 保存オプション設定 (Vに/Vへ)
#    ブラウザのlocalStorageへの保存オプション「json」または「raw」を設定する
```

### Blob

**Functions:**

```nadesiko
# 🔸 BLOB作成 (DATAをOPTIONSで/DATAから)
#    DATA(配列型)をOPTIONS(辞書型)でBlobオブジェクトを作成する。
```

### Clipboard Operations

**Functions:**

```nadesiko
# 🔸 クリップボード取得
#    クリップボードを取得する

# 🔸 クリップボード設定 (Vを/Vの)
#    クリップボードを設定する
```

### Audio

**Functions:**

```nadesiko
# 🔸 オーディオ開 (URLを/URLの)
#    オーディオファイルのURLを指定して、オーディオを読み込み、Audioオブジェクトを返す

# 🔸 オーディオ再生 (OBJを)
#    AudioオブジェクトOBJを指定してオーディオを再生

# 🔸 オーディオループ再生 (OBJを)
#    AudioオブジェクトOBJを指定してオーディオをループ再生する

# 🔸 オーディオ停止 (OBJを)
#    AudioオブジェクトOBJを指定してオーディオを停止

# 🔸 オーディオ一時停止 (OBJを)
#    AudioオブジェクトOBJを指定してオーディオを一時停止

# 🔸 オーディオ音量取得 (OBJの/OBJから)
#    AudioオブジェクトOBJの音量を取得して返す

# 🔸 オーディオ音量設定 (OBJをVに/Vへ)
#    AudioオブジェクトOBJの音量をV(0-1)に設定する

# 🔸 オーディオ長取得 (OBJの/OBJから)
#    AudioオブジェクトOBJを指定してオーディオの長さを取得して返す

# 🔸 オーディオ再生位置取得 (OBJの/OBJから)
#    AudioオブジェクトOBJを指定してオーディオの再生位置を取得して返す

# 🔸 オーディオ再生位置設定 (OBJをVに/Vへ)
#    AudioオブジェクトOBJを指定してオーディオの位置を数値Vで設定する
```

## Server/Network

### HTTP Server (Express)

**Constants:**

```nadesiko
# 🔹 GETデータ - ''
# 🔹 POSTデータ - ''
```

**Functions:**

```nadesiko
# 🔸 WEBサーバ名前設定 (NAMEに/NAMEへ)
#    Webサーバの名前を変更する

# 🔸 WEBサーバ起動 (PORTNOの/PORTNOで)
#    ポートPORTNOでWebサーバを起動して成功したら『WEBサーバ起動成功した時』を実行する

# 🔸 WEBサーバ起動時 (CALLBACKをPORTNOの/PORTNOで)
#    ポートPORTNOでWebサーバを起動して成功したらCALLBACKを実行する

# 🔸 WEBサーバ起動成功時 (CALLBACKを)
#    WEBサーバ起動が成功した時にcallbackを実行

# 🔸 WEBサーバ起動失敗時 (CALLBACKを)
#    WEBサーバ起動が失敗した時にcallbackを実行

# 🔸 WEBサーバ静的パス指定 (URLをPATHに/PATHへ)
#    サーバのHTMLや画像などを配置する静的パスを指定する

# 🔸 WEBサーバGET時 (CALLBACKをURIに/URIへ)
#    URIにGETメソッドがあった時の処理を指定

# 🔸 WEBサーバPOST時 (CALLBACKをURIに/URIへ)
#    URIにPOSTメソッドがあった時の処理を指定

# 🔸 WEBサーバPUT時 (CALLBACKをURIに/URIへ)
#    URIにPOSTメソッドがあった時の処理を指定

# 🔸 WEBサーバDELETE時 (CALLBACKをURIに/URIへ)
#    URIにPOSTメソッドがあった時の処理を指定

# 🔸 WEBサーバヘッダ出力 (OBJを/OBJの)
#    クライアントにヘッダOBJを出力

# 🔸 WEBサーバステータス出力 (NOを/NOの)
#    クライアントにステータスNOを出力

# 🔸 WEBサーバ出力 (Sを/Sと)
#    クライアントにSを出力

# 🔸 WEBサーバリダイレクト (URLへ/URLに)
#    URLにリダイレクトする
```

### WebSocket

**Functions:**

```nadesiko
# 🔸 WS接続完了時 (CALLBACKを)
#    WebSocketでサーバに接続完了した時に実行されるイベントを指定

# 🔸 WS受信時 (CALLBACKを)
#    WebSocketでサーバからメッセージを受信した時に実行されるイベントを指定

# 🔸 WSエラー発生時 (CALLBACKを)
#    WebSocketでエラーが発生した時に実行されるイベントを指定

# 🔸 WS接続 (Sに/Sへ/Sの)
#    WebSocketサーバsに接続する

# 🔸 WS送信 (Sを/Sと)
#    アクティブなWebSocketへsを送信する

# 🔸 WS切断
#    アクティブなWebSocketを閉じる
```

### WebSocket Server

**Constants:**

```nadesiko
# 🔹 WSサーバ相手 - ''
```

**Functions:**

```nadesiko
# 🔸 WSサーバ起動 (PORTNOの/PORTNOで)
#    ポートPORTNOでサーバを起動して成功したら『WSサーバ起動成功した時』を実行する

# 🔸 WSSサーバ起動 (CONFの/CONFで)
#    設定CONF{cert:サーバ証明書,key:キーファイル,port:ポート番号}を指定してWSSサーバを起動して成功したら『WSサーバ起動成功した時』を実行する

# 🔸 WSサーバ起動成功時 (CALLBACKを)
#    WSサーバ起動が成功した時にcallbackを実行

# 🔸 WSサーバ起動失敗時 (CALLBACKを)
#    WSサーバ起動が失敗した時にcallbackを実行

# 🔸 WSサーバ接続時 (CALLBACKを)
#    WSサーバにクライアントが接続してきた時callbackを実行。接続情報は、変数『対象』に入る

# 🔸 WSサーバ受信時 (CALLBACKで)
#    WSサーバでメッセージを受信した時に実行される。クライアントのIPアドレスとポートは『WSサーバー相手』に受信データは『対象』に代入される

# 🔸 WSサーバ全送信 (Sを)
#    WSサーバで全員にメッセージSを送信する

# 🔸 WSサーバ個別送信 (Sを)
#    WSサーバで個別にメッセージSを送信する

# 🔸 WSクライアント一覧取得 (Sを)
#    WSサーバに接続しているクライアントの一覧を返す
```

### SMTP

**Functions:**

```nadesiko
# 🔸 メール送信 (DATAの/DATAで)
#    辞書型のデータ{host:'xxx',port:xxx,secure:true,auth:{user:'xxx',pass:'xxx'},from:'xxx',to:'xxx',subject:'xxx',text:'xxx',html:'xxx'}を指定してメールを送信して情報を返す(非同期関数)

# 🔸 GMAIL送信 (DATAの/DATAで)
#    辞書型のデータ{user:'xxx',pass:'xxx',宛先:'xxx',件名:'xxx',本文:'xxx',html:'xxx',添付:[{filename:'xxx', path:'xxx'}]}を指定してGMAILからメール送信して情報を返す(非同期関数)
```

### LINE

**Functions:**

```nadesiko
# 🔸 LINE送信 (TOKENへMESSAGEを/TOKENに)
#    LINEにメッセージを送信する。先にLINE Notifyのページで宛先のトークンを取得する。TOKENへMESSAGEをLINE送信する。(非同期関数)

# 🔸 LINE画像送信 (TOKENへIMAGEFILEとMESSAGEを/TOKENに)
#    LINEにメッセージを送信する。先にLINE Notifyのページで宛先のトークンを取得する。TOKENへIMAGE_FILEとMESSAGEをLINE画像送信する。(非同期関数)
```

## Data

### Hash Functions

**Functions:**

```nadesiko
# 🔸 ハッシュ値計算時 (FUNCへSをALGで)
#    データSをアルゴリズムALG(sha-256/sha-384/sha-512)のエンコーディングでハッシュ値を計算して変数「対象」に代入する。

# 🔸 ハッシュ値計算 (SをALGで)
#    データSをアルゴリズムALG(sha-256/sha-384/sha-512)のエンコーディングでハッシュ値を計算して返す(非同期関数)

# 🔸 ランダムUUID生成
#    ランダムに生成された36文字のv4 UUID(文字列)を返す

# 🔸 ランダム配列生成 (CNTの)
#    暗号強度の強い乱数のバイト配列(Uint8Array)を指定の長さで返す

# 🔸 ハッシュ関数一覧取得
#    利用可能なハッシュ関数の一覧を返す

# 🔸 ハッシュ値計算 (SをALGのENCで)
#    データSをアルゴリズムALG(sha256/sha512/md5)のエンコーディングENC(hex/base64)でハッシュ値を計算して返す

# 🔸 ランダムUUID生成
#    ランダムに生成された36文字のv4 UUID(文字列)を返す

# 🔸 ランダム配列生成 (CNTの)
#    暗号強度の強い乱数のバイト配列(Uint8Array)を指定個数返す
```

### URL Encoding and Parameters

**Functions:**

```nadesiko
# 🔸 URLエンコード (TEXTを/TEXTから)
#    URLエンコードして返す

# 🔸 URLデコード (TEXTを/TEXTへ/TEXTに)
#    URLデコードして返す

# 🔸 URLパラメータ解析 (URLを/URLの/URLから)
#    URLパラメータを解析してハッシュで返す
```

### Compression and Decompression

**Constants:**

```nadesiko
# 🔹 圧縮解凍ツールパス - '7z'
```

**Functions:**

```nadesiko
# 🔸 圧縮解凍ツールパス変更 (Vに/Vへ)
#    圧縮解凍に使うツールを取得変更する

# 🔸 解凍 (AをBに/AからBへ)
#    (v1非互換)ZIPファイルAをBに解凍(実行には7-Zipが必要-https://7-zip.opensource.jp/ )

# 🔸 解凍時 (CALLBACKでAをBに/AからBへ)
#    解凍処理を行い、処理が完了したときにcallback処理を実行

# 🔸 圧縮 (AをBに/AからBへ)
#    (v1非互換)ファイルAをBにZIP圧縮(実行には7-Zipが必要-https://7-zip.opensource.jp/ )

# 🔸 圧縮時 (CALLBACKでAをBに/AからBへ)
#    圧縮処理を行い完了したときにcallback処理を指定
```

## Database

### SQLite3

**Constants:**

```nadesiko
# 🔹 SQLITE3今挿入ID - '?'
```

**Functions:**

```nadesiko
# 🔸 SQLITE3開 (Sを/Sの)
#    SQlite3のデータベースを開いて、データベースオブジェクトを返す

# 🔸 SQLITE3閉
#    アクティブなSQlite3のデータベースを閉じる

# 🔸 SQLITE3切替 (DBに/DBへ)
#    アクティブなSQlite3のデータベースをDB(SQLITE3開くで開いたもの)に切り替える

# 🔸 SQLITE3実行時 (FにSQLをPARAMSで)
#    SQLをパラメータPARAMSで実行する。完了するとコールバック関数Fを実行する。

# 🔸 SQLITE3実行後 (FにSQLをPARAMSで)
#    『SQLITE3実行時』と同じ。

# 🔸 SQLITE3取得時 (FにSQLをPARAMSで)
#    SQLをパラメータPARAMSで取得実行する。完了するとコールバック関数Fが実行され、結果は第一引数に与えられる。

# 🔸 SQLITE3実行 (SQLをPARAMSで)
#    SQLをパラメータPARAMSで実行する。(非同期関数)

# 🔸 SQLITE3取得 (SQLをPARAMSで)
#    SQLをパラメータPARAMSで取得する。(非同期関数)

# 🔸 SQLITE3全取得 (SQLをPARAMSで)
#    SQLをパラメータPARAMSで全部取得する。(非同期関数)
```

### MySQL

**Functions:**

```nadesiko
# 🔸 MYSQL開 (Sを/Sの/Sで)
#    データベースを開く

# 🔸 MYSQL閉
#    データベースを閉じる

# 🔸 MYSQL逐次実行 (SQLをPARAMSで)
#    逐次実行構文にて、SQLとパラメータPARAMSでSQLを実行し、変数『対象』に結果を得る。INSERT句の場合は『対象[insertId]』でIDが得られる。
```

### PostgreSQL

**Functions:**

```nadesiko
# 🔸 PG開 (Sを/Sの/Sで)
#    データベースを開く

# 🔸 PG閉
#    データベースを閉じる

# 🔸 PG実行 (SQLをPARAMSで)
#    SQLとパラメータPARAMSでSQLを実行し、戻り値に結果を得る。(非同期関数)

# 🔸 PG逐次実行 (SQLをPARAMSで)
#    (非推奨) 逐次実行構文にて、SQLとパラメータPARAMSでSQLを実行し、変数『対象』に結果を得る。SELECT句以外を実行した時も情報が『対象』に入る。
```

### SQLServer

**Functions:**

```nadesiko
# 🔸 MSSQL逐次開 (Sを/Sの/Sで)
#    逐次実行構文にてデータベースを開く

# 🔸 MSSQL逐次実行 (SQLをPARAMSで)
#    逐次実行構文にて、SQLとパラメータPARAMSでSQLを実行し、変数『対象』に結果を得る。

# 🔸 MSSQL逐次閉
#    開いているデータベースを閉じる
```

### ODBC

**Functions:**

```nadesiko
# 🔸 ODBC逐次開 (Sを/Sの/Sで)
#    逐次実行構文にて、ODBCのデータベースを開く

# 🔸 ODBC開 (Sを/Sの/Sで)
#    ODBCのデータベースを同期的に開いてオブジェクトを返す

# 🔸 ODBC逐次実行 (SQLをPARAMSで)
#    逐次実行構文にて、SQLとパラメータPARAMSでSQLを実行し、変数『対象』に結果を得る。

# 🔸 ODBC実行 (SQLをPARAMSで)
#    逐次実行構文内で、SQLとパラメータPARAMSでSQLを実行して結果を得る。

# 🔸 ODBC閉
#    ODBCで開いているデータベースを閉じる

# 🔸 ODBC逐次閉
#    逐次実行構文でODBCで開いているデータベースを閉じる

# 🔸 ODBCトランザクション開始
#    ODBCでトランザクションを開始する

# 🔸 ODBCトランザクション終了
#    ODBCでトランザクションを終了する
```

### KUDB

**Functions:**

```nadesiko
# 🔸 KUDB接続 (DBFILEに/DBFILEへ/DBFILEの)
#    簡易ドキュメントデータベースKUDBに接続する。DBにはファイルパスを指定する。

# 🔸 KUDB全取得
#    KUDBに挿入したドキュメントを全部返す

# 🔸 KUDB部分取得 (INDEXからCOUNTだけ/COUNTを)
#    KUDBの(0起点)INDEXからCOUNT件だけ取得

# 🔸 KUDB末尾取得 (INDEXからCOUNTだけ/COUNTを)
#    KUDBの(0起点)末尾から数えてINDEXからCOUNT件取得

# 🔸 KUDB挿入 (Vを)
#    KUDBにオブジェクトVを挿入する(TAGプロパティを指定すると検索などに使える)

# 🔸 KUDB更新 (IDをVに/Vへ)
#    KUDBのIDをVに更新

# 🔸 KUDB削除 (IDを)
#    KUDBのIDを削除する

# 🔸 KUDBタグ検索 (TAGの/TAGを)
#    KUDBでデータ一覧からTAGプロパティを検索する

# 🔸 KUDBタグ削除 (TAGの/TAGを)
#    KUDBでTAGを指定して削除

# 🔸 KUDBタグ更新 (TAGをVに/Vへ)
#    KUDBで指定TAGの内容をVに更新
```

## Office

### Excel

**Functions:**

```nadesiko
# 🔸 エクセル新規ブック
#    Excelの新規ワークブックを生成してオブジェクトを返す

# 🔸 エクセル開 (FILEを/FILEの/FILEから)
#    ファイルFILEからExcelワークブックを読んで返す(非同期関数)

# 🔸 エクセル保存 (FILEへ/FILEに)
#    ファイルFILEへ作業中のExcelワークブックを保存する(非同期関数)

# 🔸 エクセルCSV保存 (FILEへ/FILEに)
#    ファイルFILEへ作業中のExcelワークブックをCSVで保存する(ただしUTF-8のCSVとなる)(非同期関数)

# 🔸 エクセル新規シート (NAMEの/NAMEで)
#    Excelの作業中のワークブックに新規シートNAMEを追加して返す

# 🔸 エクセルシート取得 (NAMEの)
#    NAMEのシートを取得して返す

# 🔸 エクセルシート注目 (NAMEの/NAMEに/NAMEを)
#    NAMEのシートを取得して返す

# 🔸 エクセルセル設定 (CELLへVを/CELLに)
#    セル(例えば「A1」)へVを設定する

# 🔸 エクセル設定 (CELLへVを/CELLに)
#    セル(例えば「A1」)へVを設定する

# 🔸 エクセル一括設定 (CELLへVALUESを/CELLに)
#    左上のセル(例えば「A1」)を起点にして、二次元配列変数VALUESを一括設定する

# 🔸 エクセルセル取得 (CELLから/CELLを/CELLの)
#    セル(例えば「A1」)の値を取得して返す

# 🔸 エクセル取得 (CELLから/CELLを/CELLの)
#    セル(例えば「A1」)の値を取得して返す

# 🔸 エクセル一括取得 (C1からC2までの/C2まで/C2の)
#    左上のセルC1(例えば「A1」)から右下のC2までの値を取得して二次元配列変数で返す

# 🔸 エクセルシート列挙
#    作業中のブックのシート一覧取得して返す

# 🔸 エクセルシート削除 (NAMEの/NAMEを)
#    作業中のブックのシートNAMEを削除する

# 🔸 エクセルセル幅設定 (COLをWに/Wへ)
#    作業中のシートcol列目の幅をWに設定する

# 🔸 エクセル背景色設定 (CELLSをCOLORに/COLORへ)
#    作業中シートのセルcells(例「A1」「A1:C3」)の背景色をcolorに設定

# 🔸 エクセル文字色設定 (CELLSをCOLORに/COLORへ)
#    作業中シートのセルcells(例「A1」「A1:C3」)の文字色をcolorに設定
```

## Graphics

### Turtle Graphics

**Constants:**

```nadesiko
# 🔹 カメ速度 - 100
```

**Functions:**

```nadesiko
# 🔸 カメ作成
#    タートルグラフィックスを開始してカメのIDを返す

# 🔸 ゾウ作成
#    ゾウの画像でタートルグラフィックスを開始してIDを返す

# 🔸 パンダ作成
#    パンダの画像でタートルグラフィックスを開始してIDを返す

# 🔸 カメ操作対象設定 (IDに/IDへ/IDの)
#    IDを指定して操作対象となるカメを変更する

# 🔸 カメ画像変更 (URLに/URLへ)
#    カメの画像をURLに変更する

# 🔸 カメ速度設定 (Vに/Vへ)
#    カメの動作速度vに設定(大きいほど遅い)

# 🔸 カメ移動 (XYに/XYへ)
#    カメの位置を[x,y]へ移動する

# 🔸 カメ起点移動 (XYに/XYへ)
#    カメの描画起点位置を[x,y]へ移動する

# 🔸 カメ進 (Vだけ)
#    カメの位置をVだけ進める

# 🔸 カメ戻 (Vだけ)
#    カメの位置をVだけ戻す

# 🔸 カメ角度設定 (Vに/Vへ/Vの)
#    カメの向きをDEGに設定する

# 🔸 カメ右回転 (Vだけ)
#    カメの向きをDEGだけ右に向ける

# 🔸 カメ左回転 (Vだけ)
#    カメの向きをDEGだけ左に向ける

# 🔸 カメペン色設定 (Cに/Cへ)
#    カメのペン描画色をCに設定する

# 🔸 カメペンサイズ設定 (Wに/Wへ)
#    カメペンのサイズをWに設定する

# 🔸 カメペン設定 (Wに/Wへ)
#    カメペンを使うかどうかをV(オン/オフ)に設定する

# 🔸 カメパス開始
#    カメで明示的にパスの描画を開始する

# 🔸 カメパス閉
#    カメでパスを明示的に閉じる(省略可能)

# 🔸 カメパス線引
#    カメでパスを閉じて、カメペン色設定で指定した色で枠線を引く

# 🔸 カメパス塗
#    カメでパスを閉じて、カメ塗り色設定で指定した色で塗りつぶす

# 🔸 カメ文字描画 (Sを/Sと/Sの)
#    カメの位置に文字Sを描画

# 🔸 カメ文字設定 (Sに/Sへ/Sで)
#    カメ文字描画で描画するテキストサイズやフォント(48px serif)などを設定

# 🔸 カメ塗色設定 (Cに/Cへ)
#    カメパスの塗り色をCに設定する

# 🔸 カメ全消去
#    表示しているカメと描画内容を全部消去する

# 🔸 カメコマンド実行 (CMDの/CMDを)
#    カメにコマンドSを実行する。コマンドは改行か「;」で区切る。コマンドと引数は「=」で区切り引数はかカンマで区切る

# 🔸 カメ非表示
#    カメの画像を非表示にする。描画に影響しない。

# 🔸 カメ表示
#    非表示にしたカメを表示する。

# 🔸 カメクリック時 (FUNCを)
#    操作対象のカメをクリックした時のイベントを設定する
```

### 3D Turtle Graphics Basic Functions

**Functions:**

```nadesiko
# 🔸 T3D描画準備 (TOに/TOへ)
#    指定したDOMのIDに対する描画を準備し、描画オブジェクトを返す

# 🔸 T3D描画
#    現在の状態を描画する

# 🔸 T3D上書描画
#    現在の状態を元イメージをクリアせずに描画する

# 🔸 T3D実行
#    各カメの動きを経過時間等に従い実行する

# 🔸 T3D背景色設定 (Cに/Cへ)
#    canvasをクリアする際の背景色を設定する

# 🔸 T3D背景透過設定 (Aに/Aへ)
#    canvasをクリアする際の背景のアルファ値を設定する

# 🔸 T3DJSON取得
#    描画した線のJSON形式で取得する

# 🔸 T3Dレンダラ破棄
#    内部で使用しているレンダラを捨てる

# 🔸 T3D内部レンダラ取得
#    本プラグイン内部で使用しているレンダラを返す

# 🔸 T3D内部シーン取得
#    本プラグイン内部で使用しているシーンを返す

# 🔸 T3D内部カメラ取得
#    本プラグイン内部で使用しているカメラを返す

# 🔸 T3D内部線描画参照取得
#    本プラグイン内部で保持している描いた線のデータの参照を返す

# 🔸 T3D内部線描画取出
#    本プラグイン内部で保持している描いた線のデータを取り出して返す

# 🔸 T3D待 (Pを)
#    Promiseの終了を待って結果を返す(非同期関数)
```

### 3D Turtle Graphics Turtle Operations

**Constants:**

```nadesiko
# 🔹 T3Dカメ速度 - 100
```

**Functions:**

```nadesiko
# 🔸 T3Dカメ作成
#    タートルグラフィックスを開始してカメのIDを返す

# 🔸 T3Dカメ操作対象設定 (IDに/IDへ/IDの)
#    IDを指定して操作対象となるカメを変更する

# 🔸 T3Dカメモデル変更 (URLに/URLへ)
#    カメのモデルをURLに変更する

# 🔸 T3Dカメ速度設定 (Vに/Vへ)
#    カメの動作速度Vに設定(大きいほど遅い)

# 🔸 T3Dカメ移動 (XYZに/XYZへ)
#    カメの位置を[x,y,z]へ移動する

# 🔸 T3Dカメ原点設定
#    カメの原点を現在の位置・向きに設定する

# 🔸 T3Dカメ原点移動
#    カメを原点の位置・向きに移動する(描画はしない)

# 🔸 T3Dカメ起点移動 (XYZに/XYZへ)
#    カメの描画起点位置を[x,y,z]へ移動する

# 🔸 T3Dカメ進 (Lだけ)
#    カメの位置をLだけ進める

# 🔸 T3Dカメ戻 (Lだけ)
#    カメの位置をLだけ戻す

# 🔸 T3Dカメ上平行移動 (Lだけ)
#    カメの位置を上にLだけ進める

# 🔸 T3Dカメ下平行移動 (Lだけ)
#    カメの位置を下にLだけ進める

# 🔸 T3Dカメ左平行移動 (Lだけ)
#    カメの位置を左にLだけ進める

# 🔸 T3Dカメ右平行移動 (Lだけ)
#    カメの位置を右にLだけ進める

# 🔸 T3Dカメ動 (DIRへLだけ/DIRに)
#    カメの位置をDIRにLだけ進める

# 🔸 T3Dカメ角度設定 (ANGLEに/ANGLEへ/ANGLEの)
#    カメの向きをオイラー([x,y,z,XYZ])にて設定する

# 🔸 T3Dカメ右回転 (Aだけ)
#    カメの向きをAだけ右に向ける

# 🔸 T3Dカメ左回転 (Aだけ)
#    カメの向きをAだけ左に向ける

# 🔸 T3Dカメ上回転 (Aだけ)
#    カメの向きをAだけ上に向ける

# 🔸 T3Dカメ下回転 (Aだけ)
#    カメの向きをAだけ下に向ける

# 🔸 T3Dカメ回転 (DIRへAだけ/DIRに)
#    カメの向きをAだけDIRに向ける

# 🔸 T3Dカメ右ロール (Aだけ)
#    カメをAだけ右に傾ける

# 🔸 T3Dカメ左ロール (Aだけ)
#    カメのAだけ左に傾ける

# 🔸 T3Dカメ傾 (DIRにAだけ/DIRへ)
#    カメをAだけDIRに傾ける

# 🔸 T3Dカメペン色設定 (Cに/Cへ)
#    カメのペン描画色をCに設定する

# 🔸 T3Dカメペンサイズ設定 (Wに/Wへ)
#    カメペンのサイズをWに設定する

# 🔸 T3Dカメペン設定 (Wに/Wへ)
#    カメペンを使うかどうかをV(オン/オフ)に設定する

# 🔸 T3Dカメ全消去
#    表示しているカメと描画内容を全部消去する

# 🔸 T3Dカメ非表示
#    カメのモデルを非表示にする。描画に影響しない。

# 🔸 T3Dカメ表示
#    非表示にしたカメのモデルを表示する。

# 🔸 T3D視点カメ設定 (Nに/Nへ)
#    指定したカメを視点として使用する
```

### Graph Drawing CHARTJS

**Constants:**

```nadesiko
# 🔹 グラフオプション - {}
```

**Functions:**

```nadesiko
# 🔸 グラフ描画 (DATAを/DATAで/DATAの)
#    Chart.jsを利用して、DATAのグラフを描画(非同期関数)

# 🔸 線グラフ描画 (DATAを/DATAで/DATAの)
#    線グラフを描画(非同期関数)

# 🔸 棒グラフ描画 (DATAを/DATAで/DATAの)
#    棒グラフを描画(非同期関数)

# 🔸 横棒グラフ描画 (DATAを/DATAで/DATAの)
#    横棒グラフを描画(非同期関数)

# 🔸 積上棒グラフ描画 (DATAを/DATAで/DATAの)
#    複数列のデータがある場合積み上げ棒グラフを描画(非同期関数)

# 🔸 積上横棒グラフ描画 (DATAを/DATAで/DATAの)
#    複数列のデータがある場合積み上げ棒グラフを描画(非同期関数)

# 🔸 散布図描画 (DATAを/DATAで/DATAの)
#    散布図を描画(非同期関数)

# 🔸 円グラフ描画 (DATAを/DATAで/DATAの)
#    円グラフを描画(非同期関数)

# 🔸 ドーナツグラフ描画 (DATAを/DATAで/DATAの)
#    円グラフ（ドーナツ）を描画(非同期関数)

# 🔸 ポーラーグラフ描画 (DATAを/DATAで/DATAの)
#    円グラフ（鶏頭グラフ/ポーラーエリアチャート）を描画(非同期関数)

# 🔸 レーダーグラフ描画 (DATAを/DATAで/DATAの)
#    レーダーチャートを描画(非同期関数)

# 🔸 二次元グラフデータ変形 (TのDATAORGを)
#    二次元配列をXXグラフ描画の形式に整形する。種類TとDATAを指定。
```

## System

### Environment Variables

**Functions:**

```nadesiko
# 🔸 環境変数取得 (Sの)
#    環境変数Sを返す

# 🔸 環境変数一覧取得
#    環境変数の一覧を返す
```

### Timer

**Functions:**

```nadesiko
# 🔸 秒待 (N)
#    N秒の間待機する(非同期関数)

# 🔸 秒待機 (N)
#    N秒の間待機する(『秒待』と同じ)(非同期関数)

# 🔸 秒逐次待機 (N)
#    (非推奨) 逐次実行構文にて、N秒の間待機する (廃止予定)(非同期関数)

# 🔸 秒後 (FをN)
#    無名関数（あるいは、文字列で関数名を指定）FをN秒後に実行する。変数『対象』にタイマーIDを代入する。

# 🔸 秒毎 (FをN)
#    無名関数（あるいは、文字列で関数名を指定）FをN秒ごとに実行する(『タイマー停止』で停止できる)。変数『対象』にタイマーIDを代入する。

# 🔸 秒タイマー開始時 (FをN)
#    無名関数（あるいは、文字列で関数名を指定）FをN秒ごとに実行する(『秒毎』と同じ)

# 🔸 タイマー停止 (TIMERIDの/TIMERIDで)
#    『秒毎』『秒後』や『秒タイマー開始』で開始したタイマーを停止する

# 🔸 全タイマー停止
#    『秒毎』『秒後』や『秒タイマー開始』で開始したタイマーを全部停止する
```

### Node Process

**Functions:**

```nadesiko
# 🔸 終
#    Nodeでプログラム実行を強制終了する

# 🔸 強制終了時 (FUNCを)
#    Nodeでctrl+cでプログラムの実行が終了した時FUNCを実行する。もしFUNCが偽を返すと終了しない。非同期処理のとき動作する(#1010)

# 🔸 終了
#    Nodeでプログラム実行を強制終了する

# 🔸 OS取得
#    OSプラットフォームを返す(darwin/win32/linux)

# 🔸 OSアーキテクチャ取得
#    OSアーキテクチャを返す
```

### Debug Support

**Constants:**

```nadesiko
# 🔹 __DEBUG強制待機 - 0
# 🔹 __DEBUGブレイクポイント一覧 - []
# 🔹 __DEBUG待機フラグ - 0
```

**Functions:**

```nadesiko
# 🔸 デバッグ表示 (Sと/Sを/Sの)
#    デバッグ用にSを表示する

# 🔸 ハテナ関数設定 (Sを/Sの)
#    ハテナ関数「?? (計算式)」の動作をカスタマイズする。文字列の配列を指定可能で、システム関数名か「js:code」を指定可能。

# 🔸 ハテナ関数実行 (Sの/Sを/Sと)
#    『ハテナ関数設定』で設定した関数を実行する

# 🔸 エラー発生 (Sの/Sで)
#    故意にエラーSを発生させる

# 🔸 __DEBUG
#    デバッグモードにする

# 🔸 __DEBUG_BP_WAIT (CURLINEで)
#    エディタのブレイクポイント機能のための待機(非同期関数)

# 🔸 グローバル関数一覧取得
#    グローバル変数にある関数一覧を取得

# 🔸 システム関数一覧取得
#    システム関数の一覧を取得

# 🔸 システム関数存在 (FNAMEが/FNAMEの)
#    文字列で関数名を指定してシステム関数が存在するかを調べる

# 🔸 プラグイン一覧取得
#    利用中のプラグイン一覧を得る

# 🔸 モジュール一覧取得
#    取り込んだモジュール一覧を得る

# 🔸 助詞一覧取得
#    文法として定義されている助詞の一覧を取得する

# 🔸 予約語一覧取得
#    文法として定義されている予約語の一覧を取得する
```

### Dialog

**Functions:**

```nadesiko
# 🔸 言 (Sと/Sを)
#    メッセージダイアログにSを表示

# 🔸 尋 (Sと/Sを)
#    メッセージSと入力ボックスを出して尋ねる

# 🔸 文字尋 (Sと/Sを)
#    メッセージSと入力ボックスを出して尋ねる。返り値は常に入力されたままの文字列となる

# 🔸 二択 (Sで/Sの/Sと/Sを)
#    メッセージSと[OK][キャンセル]のダイアログを出して尋ねる。戻り値はtrueかfalseのどちらかになる。
```

### Plugin Management

**Constants:**

```nadesiko
# 🔹 プラグイン名 - 'メイン'
# 🔹 名前空間 - ''
```

**Functions:**

```nadesiko
# 🔸 プラグイン名設定 (Sに/Sへ)
#    プラグイン名をSに変更する(システムにより自動的に「メイン」あるいはプラグインのファイル名が呼ばれる)

# 🔸 名前空間設定 (Sに/Sへ)
#    名前空間をSに設定する(システムにより自動的に変更される。ファイル名から拡張子を削ったもの)

# 🔸 名前空間ポップ
#    システム利用のため呼ぶべからず。(名前空間を一つ前の値に戻す)
```

## Advanced

### Asynchronous Processing Guarantee

**Functions:**

```nadesiko
# 🔸 動時 (CALLBACKを/CALLBACKで)
#    非同期処理を作成する。非同期処理オブジェクト(Promise)を返す。

# 🔸 成功時 (CALLBACKをPROMISEの/PROMISEが/PROMISEに)
#    非同期処理で成功したときにcallbackが実行される。その際『対象』にデータが代入される。

# 🔸 処理時 (CBFUNCをPROMISEの/PROMISEが/PROMISEに)
#    非同期処理で終了した時にcbFuncが実行される。引数と『対象』は、成功時は真とデータが設定され、失敗時は、偽と理由が設定される。

# 🔸 失敗時 (CALLBACKをPROMISEの/PROMISEが/PROMISEに)
#    非同期処理で失敗したときにcallbackが実行される。その際『対象』に理由が代入される。

# 🔸 終了時 (CALLBACKをPROMISEの/PROMISEが/PROMISEに)
#    非同期処理で終了したときにcallbackが実行される。成功時・失敗時・処理時とは別に実行される。

# 🔸 束 (...ARGSと/...ARGSを)
#    非同期処理をまとめる。(可変引数)
```

### NAKO Worker

**Functions:**

```nadesiko
# 🔸 ワーカー起動 (URLで/URLを/URLの)
#    指定したURLでWebWorkerを起動する。ワーカオブジェクトを返す。

# 🔸 ワーカーJS起動 (SRCで/SRCを/SRCの)
#    指定したJavascriptのソースでWebWorkerを起動する。ワーカオブジェクトを返す。

# 🔸 NAKOワーカー起動 (PLUGINSで)
#    指定したなでしこ３のWebWorkerを起動する。ワーカオブジェクトを返す。(可変引数)

# 🔸 NAKOワーカーハンドラ設定 (WORKに/WORKへ/WORKの)
#    ワーカーにNAKOワーカーのための設定を行う。

# 🔸 NAKOワーカーデータ受信時 (FUNCでWORKから)
#    無名関数Fでなでしこv3エンジンに対してワーカーメッセージによりデータを受信した時に実行するイベントを設定。『受信データ』に受信したデータ。『対象イベント』にイベント引数。(可変引数)

# 🔸 NAKOワーカー表示時 (FUNCでWORKから)
#    無名関数Fでなでしこv3エンジンに対してワーカーメッセージにより表示データを受信した時に実行するイベントを設定。『受信データ』に表示しようとしたデータ。『対象イベント』にイベント引数。

# 🔸 ワーカーメッセージ受信時 (FUNCでWORKから)
#    無名関数Fでworkに対してメッセージを受信した時に実行するイベントを設定。『受信データ』に受信したデータ。『対象イベント』にイベント引数。(可変引数)

# 🔸 NAKOワーカープログラム起動 (WORKにDATAを/WORKで)
#    WORKERに固有の形式でプログラムの転送と実行行う。

# 🔸 NAKOワーカーリセット (WORKを)
#    WORKERに固有の形式でプログラムの転送と実行行う。

# 🔸 ワーカー終了 (WORKを)
#    WORKERを終了する。(可変引数)

# 🔸 NAKOワーカー終了 (WORKを)
#    WORKERを終了する。(可変引数)

# 🔸 NAKOワーカーデータ送信 (DATAをWORKに/WORKへ)
#    WORKERに固有の形式でデータを送信する。(可変引数)

# 🔸 ワーカーメッセージ送信 (MSGをWORKに/WORKへ)
#    WORKERにメッセージを送信する。(可変引数)

# 🔸 NAKOワーカー転送 (DATASをWORKに/WORKへ)
#    WORKERにユーザー定義関数またはユーザ定義のグローバル変数を転送する。(可変引数)
```

### Machine Learning

**Functions:**

```nadesiko
# 🔸 SVM開 (OPTIONで)
#    機械学習のアルゴリズムSVMをパラメータOPTIONで開く。 OPTION={type,kernel,gamma,cost}

# 🔸 ランダムフォレスト開 (OPTIONで)
#    機械学習のアルゴリズムRandom ForestをOPTIONで開く。OPTION={seed,maxFeatures,replacement=(true/false),nEstimators}

# 🔸 ランダムフォレスト回帰開 (PARAMSで)
#    機械学習のアルゴリズムRandom Forestの回帰をパラメータPARAMSで開く

# 🔸 学習 (INPUTSとLABELSで)
#    入力配列inputsとラベル配列labelsで機械学習する

# 🔸 予測 (INPUTSを/INPUTSで)
#    入力配列inputsで予測し機械学習の結果を配列で返す

# 🔸 アヤメデータ取得
#    アヤメデータをJSON形式で取得して返す

# 🔸 モデル取得
#    現在学習済みのモデルを取得する

# 🔸 モデル設定 (Mを/Mの)
#    現在学習済みのモデルMを設定する

# 🔸 データランダム分割 (DATAとLABELをRATEで)
#    データとラベルの組をRATEで分割して{学習:{データ:[..],ラベル:[..]},テスト:{データ:[..],ラベル:[..]}}の形式で返す

# 🔸 正解率計算 (TとPの/Pで)
#    配列T(正解)とP(予測)の正解率を計算して返す
```

### Morphological Analysis (MECAB)

**Functions:**

```nadesiko
# 🔸 MECAB (Sで/Sを)
#    Sについて形態素解析を行って結果を二次元配列で返す

# 🔸 MECABヨミガナ取得 (Sの/Sを/Sから)
#    Sについてヨミガナを取得する
```

### Speech Synthesis

**Constants:**

```nadesiko
# 🔹 話者速度 - 1.0
# 🔹 話者声高 - 1.0
# 🔹 話者音量 - 1.0
```

**Functions:**

```nadesiko
# 🔸 話 (Sと/Sを/Sの)
#    音声合成APIを使って、Sを発話する

# 🔸 話終 (Sと/Sを/Sの)
#    音声合成APIを使ってSを発話し終えるまで待機する(非同期関数)

# 🔸 話終時 (CALLBACKでSと/Sを/Sの)
#    音声合成APIを使って、Sを発話し発話した後でcallbackを実行

# 🔸 音声合成発話オブジェクト取得 (Sの/Sで)
#    内容Sで音声合成APIのインスタンスを得る

# 🔸 話者一覧取得
#    音声合成APIの話者一覧を得る

# 🔸 話者設定 (Vに/Vへ)
#    音声合成APIの話者を指定する

# 🔸 話者詳細設定 (OBJで/OBJに/OBJへ)
#    音声合成APIの話者の設定をオブジェクト形式{速度:1.0,ピッチ:1.0,音量:1.0}のように設定する
```

### Music

**Functions:**

```nadesiko
# 🔸 MML演奏 (MMLを/MMLの)
#    MMLを演奏する

# 🔸 MML停止
#    MML演奏で開始した演奏を停止する

# 🔸 MIDI演奏 (URLを/URLの)
#    MIDIファイルのあるURLを指定して演奏する(非同期関数)

# 🔸 MIDI停止
#    MIDI演奏で開始した演奏を停止する

# 🔸 MIDIループ再生設定 (Vに/Vへ)
#    V(オン/オフ)にMML演奏/MIDI演奏で再生をループするように指定
```
