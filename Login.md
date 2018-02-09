<!DOCTYPE html>
<html>
<head>
<script>

 function p1(){
                document.getElementById("q1").innerHTML="";
                document.getElementById("q2").innerHTML="";
                var name = document.getElementById("name").value;
                var pw = document.getElementById("pw").value;
                if(name=="123"){
                    if(pw=="123"){
                       document.write("登录成功，loading...");
                    }else{
                        document.getElementById("q2").innerHTML="密码错误！温馨提示：默认密码为123。"; 
						document.getElementById("pw").value="";
                    }
                }else{
                    document.getElementById("q1").innerHTML="帐号错误！温馨提示：默认帐号为123。";
					document.getElementById("name").value="";
                }	         
            }

</script>
</head>	
	
<body>
	<div  class="jdt">
		<h2  style="text-align:center;">用户登录</h2><br>
		账 户：<input type=" text" name="name" value="" id="name" onfocus="onover();"  onblur="onout();"/>
		<span id ="q1"></span><br><br>
		密 码：<input type="text" name="password" value="" id="pw" onfocus="onover1();"  onblur="onout1();"/>
		<span id ="q2"></span><br><br>
		<input type="button" name="an" value="登录" onclick="p1();">
	</div>
</body>
</html>
