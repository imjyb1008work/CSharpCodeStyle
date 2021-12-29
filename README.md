# C# Code Style Guide

Item | 採用方式 | 前綴 | 後綴 | 備註
---- |--------| -----|-----  | ----
Class | PascalCase | |  | 使用名詞或名詞片，不使用前後綴，並且與程式碼檔案名稱相同
Interface | PascalCase | I |
Method | PascalCase
Enum | PascalCase
Public Propery | PascalCase
Public Field | PascalCase
local variable | camelCase
private field | camelCase | _ |

## [Class(類別)](https://docs.microsoft.com/zh-tw/dotnet/csharp/fundamentals/types/classes)

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

## [Interface(介面)](https://docs.microsoft.com/zh-tw/dotnet/csharp/language-reference/keywords/interface)

前綴一律大寫I

## [Enum](https://docs.microsoft.com/zh-tw/dotnet/csharp/language-reference/builtin-types/enum)(列舉)

使用大駱駝峰式命名，後綴可加上Type或是Enum

## 集合變數、迴圈、Array、List、[LINQ](https://docs.microsoft.com/zh-tw/dotnet/csharp/programming-guide/concepts/linq/)

### 集合變數

- 建議使用複數名詞

### for迴圈

1. 請優先依序i、j、k
2. 不建議用到4層以上的迴圈

例如:

```C#
int length = 10;

for(var i = 0; i < length; i++)
{
	for(var j = 0; j < length; j++)
	{
		for(var k = 0; k < length; k++)
		{
		}    
	}
}
```

### Array vs List

- 使用Array建議的情境
  
  - 集合大小固定
  - 資料不可變
  - 要求執行速度
- 使用List建議的情境
  
  - 集合大小不確定
  - 資料可變動
  - 程式撰寫靈活性

LINQ結果的查詢變數後綴可接Query

## 布林變數

開頭建議使用is、can、has、shoud，若無法定義其名稱可使用flag
