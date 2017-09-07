# monthly-calendar


<html>
	<head>
    	<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    	<title></title>
    </head>
    <style>
		#div1{
			height:560px;
			width:400px;
			background:#CCC;
			margin:20px auto;
			padding-top:1px;
		}
		#div2{
			height:350px;
			width:370px;
			background:#999;	
			margin:20px auto;
			
		}
		#div3{
			background:#999;
			height:160px;
			width:370px;
			margin:20px auto;
			text-align:center;
			padding-top:1px;
		}
		#div2 div{
			background:black;
			color:#FFF;
			height:80px;
			width:110px;
			float:left;
			text-align:center;
			line-height:70px;
			margin-left:10px;
			margin-top:5px;
		}
		#div4 span{
			display:none;
		}
    </style>
    <script>

    	window.onload = function(){
		var oDiv2=document.getElementById('div2');
		var oDiv3=document.getElementById('div3');
		var oDiv4=document.getElementById('div4');
		var aDiv1=oDiv2.getElementsByTagName('div');
		var aSpan=oDiv4.getElementsByTagName('span');
			
			for(var i=0; i<aDiv1.length; i++){
				aDiv1[i].index=i;
				
				aDiv1[i].onclick = function(){
					init();
					this.style.background='#fff';
					this.style.color='red';
					oDiv3.innerHTML = aSpan[this.index].innerHTML;
				}
			}
			function init(){
				for(var i=0; i<aDiv1.length; i++){
					aDiv1[i].style.background='black';
					aDiv1[i].style.color='white';
				}	
			}	
		} 
    </script>
    <body>
    	<div id="div1">
    		<div id="div2">
            	<div>1月</div>
                <div>2月</div>
                <div>3月</div>       
                <div>4月</div>
                <div>5月</div>
                <div>6月</div>     
                <div>7月</div>
                <div>8月</div>
                <div>9月</div>  
                <div>10月</div>
                <div>11月</div>
                <div>12月</div>     
            </div>
            <div id="div3">
			
            </div>
            <div id='div4'>
            	<span><h1>一月活动</h1><h2>这是一月的活动信息元旦节</h2></span>
                <span><h1>二月活动</h1><h2>这是二月的活动信息情人节</h2></span>
                <span><h1>三月活动</h1><h2>这是三月的活动信息国际劳动妇女节</h2></span>
                <span><h1>四月活动</h1><h2>这是四月的活动信息清明节</h2></span>
                <span><h1>五月活动</h1><h2>这是五月的活动信息母亲节</h2></span>
                <span><h1>六月活动</h1><h2>这是六月的活动信息父亲节</h2></span>
                <span><h1>七月活动</h1><h2>这是七月的活动信息中国共党建党纪念日</h2></span>
                <span><h1>八月活动</h1><h2>这是八月的活动信息建军节</h2></span>
                <span><h1>九月活动</h1><h2>这是九月的活动信息教师节</h2></span>
                <span><h1>十月活动</h1><h2>这是十月的活动信息国庆节</h2></span>
                <span><h1>十一月活动</h1><h2>这是十一月的活动信息感恩节</h2></span>
                <span><h1>十二月活动</h1><h2>这是十二月的活动信息圣诞节</h2></span>
             </div>
       	</div>
    </body>
</html>
