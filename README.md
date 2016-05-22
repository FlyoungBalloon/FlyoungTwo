<!doctype html>
<html lang="zh-cn">
<head>
	<meta charset="zh-cn">
	<title>You can't click me</title>
	<script src="http://code.jquery.com/jquery-latest.min.js"></script>
	<script type="text/javascript">
	function move(){
		var coords=new Array(10,50,100,130,175,225,260,300,320,350);
		var x=coords[Math.floor((Math.random()*10))];       //产生数组里的任意一个数
		var y=coords[Math.floor((Math.random()*10))];
		$("#elusiveText").css({"top":y+"px","left":x+"px"})   //改变位置
	}
	</script>
	<style type="text/css">
	span{
		background: #0066AA;
		color: #FFFFFF;
		font-weight: bold;
		border-color: #c0c0c0;
		border: 2px solid;
		border-radius: 5px;
		padding: 3px;
		position: absolute;
		top: 150px;
		left: 100px;
	}
	</style>
</head>
<body>
	<span id="elusiveText" onmouseover="move()">Please click me</span>
</body>
</html>
