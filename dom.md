# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<script>

//DOM : Document Object Modeling
	window.onload = function(){
		//로직을 작성...
		//1.노드 생성(태그, 내용)
		var h1=document.createElement('h1'); //<h1></h1>이 만들어진다.
		var text = document.createTextNode('Hello DOM!!');
		
		//2. 생성한 노드 연결...기존의 태그에 연결
		h1.appendChild(text);
		document.body.appendChild(h1);
		
		//3. 이미지 태그를 생성
		var img = document.createElement('img');
		img.setAttribute('src','../img/jack.jpg');
		img.setAttribute('width',300);
		img.setAttribute('height',350);
		
		//body 밑에 붙인다.
		document.body.appendChild(img);
	};

</script>
</head>
<body>

</body>
</html>

---------------------------------------------------------

<!-- 
DOM
html 문서의 조작과 관련된 api
html 문서 생성, 삭제, 변경, 검색...등등이 가능하다.
 -->
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<script>
	window.onload = function(){
		//1.
	/*var header1	= document.getElementById("header1");
	var header2	= document.getElementById("header2");
	var header3	= document.getElementById("header3");
	
	header1.innerHTML = '<h2><font color=red> Using getElementById()...</h2>';
	
	};*/
	
	//2.
	var headers = document.getElementsByTagName('h1');
	//alert(headers); 배열인지 아닌지 확인
	//alert(headers.length);//배열에 담긴 갯수 확인 : 3
	for(var i=0; i<header.length; i++){
		headers[i].innerHTML = "Using getElementsByTagName()..."
		}
	};

</script>
</head>
<body>
	<h1 id="header1">header - 1</h1>
	<h1 id="header2">header - 2</h1>
	<h1 id="header3">header - 3</h1>
</body>
</html>

-------------------------------------------------

<!-- 
getElementById()


 -->

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert tittle here</title>
<script>
	window.onload = function(){
	var cityarr =document.getElementsByName('city');
		for(var i=0; i<cityarr.length; i++){
			cityarr[i].innerHTML = 'getElementsByName['+i+']번째 접근';
		}
		
		var queryAll = document.querySelectorAll('.region');
		for(var i=0; i<queryAll.length; i++){
			queryAll[i].style.color='red';
		}
		
	};


</script>
</head>
<body>
	<p name="city">서울 교대 지점</p>
	<p name="city">서울 남부 지점</p>
	
	<p id="p1">Encore Academy 서초</p>
	<p id="p2">Encore Academy 남부</p>
	
	<p class="region">서초 지점은 교대역 14번 출구 300m 지점에 위치합니다.</p>
	<p class="region">남부 지점은 남부터미널역 2번 출구 150m 지점에 위치합니다.</p>
</body>
</html>


