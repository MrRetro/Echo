# echo.js
前端常用的一些js事件(基于jQuery1.11.3开发)

01.场景：当我们需要在一个标签A上绑定一个点击事件来控制标签B的变化(只有两种状态)       
  实现：$.fn.binChange({btn:'按钮类名',target:'目标类名',cs:'状态名称',click:'事件名称'})   
  -->点这里：[binChange](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/01.给按钮绑定事件.html)
     
02.场景：需要在非A标签的标签上也有A标签的跳转事件   
  实现：$.fn.aLink({btn:'按钮类名',target:'跳转类型',click:'事件名称',link:'跳转路径'})   
  -->点这里：[aLink](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/02.单页非a标签需要有a标签跳转.html)
     
03.场景：整个页面需要响应式-根据根html标签的大小来控制   
  实现：$.fn.autoFontSize({fontSize:'根字体大小',screenW:'适配显示器的最大宽度'})   
  -->点这里：[autoFontSize](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/03.小球随html字体大小而缩放.html)
     
04.场景：批量给关键字加高亮状态   
  实现：$.fn.light({content:'上下文',target:'目标',key:'关键字',newKey:'新关键字',cs:'类名'})   
  -->点这里：[light](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/04.批量替换关键字.html)
     
05.场景：给背景图片做预加载   
  实现：$.fn.imgsOpt({cs:'目标',color:'loading颜色',scale:'loading缩放比例'})   
  -->点这里：[imgsOpt](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/05.背景图片预先加载.html)
     
06.场景：页面滚轮回到固定位置  
	实现：$.fn.scrollTop({cs:'目标',top:'置顶位置',click:'事件',	animate:'是否动画',time:'动画时间',parent:'是否为父类'})    
  -->点这里：[scrollTop](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/06.滚轮回到顶部.html)
     
07.场景：浏览器在不操作的情况下超时处理  
	实现：$.fn.countDown({time:'时间单位为秒  60秒为1分钟|3600秒为一小时|86400秒为一天 ',cs:'倒计时数元素',func:'回调函数/这边的回调函数也可以放在第二形参位置'})    
  -->点这里：[countDown](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/07.倒计时关闭浏览器.html)
     
08.场景：浏览器滚动加载也叫下拉刷新  
	实现：$.fn.rollLoad({range:'距下边界长度/单位px',maxNum:'设置加载最多次数',func:'回调函数/这边的回调函数也可以放在第二形参位置'})    
  -->点这里：[rollLoad](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/08.滚动加载_下拉刷新.html)
     
09.场景：鼠标移动到一个不规则图像时选中这个图像     
	实现：$.fn.polygon(e,callback)   
#### {    
        btn:'',	//目标    
        click:'click',	//事件    
        poly:[],	//多边形点坐标数组    
        cs:'',	//变化类名    
        func:{},	//回调函数    
#### }     
    参数callback:此处放回调函数     
  -->点这里：[polygon](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/09.计算鼠标是否在多边形内.html)
     
10.场景：通过坐标点数据画出折线图  
	实现：$.fn.svgLines(e,callback)   
			参数e:      
#### {       
        points:[],	//坐标点[{x:50,y:50},{x:60,y:70},{x:80,y:90}]    
        btn:'svg',	//svg元素     
        style:{},	//svg样式    
        parent:'body',	//父级有影响排版的类名     
        color:'rgb(0,170,255)',	//线颜色    
        strokeWidth:2,	//线粗细   
        click:'click',	//给每段直线绑定事件   
        func:{},	//回调函数   
#### }
    参数callback:此处放回调函数     
  -->点这里：[svgLines](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/10.根据所有点坐标画折线.html)
     
11.场景：复制网页的内容后想让别人看到自己的版权  
	实现：$.fn.pasteFrom({url: '连接地址',description: '版权说明'})    
  -->点这里：[pasteFrom](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/11.复制后自带版权.html)
     
12.场景：获取页面所有标签的类名和id并去重  
	实现：$.fn.getClasses()    
  -->点这里：[getClasses](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/12.获取页面所有标签的类名和id并去重.html)
     
13.场景：筛选出所有存在的id或类名的样式行  
	实现：$.fn.getStyleLines(e)   
			参数e:      
#### {       
        el:[],	//类名或id数组    
        css:'',	//样式字符串
#### }
  -->点这里：[getStyleLines](http://htmlpreview.github.io/?https://github.com/MrRetro/Echo/blob/master/src/13.筛选出所有存在的id或类名的样式行.html)