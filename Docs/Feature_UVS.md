# 「遊趣體」變體序列一覽表 
## Unicode 標準化變體序列  
Unicode 標準化變體序列 (Standardized Variation Sequences, SVS) 資料來源：https://www.unicode.org/Public/16.0.0/ucd/StandardizedVariants.txt

根據 Unicode 16.0 相關文檔，TC 0.500 版本新增 Unicode 變體序列（UVS）支援，在允許使用 UVS 的情況下，可透過該功能實現標點符號位置與寬度的切換，以及部分字符的變體字形。  
支援的標準化變體序列如下表：  
| 字元 | Unicode | + `U+FE00` | + `U+FE01` | 
| :-------: | :-------: | :--------: | :--------: | 
| 0 | `U+30` | 斜線零[0︀] |
| ０ | `U+FF10` | 斜線零[0︀] |
| ， | `U+FF0C` | 左下[<span lang="zh-cn">，︀</span>] | 置中[<span lang="zh-tw">，︁</span>] |
| ． | `U+FF0E` | 左下[<span lang="zh-cn">．︀</span>] | 置中[<span lang="zh-tw">．︁</span>] |
| 、 | `U+3001` | 左下[<span lang="zh-cn">、︀</span>] | 置中[<span lang="zh-tw">、︁</span>] |
| 。 | `U+3002` | 左下[<span lang="zh-cn">。︀</span>] | 置中[<span lang="zh-tw">。︁</span>] |
| ： | `U+FF1A` | 左下[<span lang="zh-cn">：︀</span>] | 置中[<span lang="zh-tw">：︁</span>] |
| ； | `U+FF1B` | 左下[<span lang="zh-cn">；︀</span>] | 置中[<span lang="zh-tw">；︁</span>] |
| ！ | `U+FF01` | 靠左[<span lang="zh-cn">！︀</span>] | 置中[<span lang="zh-tw">！︁</span>] |
| ？ | `U+FF1F` | 靠左[<span lang="zh-cn">？︀</span>] | 置中[<span lang="zh-tw">？︁</span>] |
| “ | `U+201C` | 比例[“] | 全形[“︁] |
| ” | `U+201D` | 比例[”] | 全形[”︁] |
| ‘ | `U+2018` | 比例[‘] | 全形[‘︁] |
| ’ | `U+2019` | 比例[’] | 全形[’︁] |

> [!NOTE]
> 1. 若全形標點在橫排時偏置（靠左下方），則直排時靠右上方偏置。反之若標點橫排時置中，則直排位置不變更。  
> 2. 此規定可能與 UAX#50 規則衝突，部分軟件可能因此顯示異常，具體表現為全形冒號「：」與全形分號「；」直排時翻轉 90 度。

## 關於 SVS 的常見問題  
### Q：如何使用全形彎引號特性？  
A：在 Word (Microsoft 365) 中，在支援變體序列的字元後（如彎引號`“‘’”`）後輸入變體選擇符的 Unicode 碼位（如`FE01`），再按 Alt + X，即可使用變體序列。

### Q：為什麼此字型在一些情況下不支援 SVS 特性？ 
A：部分軟體不支援此特性，如**PowerPoint (Microsoft 365)** 等，使用時需留意。
