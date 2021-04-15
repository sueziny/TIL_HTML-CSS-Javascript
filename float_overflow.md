# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<style type="text/css">
	#wrap{
		border:1px solid black;
		padding:10px;
		overflow:hidden;
	}
	#a{
		border:1px solid red;
		margin:0px;
		 /* 자식 요소에서 float 속성 사용시 부모 요소 범위를 벗어나게 된다.
			1. 부모 요소 범위의 사이즈를 크게 잡아버린다.
			2. overflow : hidden주는 방법이 있다.---부모 요소에 지정한다.
		 */
		float: left;   
	}
	#b{
		border:1px solid red;
		margin:0px;
		height:30px;
		float: left;
	}
	

</style>
</head>
<body>
<div id="wrap">
	<div id="a">
		Encore
	</div>
</div>
<div id="b">
	Play
</div>
</body>
</html>
