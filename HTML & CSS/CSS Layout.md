### float 排版
- float區塊無法調整同樣高度

- 橫向排列只能靠上對齊
 
- 必要時使用 div 群組化
 
- 解除 float 方法:
    + 在要解除 float 的下一個元素使用 clear:both
    + 以 :after 生成虛擬元素，並且在該元素中解除 float
    + 使用 overflow:hidden  
