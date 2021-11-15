# C# Code Style Guide


以下採用PascalCase
- Class
- Method
- Enum
- Public Propery
- Public Field

以下採用camelCase
- local variable(方法變數或區域變數)

以下採用_camelCase
- private field


迴圈變數
請優先依序i、j、k

集合變數
建議使用複數名詞

Array vs List
使用Array建議的場合
- 集合大小固定
- 資料不可變
- 要求執行速度

使用List建議的場合
- 集合大小不確定
- 資料可變動
- 程式撰寫靈活性

Linq結果的查詢變數後綴可接Query


## Class(類別)

使用大駝峰式命名法

使用名詞或名詞片，不使用前後綴，與檔案名稱相同

## Property(屬性)

使用大駝峰式命名法

使用名詞或名詞片，不使用前後綴

## Field(欄位)

使用駝峰式命名法

前綴使用底線

## Method(方法)

使用大駱駝峰式命名

方法的參數請使用駝峰式

## 區域變數

## Interface(介面)

前綴一律大寫I

## Enum(列舉)

使用大駱駝峰式命名，後綴可加上Type或是Enum

## Array、List、集合變數

## 布林變數

開頭建議使用is、can、has、shoud，若無法定義其名稱可使用flag
