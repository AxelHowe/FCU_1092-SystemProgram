# SIC Assembler (SIC版本 完成)

- 班級：資訊二乙
- 學號：D0886096
- 姓名：蘇家弘

## 1. 程式開發過程 
- 程式開發過程僅參考課本架構自行開發

## 2. 開發語言、開發平台、程式使用方式、使用範例與輸出結果範例  
- 開發語言：Python
- 開發平台：使用 PyCharm 作為開發環境
- 程式使用方式
    - 將組譯檔(SRCFILE)與程式檔(D0886096.py)放在同個目錄下
    - 執行.py檔
- 使用範例
    - 組譯檔案(SRCFILE)
    - ![](https://i.imgur.com/oiDtKUG.png)

- 輸出結果範例
    - 輸出OBJFILE
    - ![](https://i.imgur.com/E6MQNli.png)
    - 輸出LISTFILE
    - ![](https://i.imgur.com/PejMTQb.png)

## 3. 可以處理怎樣格式的輸入
- 組譯的檔案名稱須為 "SRCFILE"
- 指令的前後有空白或是大小寫皆可被程式正常判斷
- 可以處理註解
## 4. 有哪些輸出
- 可以產生 Object file 與 Listing file
- 錯誤訊息只能判斷以下三種
    - 判斷重複的Label
    - 判斷錯誤的指令
    - 判斷沒有宣告過的Label
- 錯誤訊息會輸出在Terminat
## 5. 可以處理哪些 addressing modes
- 本組譯器為SIC版本，無法處理SIC/XE的 addressing modes

## 6. 可以處理哪些 assembler directives
- 可正常處理 start/end/byte/word/resb/resw
- 即 SIC 基本版假指令皆可執行
- byte指令可判斷 C 與 X 並處理
- word指令可判斷負數

## 7. 有哪些 data structures (說明自行開發的或者自行修改的即可，  
- 使用Python的dictionary實作OPTAB及SYMTAB

## 8. 有哪些 特別的 function
- readline()
    - 負責讀取組譯檔
    - 可以過濾大小寫及空格
- ifComment()
    - 負責判斷是否為註解行
- storeData()
    - 負責第一階段時把資料存入
- readData()
    - 在第二階段時負責把儲存的資料取出

## 9. 心酸血淚史 
- 這次想說使用Python開發應該會比較容易，順便練習我對Python語言的熟悉度，但可惜因為我把時間分配在做其他的專題，所以只寫了SIC版本的Assembler。在撰寫的過程中，有多次需要回頭修改程式碼的部分，我體驗到程式碼可修改性的重要，還好我也都有寫成函式處理，變數的命名也不太隨便，才沒有太困擾的事情發生。