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




 