# 簡介 #

本文是周蟒語法快速參考手冊

大多數的 Python 程式的語法都可在周蟒中找到對應的中文關鍵詞。

最新的完整關鍵詞對應表請參照[這裡](KeyWords.md)。

# 保留字 #

英文
```
['and', 'as', 'assert', 'break', 'class', 'continue', 'def', 'del', 'elif', 
'else', 'except', 'exec', 'finally', 'for', 'from', 'global', 'if', 'import', 
'in', 'is', 'lambda', 'not', 'or', 'pass', 'print', 'raise', 'return', 
'try', 'while', 'with', 'yield']
```

正體中文
```
['和', '作為', '申明', '中斷', '類別', '繼續', '定義', '刪除', '假使',
'否則', '異常', '執行', '最後', '取', '從', '共用', '如果', '導入',
'自', '是', '方程式', '非', '或', '略過', '印出', '引發', '返回',
'嘗試', '當', '伴隨', '產生']
```

簡體中文
```
['和', '作为', '申明', '中断', '类', '继续', '定义', '删除', '假使',
'否则', '异常', '执行', '最后', '取', '从', '共用', '如果', '导入',
'自', '是', '方程式', '非', '或', '略过', '印出', '引发', '返回',
'尝试', '当', '伴随', '产生']
```

# 內建類型 #

## 數字 ##

  * 整數: 1, 256
  * 浮點數: 3.14, 0.86, 1.2e-3
  * 複數
  * 十六進位: 0xfffe

## 字串 ##

  * 單引號字串 'this is string'
  * 雙引號字串 "this is string"

## 文件字串 ##

  * """this is docstring"""

## 布林 ##

  * 真/假: True/False

## 列表 ##

  * ['this', 'is','list']
  * [1,2,3,4]

## 字典 ##

  * {"真":"True", "十":10, "表":[1,2,3]}

## 元組 ##

  * (1,2,3)

## 集合 ##

  * set((1,2,3))
  * set([1,2,3])

## 空 ##

  * None

## 檔案 ##

  * fd = file.open('hello.txt').read()

# 關鍵詞 #

## 輸入輸出 Input/Output ##

| 關鍵詞 | 繁體中文 | 簡體中文 |
|:----|:-----|:-----|
| raw\_input | 輸入         | 输入   |
| print      | 印出         | 打印          |

## 類別, 定義 Definition ##

| 關鍵詞 | 繁體中文 | 簡體中文 |
|:----|:-----|:-----|
| def     | 定義      | 定义       |
| class    | 類別       | 类         |
| global  | 共用       | 共用   |

## 導入模組 import module ##

| 關鍵詞 | 繁體中文 | 簡體中文 |
|:----|:-----|:-----|
| from    | 從        | 从         |
| import  | 導入      | 导入      |
| as       | 作為      | 作为     |

基本語法:

  * import
  * from ... import
  * from ... import ... as

```
  導入 sys
```

```
  從 os 導入 path
```

```
  從 os 導入 path 作為 路徑
```

## 回應 response ##

| 關鍵詞 | 繁體中文 | 簡體中文 |
|:----|:-----|:-----|
| return   | 返回     | 返回       |
| pass     | 略過      | 略过      |
| raise     | 引發      | 引发     |
| continue | 繼續      | 继续     |

## 控制流程 flow control ##

| 關鍵詞 | 繁體中文 | 簡體中文 |
|:----|:-----|:-----|
| if  | 如果   | 如果   |
| elif | 假使, 否則如果 | 假使, 否则如果 |
| else | 否則   | 否则   |


基本語法:

  * if ...: ...
  * if ...: ... else [...] : ...
  * if ...: ... elif [...] : ... else [...] : ...

```
人數 = 10
如果 人數 為 空:
    印出 "都沒人"
否則:
    印出 人數
```

## 迴圈 ##

| 關鍵詞 | 繁體中文 | 簡體中文 |
|:----|:-----|:-----|
| for   | 取     | 取    |
| in     | 自,在  | 自,在      |
| while  | 當    | 当    |
| break | 中斷, 跳出  | 中斷, 跳出 |

基本語法:

  * for ... in ...
  * while ... break

## 驗證 ##

| 關鍵詞 | 繁體中文 | 簡體中文 |
|:----|:-----|:-----|
| try      | 嘗試      | 尝试    |
| except  | 異常      | 异常   |
| finally   | 最後      | 最后       |
| assert   | 申明      | 申明       |

基本語法:

  * try ... except
  * try ... except ... else
  * try ... finally

```
嘗試:
    導入 sqlalchemy

異常, 導入錯誤, 錯誤訊息:
    印出 錯誤訊息
```

## 邏輯 ##

| 關鍵詞 | 繁體中文 | 簡體中文 |
|:----|:-----|:-----|
| and      | 和      | 和    |
| or      | 或      | 或    |
| is      | 是      | 是    |
| not      | 非      | 非    |
| is not      | 不是      | 不是    |
| True     | 真    | 真    |
| False    | 假    | 假    |
| None    | 空    | 空    |
