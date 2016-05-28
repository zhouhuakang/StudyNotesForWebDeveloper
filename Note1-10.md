#1.读懂下面代码片段  关键点  .box代表是class = box的元素。

```javascript	
$(".box").click(function(e){
  if($(e.target).is("input")){
      $(".box").removeClass("blueBox");
      $(this).toggleClass("blueBox");
      return;
  }  
``` 
Reference:  
1.1.[http://www.w3school.com.cn/jquery/attributes_removeclass.asp](http://www.w3school.com.cn/jquery/attributes_removeclass.asp)
1.2.[http://www.w3school.com.cn/jquery/attributes_removeclass.asp](http://www.w3school.com.cn/jquery/attributes_removeclass.asp)


#3.事件绑定

```javascript
$wizard.wizard().on('finished', function (e) {
    // wizard complete code
}).on("changed", function (e) {
    var step = $wizard.wizard("selectedItem");
    // reset states
    $btnNext.removeAttr("disabled");
    $btnPrev.removeAttr("disabled");
    $btnNext.show();
    $btnFinish.hide();
    if (step.step === 1) {
        $btnPrev.attr("disabled", "disabled");
    } else if (step.step === 4) {
        $btnNext.hide();
        $btnFinish.show();
    }
});
```
Reference:  
2.1.[http://getfuelux.com/javascript.html#wizard](http://getfuelux.com/javascript.html#wizard)  
2.2.[jQuery事件绑定.on()简要概述及应用](http://www.jquerycn.cn/a_5346)  





#4.disable标签和removeAttr()   
[HTML disabled属性的启用和禁止](http://tjuking.iteye.com/blog/1397821)   
[jQuery 属性操作 - removeAttr() 方法](http://www.w3school.com.cn/jquery/attributes_removeattr.asp)

##5.JQuery如何自定义插件——$.fn的使用
[JQuery如何自定义插件——$.fn的使用](http://www.2cto.com/kf/201412/357002.html)  
[jquery开发自定义的插件总结](http://www.cnblogs.com/Jimmy009/archive/2013/01/17/jquery%E6%8F%92%E4%BB%B6.html)    
[jQuery自定义插件](http://blog.csdn.net/bao19901210/article/details/21540137/)

##6.好书推荐：《你不知道的JavaScript(上卷)》KYLE SIMPSON著作
    看了第一部分前两节的内容，觉得虽然有些部分还是写的通俗，但是有些内容比较学术，感觉是javascript层编译原理。先阶段是在学习使用javascript，估计还是不适合看这本书
    
    	
##7.jQuery.serializeArray() 函数详解  
[jQuery.serializeArray() 函数详解](http://www.365mini.com/page/jquery-serializearray.htm)



 