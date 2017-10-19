### 元素選擇器
選擇器       |功能                   |範例           
------------|-----------------------|-------------------
`*`           |所有元素                | * {...}
E           |指定元素                | h1 {...}
#id         |指定索引                | #myID {...}
.class      |指定型別                | .myClass {...}
E F         |所有子/孫元素           | h1 span {...}
E>F         |所有子元素　            | ui>li {...}
E+F         |同一階層相鄰元素         |h2+p {...}
E~F         |同一階層Ｅ之後所有元素   |h2~p {...}

<br>

### 屬性選擇器
選擇器               |功能                         |範例           
--------------------|-----------------------------|-------------------
E[attr]             |擁有指定屬性的元素             | a[href]
E[attr="value"]     |擁有指定屬性與值的元素         | a[target="_blank"]
E[attr^="value"]    |屬性的值以 value 開頭的元素    | a[target^="_blank"]
E[attr$="value"]    |屬性的值以 value 結尾的元素    | a[target$="_blank"]
E[attr*="value"]    |屬性的值包含 value 的元素      | a[target*="_blank"]

<br>

### 虛擬型別 
選擇器                   |功能                       |範例           
------------------------|---------------------------|-------------------
:root                   |文檔根元素(html)            |
:link                   |未訪問的連結                | a:link
:visited                |已訪問的連結                | a:visited
:hover                  |滑鼠移入元素時              | a:hover
:active                 |點選元素時                  | a:active
:focus                  |元素聚焦時                  | a:focus
:first-child            |首位子元素                  | li:first-child
:last-child             |末位子元素                  | 
:nth-child(n)           |第n個子元素                 | 
:nth-last-child(n)      |倒數第n個子元素             | 
:only-child             |唯一子元素                  | 
:first-of-type          |首位元素                    | 
:last-of-type           |末位元素                    | 
:nth-of-type(n)         |第n個元素                   | 
:nth-last-of-type(n)    |倒數第n個子元素             | 
:only-of-type           |唯一元素                    | 
:empty                  |沒有文字內容的元素           | 
:not(s)                 |不含s的元素                 | 
:target                 |目標元素                    |
:enabled                |可輸入的UI元素              | 
:disabled               |無法輸入的UI元素            | 
:checked                |已點選的UI元素              | 
:lang()                 |元素含有指定編碼時           | span:lang(en)

<br>

### 虛擬元素 
選擇器                   |功能                      |範例           
------------------------|--------------------------|-------------------
:first-letter           |元素內容的第一個字          | p:first-letter
:first-line             |元素內容的第一行            | p:first-line
:before                 |在元素前面產生內容          | p:before
:after                  |在元素後面產生內容          | p:after
::first-letter          |元素的第一行               | 
::first-line            |元素的第一個字             | 
::before                |在元素前面插入內容          | 
::after                 |在元素後面插入內容          | 
::selection             |使用者選擇的區域            | 