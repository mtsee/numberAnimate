#高效的数字滚动插件一枚,兼容到IE8+
插件地址：[插件地址](http://www.mtsee.com/numberAnimate/)
```javascript
// #使用方法：
// 默认参数
option = { 
  speed : 1000,//动画速度
  num : "", //初始化值
  iniAnimate : true, //是否要初始化动画效果
  symbol : '',//默认的分割符号，千，万，千万
  dot : 0 //保留几位小数点
}
// 调用numberAnimate方法会回调一个函数 ：resetData(num); 方法，传入新的参数即可变化
var d = $(obj).numberAnimate(option);
d.resetData(new num);

// #案例如下
//JS
var numRun = $(".numberRun").numberAnimate({num:'15343242.10', dot:2, speed:2000, symbol:","});
var nums = 15343242.10;
setInterval(function(){
    nums+= 3433.24;
    numRun.resetData(nums);
},3000);
```
