1.读懂下面代码片段  关键点  .box代表是class = box的元素。

```javascript	
$(".box").click(function(e){
  if($(e.target).is("input")){
      $(".box").removeClass("blueBox");
      $(this).toggleClass("blueBox");
      return;
  }  
``` 
Reference:  
1.[http://www.w3school.com.cn/jquery/attributes_removeclass.asp](http://www.w3school.com.cn/jquery/attributes_removeclass.asp)
2.[http://www.w3school.com.cn/jquery/attributes_removeclass.asp](http://www.w3school.com.cn/jquery/attributes_removeclass.asp)


3.

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
1.[http://getfuelux.com/javascript.html#wizard](http://getfuelux.com/javascript.html#wizard)



 