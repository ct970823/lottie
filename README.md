# lottie web动画

#### 介绍
使用json动画在网页中呈现动画（lottie）

#### 使用说明

1.  引入lottie官方的js
    <script src="https://cdnjs.cloudflare.com/ajax/libs/bodymovin/5.6.6/lottie.min.js" type="text/javascript"></script> 
2.  引入动画json文件，由于script引入json在使用时会报错，在json文件中自定义变量 var animationData = {}
3.  创建div用来放置动画
4.  写入js
    var animation = bodymovin.loadAnimation({
	    container: document.getElementById('lottie'), // Required
	    renderer: 'svg', // Required
	    loop: true, // Optional
	    autoplay: true, // Optional
	    animationData: animationData // Name for future reference. Optional.
	})    

