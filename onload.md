# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<script type="text/javacript">

/*
  window.onload
  ::
  html 문서에 포함된 모든 컨텐츠가 메모리에 로드된 후에 실행되는 함수
  동일한 문서 (html)에 오직 하나만 사용 가능하다
  이것과 기능은 동일하나 여러개 함수 사용가능한 것이
  JQuery의 ready함수이다.
  
 */
 
window.onload = function(){

	var list = '';//값에 의해서 데이터 타입이 동적으로 할당
	
	//복합연산자 사용
	list +='<ul>';
	list +='<li>Hello</li>';
	// ---> <ul><li>Hello</li>
	list +='<li>JavaScript</li>';
	list +='</ul>';
	
	
	//list변수 안에 있는 축적된 모든 내용을 웹 브라우저에 출력
	//이때 document.어느 영역.innerHTML =  list;
	
	document.getElementById("wrap").innerHTML = list;
};
	

</script>
</head>
<body>
<h2>=====onload=====</h2>
<div id="wrap"></div>
</body>
</html>
