# Python 的檔案 IO

檔案 (Files) 裡面存放的是位元組 (Bytes)。

如果檔案內的所有位元組可以對應到任何語系的任何字元，則該檔案可以歸類為文字檔 (Text Files)，如果不行則該檔案是二進位檔 (Binary Files)。

檔案的分類：

* 文字檔
  - 一般文字檔
  - .csv (Comma-Separated Values)
  - .html (<標籤> </標籤>)
* 二進位檔
  - 圖片檔
  - .xls, .xlsx

## 文字檔的讀寫方式

1. 使用 open() 來打開檔案，並選擇操作模式 (mode)，預設的操作模式為 'r'，即讀取模式。
2. 使用 read() 或 write() 等等方法來讀寫檔案。
3. 使用 close() 來關閉檔案，將記憶體內的位元組寫入檔案，並釋放資源。

## open() 的模式 (mode) 字元：

|字元|說明|
|:-:|:-|
|r|讀取模式|
|w|寫入模式|
|x|檔案不存在時才寫入|
|a|附加模式|
|b|二進位模式|
|t|文字模式|
|+|更新模式|

## 讀取文字檔

用下面三個函式，讀取文字檔資料：

* read()：一次讀完全部內容。
* readline()：一次讀一行。
* readlines()：一次讀完全部的行數，並放在 list 裡面。

```python
# 方法一
f = open('test.txt')
data = f.read()
print(data)
f.close()

# 方法二
f = open('test.txt')
line = f.readline()
while line:
    print(line, end="")
    line = f.readline()
f.close()

# 方法三
f = open('test.txt')
lines = f.readlines()
for line in lines:
    print(line, end="")
f.close()

# 方法四
f = open('test.txt')
for line in f:
    print(line, end="")
f.close()
```

## 用 with 建立檔案，會自動呼叫 close() 

語法：

```python
with open("test.txt") as f:
    data = f.read()
    print(data)
```

## 二進位檔的讀寫方式

1. 使用 open() 來打開檔案，並選擇操作模式 (mode)，如 'rb'為讀取二進位檔，'wb'為寫入二進位檔。
2. 使用 read() 或 write() 等等方法來讀寫檔案。
3. 使用 close() 來關閉檔案，將記憶體內的位元組寫入檔案，並釋放資源。

```python
import requests
url = "https://doqvf81n9htmm.cloudfront.net/data/changchi_177/51079024_574066513066625_5229772988173254656_n.jpg"

# 抓取圖片
r = requests.get(url)

# 存成檔案
with open("kuo.jpg", "wb") as f:
    f.write(r.content)
```