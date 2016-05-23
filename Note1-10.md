1.读懂下面代码片段  关键点  .box代表是class = box的元素。

```javascript	
$(".box").click(function(e){
  if($(e.target).is("input")){
      $(".box").removeClass("blueBox");
      $(this).toggleClass("blueBox");
      return;
  }  
``` 
Ref:  
[http://www.w3school.com.cn/jquery/attributes_removeclass.asp](http://www.w3school.com.cn/jquery/attributes_removeclass.asp)
[http://www.w3school.com.cn/jquery/attributes_removeclass.asp](http://www.w3school.com.cn/jquery/attributes_removeclass.asp)



 