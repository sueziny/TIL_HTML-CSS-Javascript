# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>margin, padding</title>
<!-- 외부에 분리시킨 css파일을 연결해서 사용하는 방법 -->
<link rel="stylesheet" type="text/css" href="css/css01.css">
<style type="text/css">
	@IMPORT url("./css/css01.css");
	
	#wrap{
		color: blue;
	}
</style>
</head>
<body>
<h2>외부 파일 재사용성 :: link 태그를 이용해서 css를 별도로 저장한다</h2>
<div>
	<h1>CONTENT</h1>
</div>	
<div id="wrap">
	<h3>@IMPORT 방법으로 연결하기</h3>
</div>
</body>
</html>
