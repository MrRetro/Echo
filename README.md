# echo.js
前端常用的一些js事件(基于jQuery1.11.3开发)

1.场景：当我们需要在一个标签A上绑定一个点击事件来控制标签B的变化(只有两种状态)    
  实现：$.fn.binChange({btn:'按钮类名',target:'目标类名',cs:'状态名称',click:'事件名称'})
  [binChange](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/1.给按钮绑定事件.html)
