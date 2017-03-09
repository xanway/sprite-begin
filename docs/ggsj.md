<h1>公共事件</h1>

----------
  

**click事件**

单击UI组件时候触发，event事件对象包括：  

>   type：事件类型，字符串类型，固定值：click；
>   
>   target：触发事件的目标组件，dom对象；
>   
>   timestamp：事件触发的时间戳,单位毫秒，数字类型

示例：   

```javascript
button.on("click",function(event){
    var eventType = event.type;
    var targetObj = event.target;
    var timestamp = event.timestamp;
});

```

**注：**  当某个控件同时有click和touchMove事件时，当touchMove事件触发后，click事件就会失效，这个特点可以用来做那种点上去如果反悔了可以移动手指让点击事件失效的效果。


**longTouch事件**  

长按UI组件时候触发，event事件对象包括：  

>   type：事件类型，字符串类型，固定值：longTouch；  
>     
>  target：触发事件的目标组件，dom对象；  
>     
>  timestamp：事件触发的时间戳,单位毫秒，数字类型
 

示例：  

```javascript
button.on("longTouch",function(event){
    var eventType = event.type;
    var targetObj = event.target;
    var timestamp = event.timestamp;
});

```

**注：**  如果触发了longTouch事件，click事件也会失效。


 

