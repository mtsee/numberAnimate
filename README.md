#高效的数字滚动插件一枚,兼容到IE8+
#使用方法：
//默认参数<br />  
option = { <br />  
  speed : 1000,//动画速度<br />  
  num : "", //初始化值<br />  
  iniAnimate : true, //是否要初始化动画效果<br />  
  symbol : '',//默认的分割符号，千，万，千万<br />  
  dot : 0 //保留几位小数点<br />  
}<br />  
//调用numberAnimate方法会回调一个函数 ：resetData(num); 方法，传入新的参数即可变化<br />  
var d = $(obj).numberAnimate(option); <br />  
d.resetData(new num);<br />  
<br />  
#案例如下<br />  
//JS<br />  
var numRun = $(".numberRun").numberAnimate({num:'15343242.10', dot:2, speed:2000, symbol:","});<br />  
var nums = 15343242.10;<br />  
setInterval(function(){<br />  
    nums+= 3433.24;<br />  
    numRun.resetData(nums);<br />  
},3000);<br />  
